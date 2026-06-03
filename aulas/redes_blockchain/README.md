<p align="center">
    <img src="../../others/assets/banner_blockas.png" alt="Banner Blockas">
</p>

# Guia de Estudo: Estudo Comparativo Avançado de Redes Blockchain

Este material foi desenvolvido para os membros do Inteli Blockchain como um documento de referência técnica avançada. O objetivo é fornecer um estudo comparativo aprofundado sobre a evolução das principais redes blockchain, seus modelos de consenso, arquiteturas de execução e implementação prática.

Antes de ler o material, recomenda-se a leitura de palavras técnicas no [dicionário](./dicionario.md) para facilitar o entendimento do conteúdo.

---

## Introdução: Gênese Histórica e Evolução Tecnológica

O desenvolvimento de redes blockchain modernas não representa uma ruptura tecnológica isolada, mas sim a convergência de mais de quatro décadas de pesquisa em criptografia, sistemas distribuídos e teoria dos jogos. O núcleo conceitual do registro distribuído (ledger) baseia-se em propostas que buscavam resolver a descentralização de dados e a garantia de escassez digital sem intermediários.

A fundação dessa tecnologia foi construída em etapas:
* **1982:** David Chaum propôs sistemas de computação confiáveis mantidos por grupos mutuamente suspeitos.
* **1991:** Stuart Haber e W. Scott Stornetta introduziram o encadeamento cronológico de blocos por meio de hashes criptográficos para evitar a adulteração de documentos.
* **1997:** Adam Back desenvolveu o *Hashcash*, um sistema de prova de trabalho (PoW) inicialmente criado para combater o spam de e-mails, que viria a ser o motor da validação de blocos.
* **1998:** Wei Dai (*b-money*) e Nick Szabo (*bit gold*) estruturaram modelos teóricos de dinheiro eletrônico baseados em esforço computacional e chaves públicas.

A síntese definitiva ocorreu no final de 2008, impulsionada pelo cenário de instabilidade macroeconômica global gerado pela crise financeira. A primeira implementação prática materializou essas décadas de pesquisa, originando a tecnologia que hoje chamamos de blockchain.

---

## 1. Bitcoin (BTC)

### Contexto de Surgimento e Propósito
O Bitcoin surgiu formalmente em 31 de outubro de 2008 com a publicação do whitepaper *"Bitcoin: A Peer-to-Peer Electronic Cash System"*, de autoria do pseudônimo Satoshi Nakamoto. O propósito era estabelecer uma arquitetura de dinheiro eletrônico puramente ponto a ponto, sem a necessidade de custódia de bancos centrais. A rede foi iniciada em 3 de janeiro de 2009 (Bloco Gênese), trazendo embutida a manchete do jornal The Times: *"Chancellor on brink of second bailout for banks"*, um protesto histórico contra o sistema financeiro tradicional. A primeira precificação real ocorreu em 2010, quando Laszlo Hanyecz comprou duas pizzas por 10.000 BTC.

### Mecanismo de Consenso
Para garantir a imutabilidade e evitar o gasto duplo de tokens (Double Spending), o Bitcoin utiliza o algoritmo de **Prova de Trabalho (PoW - Proof of Work)**. Os nós competem computacionalmente para encontrar um *nonce* que faça o hash do bloco atender à dificuldade da rede.
A assinatura de transações baseia-se na criptografia de curva elíptica ECDSA (curva `secp256k1`). A política monetária é inviolável e ditada por matemática: a recompensa dos blocos cai pela metade a cada 210.000 blocos (evento chamado *Halving*), limitando o fornecimento máximo histórico estritamente a 21 milhões de unidades.

### Pontos Fortes e Fracos
* **Pontos Fortes:** Apresenta o mais elevado nível de segurança criptográfica acumulada e extrema descentralização. É totalmente resistente à censura, consolidando-se no mercado institucional como a principal reserva de valor global (ouro digital).
* **Pontos Fracos:** O *throughput* (capacidade de processamento) é severamente limitado a cerca de 7 transações por segundo (TPS), com tempo de bloco em torno de 10 minutos. O modelo PoW demanda altíssimo consumo de energia elétrica. Além disso, a linguagem de script nativa não é *Turing-complete*, impedindo contratos inteligentes complexos na camada principal.

### Protocolos e Evolução Técnica
* **Lightning Network:** Rede de segunda camada (Layer-2) que opera via canais bidirecionais (HTLCs), permitindo micropagamentos quase instantâneos e taxas baixíssimas, superando a lentidão da camada base.
* **Taproot:** Atualização estrutural ativada em 2021. Trouxe as Assinaturas Schnorr (que agregam chaves públicas para aumentar a privacidade) e as Árvores MAST (que otimizam o armazenamento revelando apenas a condição do script que foi ativada).
* **Taproot Assets Protocol (TAP):** Permite a emissão e transferência de ativos digitais customizados (como stablecoins) diretamente na rede Bitcoin, operando em sinergia com a Lightning Network.

