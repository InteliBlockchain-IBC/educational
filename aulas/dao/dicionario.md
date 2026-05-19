<p align="center">
    <img src="../../others/assets/banner_blockas.png" alt="Banner Blockas">
</p>

# Dicionário de Organizações Autônomas Descentralizadas (DAOs)

Este dicionário reúne os principais termos técnicos e conceitos do ecossistema de DAOs e governança descentralizada. Cada termo acompanha uma definição clara e um link para um material de estudo aprofundado.

Para voltar ao material principal [clique aqui](./README.md)

**Índice Remissivo:**
[ A ](#a) | [ C ](#c) | [ D ](#d) | [ E ](#e) | [ F ](#f) | [ G ](#g) | [ H ](#h) | [ I ](#i) | [ M ](#m) | [ O ](#o) | [ R ](#r) | [ S ](#s) | [ T ](#t)

---

### A

**Ataque de Reentrância (Reentrancy Attack)**
Vulnerabilidade em contratos inteligentes onde uma função maliciosa consegue chamar a si mesma repetidamente antes de atualizar o estado e os saldos, permitindo drenar os fundos do contrato.

- [Aprofunde-se sobre Ataques de Reentrância](https://consensys.github.io/smart-contract-best-practices/attacks/reentrancy/)

### C

**Checkpoints**
Mecanismo técnico em tokens de governança que registra o saldo dos usuários em blocos específicos da rede, evitando que atores maliciosos comprem tokens no momento da votação apenas para manipulá-la e os vendam logo em seguida.

- [Aprofunde-se sobre Checkpoints na governança](https://docs.openzeppelin.com/contracts/4.x/api/token/erc20#ERC20Votes)

### D

**DAO (Decentralized Autonomous Organization)**
Organização corporativa sem uma liderança central humana, cujas regras estatutárias, governança e tesouraria são codificadas e executadas por contratos inteligentes de forma transparente na blockchain.

- [Aprofunde-se no conceito de DAO](https://ethereum.org/pt-br/dao/)

**Descentralização Progressiva**
Framework de desenvolvimento estratégico onde um projeto inicia de forma centralizada (para garantir agilidade e segurança) e gradualmente transfere o controle do protocolo e a tesouraria para a comunidade.

- [Aprofunde-se sobre Descentralização Progressiva](https://a16zcrypto.com/posts/article/progressive-decentralization-a-playbook-for-building-crypto-applications/)

### E

**Espiral da Morte (Death Spiral)**
Cenário de colapso econômico que ocorre quando uma DAO mantém a maior parte de sua tesouraria no próprio token nativo; uma queda de preço força a organização a vender mais tokens para se financiar, derrubando o valor a zero.

- [Aprofunde-se sobre a Gestão de Tesouraria em DAOs](https://a16zcrypto.com/posts/article/dao-treasury-management/)

### F

**Flash Loan (Empréstimo Relâmpago)**
Empréstimo não colateralizado de criptomoedas onde um alto valor deve ser emprestado e devolvido obrigatoriamente dentro do mesmo bloco de transação. Muito utilizado por atacantes para tentar fraudar sistemas de votação.

- [Aprofunde-se sobre Flash Loans](https://aave.com/docs/concepts/flash-loans/)

### G

**Gnosis Safe (Safe)**
A plataforma de contrato inteligente mais consolidada do mercado utilizada por DAOs para criar carteiras de múltiplas assinaturas, armazenando a tesouraria corporativa com alta segurança.

- [Aprofunde-se sobre o Gnosis Safe](https://safe.global/)

**Governor (Contrato do Governador)**
O contrato inteligente que funciona como o cérebro em uma DAO. Ele contém a lógica matemática para receber propostas, definir o período eleitoral, calcular o quórum e registrar a contagem dos votos on-chain.

- [Aprofunde-se sobre o padrão OpenZeppelin Governor](https://docs.openzeppelin.com/contracts/4.x/governance)

### H

**Hard Fork**
Uma alteração radical e incompatível no protocolo de uma blockchain que força a rede a se dividir permanentemente em duas, como ocorreu na separação entre Ethereum (ETH) e Ethereum Classic (ETC) após o hack do "The DAO".

- [Aprofunde-se sobre Hard Forks](https://www.investopedia.com/terms/h/hard-fork.asp)

### I

**IPFS (InterPlanetary File System)**
Rede descentralizada e global de armazenamento e compartilhamento de arquivos. É amplamente utilizada para salvar de forma imutável os recibos das votações off-chain gerados por plataformas como o Snapshot.

- [Aprofunde-se sobre o funcionamento do IPFS](https://ipfs.tech/)

### M

**Multi-Sig (Múltiplas Assinaturas)**
Configuração de segurança para carteiras digitais que exige que um número mínimo de usuários previamente aprovados (ex: 3 de 5) assinem uma transação antes que ela seja autorizada e enviada para a blockchain.

- [Aprofunde-se sobre Carteiras Multi-Sig](https://ethereum.org/pt-br/wallets/)

### O

**OpenZeppelin**
Biblioteca padrão da indústria que fornece implementações auditadas e altamente seguras de contratos inteligentes, oferecendo os moldes para criar tanto os tokens de votação quanto os contratos de governança.

- [Aprofunde-se sobre a OpenZeppelin](https://www.openzeppelin.com/)

### R

**Ragequit**
Mecanismo de segurança estrutural que permite a um membro discordante retirar seus fundos ou sua liquidez da tesouraria da DAO antes que uma proposta aprovada com a qual ele não concorda seja executada on-chain.

- [Aprofunde-se sobre o conceito de Ragequit](https://wengal.medium.com/what-is-ragequit-in-a-dao-4017f86f78f8)

### S

**Snapshot**
Plataforma off-chain padrão do mercado utilizada por DAOs para realizar votações sem custo de Gas (taxas de rede), onde os membros apenas assinam criptograficamente suas decisões baseadas no seu saldo de tokens.

- [Aprofunde-se sobre o Snapshot](https://snapshot.org/)

### T

**Timelock (Trava de Tempo)**
Contrato inteligente de segurança que guarda os fundos da organização e impõe um atraso temporal obrigatório (ex: 48 horas) entre a aprovação de uma proposta e a sua execução real, permitindo revisões em caso de ataques.

- [Aprofunde-se sobre o funcionamento do Timelock](https://docs.openzeppelin.com/contracts/4.x/api/governance#TimelockController)