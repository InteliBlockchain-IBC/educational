<p align="center">
    <img src="../../others/assets/banner_blockas.png" alt="Banner Blockas">
</p>

# Guia de Estudo: Organizações Autônomas Descentralizadas (DAOs)

Este material foi desenvolvido para os membros do Inteli Blockchain como um documento de referência e consulta contínua. O objetivo é fornecer uma base teórica e técnica sólida sobre as DAOs, detalhando desde a sua origem histórica e arquitetura de contratos inteligentes até os fluxos operacionais híbridos utilizados pelo mercado atual. Utilize este guia para embasar o desenvolvimento de sistemas de governança on-chain e off-chain.

Antes de ler o material, recomenda-se a leitura de palavras técnicas no [dicionário](./dicionario.md) para facilitar o entendimento do conteúdo.

---

## 1. A Origem Histórica e o Dilema "Code is Law"

O conceito de organizações descentralizadas não nasceu perfeito; foi moldado por um dos eventos mais críticos da história da criptografia.

### O Caso "The DAO" (2016)

A primeira grande implementação prática de governança descentralizada foi um fundo de investimento chamado simplesmente de "The DAO", lançado na rede Ethereum. O projeto arrecadou cerca de 150 milhões de dólares (14% de todo o Ether em circulação na época). Semanas após o lançamento, um hacker explorou uma vulnerabilidade no código (Ataque de Reentrância) e drenou 50 milhões de dólares do contrato.

Isso gerou um dilema filosófico: intervir e reescrever o histórico da blockchain para devolver o dinheiro (quebrando a imutabilidade), ou aceitar que "o código é a lei" e deixar o hacker com os fundos. A maioria da comunidade decidiu fazer um Hard Fork para devolver os fundos (versão que hoje conhecemos como a rede Ethereum principal - ETH). A minoria que discordou continuou rodando o histórico antigo (Ethereum Classic - ETC). Esse evento provou que a segurança da arquitetura de uma DAO deve ser construída com extrema cautela.

---

## 2. Arquitetura de Código: Como uma DAO funciona na Blockchain?

Uma DAO moderna não é um único contrato inteligente, mas um ecossistema de contratos interconectados que assumem diferentes papéis na governança. O padrão mais utilizado hoje é baseado na arquitetura OpenZeppelin Governor, dividida em três pilares:

### O Contrato do Token (ERC-20 Votes)

Diferente de um token comum, o token de governança possui uma mecânica de "checkpoints" (pontos de verificação). Ele registra o histórico de saldos em blocos específicos da rede. Isso evita que atores maliciosos comprem tokens no momento da votação, votem, e vendam logo em seguida.

### O Contrato do Governador (Governor)

É o cérebro da organização. Ele contém a lógica matemática para a criação de propostas, definição do período de votação, cálculo de quórum (participação mínima exigida) e contagem dos votos.

### A Trava de Tempo (Timelock) e o Cofre

O Governador não guarda os fundos da DAO. Quem armazena o dinheiro e tem a permissão final para alterar regras do protocolo é o contrato Timelock. O Governador apenas aprova uma decisão e envia uma ordem de execução para o Timelock.

---

## 3. A Anatomia de uma Proposta On-Chain

Uma proposta votada em uma DAO não é um documento de texto, mas um pacote de dados executáveis. Quando os membros votam para realizar uma ação (ex: transferir 10 ETH), o contrato armazena parâmetros técnicos precisos:

- **Target:** O endereço do contrato que será afetado (ex: a tesouraria).
- **Value:** A quantidade de criptomoeda nativa envolvida na transação.
- **Signature:** A função específica que será chamada no contrato alvo (ex: `transfer`).
- **Calldata:** Os argumentos em formato hexadecimal que alimentam essa função.

Se a proposta for aprovada, o código pega esses parâmetros e faz uma chamada de baixo nível (`low-level call`) na blockchain. A transação acontece sem que nenhum humano precise assinar a transferência final.

---

## 4. Mecanismos de Segurança Institucional

Para evitar manipulações de mercado e falhas sistêmicas, a engenharia de contratos para DAOs evoluiu com mecanismos de proteção essenciais:

- **Defesa contra Flash Loans:** O sistema de checkpoints do token garante que empréstimos relâmpago não possam ser usados para acumular poder de voto momentâneo. O contrato contabiliza apenas os tokens que o eleitor possuía antes da proposta ser criada.
- **Atraso de Execução (Timelock Delay):** Quando uma proposta é aprovada, ela não é executada imediatamente. O Timelock impõe um atraso obrigatório (ex: 48 horas). Isso serve como uma saída de emergência: se uma decisão maliciosa passar, a minoria tem tempo hábil para vender seus tokens ou retirar sua liquidez do protocolo antes da execução.
- **Multi-Sigs e Guardians:** Em DAOs mais jovens, o Timelock pode ser controlado por um grupo de membros de confiança (Guardians) através de uma carteira de múltiplas assinaturas. Em caso de falha crítica no código, eles podem vetar uma transação letal.

---

## 5. O Fluxo de Governança Híbrida (Off-chain e On-chain)

O custo computacional (Gas) da rede Ethereum torna financeiramente inviável votar todas as micro-decisões diretamente na blockchain. Para contornar isso e evitar a exclusão de pequenos detentores de tokens, o mercado adotou o fluxo híbrido:

1. **Ideação Off-chain:** O debate da proposta ocorre em fóruns (Discourse) ou canais de comunicação (Discord), onde a comunidade molda a ideia.
2. **Votação sem custo (Snapshot):** A proposta madura vai para uma plataforma off-chain (como o Snapshot). Os membros assinam digitalmente seus votos de forma gratuita. O sistema lê o saldo de tokens diretamente da blockchain e armazena o resultado criptograficamente no IPFS.
3. **Execução On-chain (Gnosis Safe):** Se aprovada, a decisão precisa ser materializada. Um conselho eleito utiliza a tesouraria multi-assinatura (Safe) para executar na blockchain exatamente aquilo que a comunidade aprovou no Snapshot.

---

## 6. Modelos de Maturidade e Gestão Financeira

A implementação de uma DAO não termina no deploy do contrato inteligente; ela exige estruturação de governança corporativa e gestão de risco.

### Descentralização Progressiva

Projetos complexos não nascem 100% descentralizados. O framework de descentralização progressiva é o padrão do mercado:
- **Estágio 1:** A equipe fundadora mantém o controle total para iterar rápido e encontrar o ajuste do produto no mercado.
- **Estágio 2:** O token é lançado e a comunidade começa a votar em parâmetros secundários, enquanto a equipe mantém chaves de administrador (God Mode) para emergências.
- **Estágio 3:** A equipe fundadora destrói as chaves de administrador. O protocolo passa a ser governado única e exclusivamente pelos contratos inteligentes e pela comunidade.

### Gestão de Tesouraria e a "Espiral da Morte"

Um dos maiores erros estruturais em DAOs é manter 100% dos fundos no seu próprio token nativo. Se o mercado retrair e o valor do token despencar, a organização perde a capacidade de pagar colaboradores, forçando a venda de mais tokens e criando uma espiral de desvalorização. Uma tesouraria saudável deve aprovar a diversificação de seus ativos, convertendo parte das receitas em Stablecoins (ex: USDC) e ativos de reserva globais (ex: ETH e BTC) para garantir resiliência operacional a longo prazo.