---

## 2. Ethereum (ETH)

### Contexto de Surgimento e Propósito
As limitações de script do Bitcoin evidenciaram a necessidade de uma rede flexível capaz de executar lógicas condicionais complexas. Em 2013, Vitalik Buterin propôs o Ethereum, lançado oficialmente em 2015, com o objetivo de atuar não apenas como uma contabilidade de saldos, mas como um computador global descentralizado. Através dele, tornou-se possível hospedar contratos inteligentes autônomos que processam dados de forma determinística e imutável.

### Mecanismo de Consenso
Originalmente estruturado em PoW, o Ethereum realizou a transição de arquitetura em setembro de 2022 (conhecida como *"The Merge"*), passando a utilizar o consenso de **Prova de Participação (PoS - Proof of Stake)**.
Nesse sistema, a criação de blocos é mantida por nós validadores que bloqueiam (*staking*) 32 ETH. Comportamentos maliciosos geram cortes punitivos do saldo (*slashing*). O fornecimento do token tornou-se dinâmico, sendo ajustado pela emissão versus a queima automática de taxas de uso (implementada pela EIP-1559).

### Pontos Fortes e Fracos
* **Pontos Fortes:** Possui a infraestrutura de liquidez e desenvolvedores mais densa do ecossistema. Executa de forma nativa a **EVM (Ethereum Virtual Machine)**, que suporta contratos *Turing-complete*, sendo a espinha dorsal de aplicações de Finanças Descentralizadas (DeFi) e NFTs.
* **Pontos Fracos:** O processamento sequencial da EVM restringe a capacidade da camada principal (Layer-1) a apenas 15-30 TPS. Em momentos de alta demanda, a rede sofre congestionamentos, resultando em taxas (*gas fees*) proibitivas.

### Protocolos e Evolução Técnica
* **Padrões ERC:** O ecossistema desenvolveu diretrizes unificadas de interoperabilidade, com destaque para o ERC-20 (tokens fungíveis) e ERC-721 (NFTs).
* **Layer-2 Rollups:** A solução para escalabilidade migrou para as segundas camadas (como Arbitrum, Optimism e Base). Essas L2 executam milhares de transações e enviam apenas provas criptográficas consolidadas de volta à rede principal, garantindo segurança a custos irrisórios.
* **Pectra:** Próxima grande atualização planejada para implementar a "Abstração de Conta" e otimizar ainda mais o processamento e a precificação de dados para as redes Layer-2.

---

## 3. Solana (SOL)

### Contexto de Surgimento e Propósito
O processamento linear de transações e a alta latência limitavam a adoção da blockchain pelo mercado financeiro de alta frequência. Em 2017, Anatoly Yakovenko identificou que o gargalo era a coordenação cronológica entre nós distribuídos no mundo. O protocolo Solana foi projetado e lançado em 2020 para superar essa limitação, introduzindo um relógio criptográfico descentralizado que permite aos nós sincronizarem o tempo sem depender de aprovações constantes.

### Mecanismo de Consenso
A Solana utiliza uma arquitetura híbrida focada em velocidade máxima. Ela combina o PoS para governança e segurança de rede com o inovador **Proof of History (PoH)** para marcação temporal.
O PoH atua como um carimbo de tempo sequencial (*Verifiable Delay Function* em SHA-256) que prova a ordem exata das transações. Como todos sabem *quando* algo aconteceu, os nós podem reconstruir o histórico e validar os blocos de forma assíncrona.

### Pontos Fortes e Fracos
* **Pontos Fortes:** Capacidade massiva de processamento em larga escala, atingindo rotineiramente milhares de TPS (com picos teóricos de 65.000). Tempos de confirmação em milissegundos e taxas extremamente baratas (~0,00025 SOL), tornando-se a favorita para redes DePIN e aplicações de consumo.
* **Pontos Fracos:** A velocidade exige especificações de hardware de altíssimo nível, aumentando a centralização e dificultando a criação de nós individuais. A complexidade do sistema resultou em histórico de paralisações temporárias (*outages*) da rede devido ao estresse de *bots*.

### Protocolos e Evolução Técnica
* **Sealevel & Gulf Stream:** O *Sealevel* é o motor da Solana que processa contratos inteligentes simultaneamente (execução paralela), enquanto o *Gulf Stream* descarta a fila de espera (*mempool*), enviando transações diretas aos validadores.
* **Token Extensions (Token-2022):** Uma expansão da Solana Program Library (SPL) que fornece ferramentas de conformidade nativas, como transferências privadas com *Zero-Knowledge Proofs* e controle de congelamento de ativos.
* **Firedancer:** Um novo cliente validador de alto desempenho sendo programado em C/C++ de forma independente pela Jump Crypto, buscando adicionar redundância vital para evitar futuras quedas na rede.

---

## 4. Stellar (XLM)

### Contexto de Surgimento e Propósito
Ao contrário das redes focadas em dApps especulativos, a Stellar foi estruturada em 2014 por Jed McCaleb com foco institucional claro: viabilizar pagamentos transfronteiriços, microcréditos e representação de moedas soberanas tradicionais (Dólar, Euro, Real) de forma ágil e de baixo custo, conectando os desbancarizados e instituições financeiras.

### Mecanismo de Consenso
A rede afasta-se totalmente da mineração PoW ou do staking financeiro PoS. Ela adota o **Stellar Consensus Protocol (SCP)**, a primeira aplicação prática do Acordo Bizantino Federado (FBA). No SCP, cada validador escolhe autonomamente um pequeno grupo de validadores em quem confia (*Quorum Slice*). O consenso final da rede é alcançado de forma orgânica pela intersecção matemática global dessas fatias (*Quorum Intersection*).

### Pontos Fortes e Fracos
* **Pontos Fortes:** Custos praticamente inexistentes e finalização instantânea de transações (2 a 5 segundos). Possui um histórico impecável de estabilidade (zero *downtime* desde 2014). Oferece recursos robustos de conformidade corporativa para bancos.
* **Pontos Fracos:** Foco estreito em pagamentos a deixou, por muitos anos, defasada no desenvolvimento de contratos inteligentes e DeFi para o mercado de varejo especulativo, além de críticas sobre centralização das decisões pela Stellar Development Foundation (SDF).

### Protocolos e Evolução Técnica
* **Anchors e Trustlines:** O protocolo exige que os usuários registrem o aceite prévio de um token (*Trustline*) antes de recebê-lo, prevenindo fraudes e *spam*. Os ativos geralmente são emitidos por *Anchors*, instituições que custodiam o valor fiduciário físico (1:1).
* **DEX Nativa:** A rede possui um livro de ofertas embutido diretamente na Camada 1 (Layer-1), permitindo conversões e trocas instantâneas (ex: remetente envia Real, destinatário recebe Dólar na outra ponta).
* **Soroban:** Uma expansão recente e maciça lançada em 2024. É a plataforma de contratos inteligentes nativa da Stellar, escrita em Rust e executada via *WebAssembly (Wasm)*. A Soroban introduziu um "Modelo de Estado Inteligente" de três níveis de memória (Temporário, Instância e Persistente) para evitar inchaço do armazenamento da rede.

---

## 5. Análise Comparativa Multidimensional

O quadro comparativo abaixo sintetiza os aspectos cruciais e os compromissos (trade-offs) arquiteturais assumidos por cada uma das redes analisadas:

| Dimensão de Comparação | Bitcoin (BTC) | Ethereum (ETH) | Solana (SOL) | Stellar (XLM) |
| :--- | :--- | :--- | :--- | :--- |
| **Arquitetura Base de Transação** | Modelo UTXO | Modelo de Contas (Estado Global) | Modelo de Contas (Estado Isolado) | Modelo de Contas (Saldos com Trustlines) |
| **Throughput Médio da Camada Base** | ~7 TPS | ~15 a 30 TPS | 1.000 a 3.000 TPS estáveis (pico de 65.000) | ~1.000 TPS estáveis |
| **Latência / Confirmação de Finalidade** | ~10 a 60 minutos | ~12 a 15 segundos no L1 | ~400 milissegundos | ~2 a 5 segundos |
| **Estrutura Média de Tarifas** | Variável, elevada sob estresse | Alta no L1, centavos nas redes L2 | Extremamente barata (~0,00025 SOL) | Irrisória (frações mínimas de centavo) |
| **Paradigmas de Programação** | Scripts lineares restritos (não *Turing-complete*) | Contratos inteligentes *Turing-complete* (Solidity) | Programas paralelos em Rust/C++ | Contratos rápidos via Soroban (Rust/Wasm) |
| **Política de Fornecimento de Tokens** | Fixo de 21M, deflacionário por halving | Sem teto, dinâmico conforme queima de *gas* | Inflação decrescente base de 4,5% | Fixo de 50 Bilhões, sem processos inflacionários |