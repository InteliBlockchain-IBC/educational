<p align="center">
	<img src="../others/assets/banner_blockas.png" alt="Banner Blockas">
</p>

# Materiais Adicionais de Estudo: Trilha de Aprendizagem Blockchain

Materiais de introdução, aprofundamento e prática para membros em blockchain. Prioridade para recursos em português e, quando necessário, complementos em inglês com qualidade técnica relevante. Cobre fundamentos, redes importantes, cursos, artigos, whitepapers, ferramentas, comunidades e uso de IA aplicado ao desenvolvimento em Bitcoin, Ethereum, Solana e Stellar.

## Sumário Geral

1. [Como usar este documento](#1-como-usar-este-documento)
   - [1.1 Sistema de tags e busca](#11-sistema-de-tags-e-busca)
2. [Livros de referência](#2-livros-de-referência)
   - [2.1 Fundamentos gerais](#21-fundamentos-gerais)
   - [2.2 Bitcoin](#22-bitcoin)
   - [2.3 Ethereum e smart contracts](#23-ethereum-e-smart-contracts)
3. [Guias iniciantes de redes importantes](#3-guias-iniciantes-de-redes-importantes)
   - [3.1 Bitcoin](#31-bitcoin)
   - [3.2 Ethereum](#32-ethereum)
   - [3.3 Solana](#33-solana)
   - [3.4 Stellar](#34-stellar)
4. [Cursos em sites](#4-cursos-em-sites)
5. [Cursos em vídeo e bootcamps](#5-cursos-em-vídeo-e-bootcamps)
6. [Artigos, blogs e newsletters](#6-artigos-blogs-e-newsletters)
   - [6.1 Hubs por ecossistema](#61-hubs-por-ecossistema)
   - [6.2 Blogs e newsletters técnicas](#62-blogs-e-newsletters-técnicas)
7. [Whitepapers fundamentais](#7-whitepapers-fundamentais)
8. [Ferramentas de desenvolvimento e segurança](#8-ferramentas-de-desenvolvimento-e-segurança)
   - [8.1 Ferramentas EVM](#81-ferramentas-evm)
   - [8.2 Ferramentas Bitcoin](#82-ferramentas-bitcoin)
   - [8.3 Ferramentas Solana](#83-ferramentas-solana)
   - [8.4 Ferramentas Stellar](#84-ferramentas-stellar)
   - [8.5 Segurança](#85-segurança)
9. [Comunidades e ecossistemas](#9-comunidades-e-ecossistemas)
   - [9.1 Comunidades por rede](#91-comunidades-por-rede)
   - [9.2 Fóruns e discussões técnicas](#92-fóruns-e-discussões-técnicas)
10. [IA para desenvolvimento blockchain](#10-ia-para-desenvolvimento-blockchain)
    - [10.1 Onde IA ajuda de verdade](#101-onde-ia-ajuda-de-verdade)
    - [10.2 Ferramentas e materiais](#102-ferramentas-e-materiais)
    - [10.3 Prompts úteis](#103-prompts-úteis)
    - [10.4 Skills para alunos](#104-skills-para-alunos)
11. [Trilha de aprendizagem](#11-trilha-de-aprendizagem)
    - [11.1 Quero entender a tecnologia](#111-quero-entender-a-tecnologia)
    - [11.2 Desenvolvimento Ethereum / EVM](#112-desenvolvimento-ethereum--evm)
    - [11.3 Desenvolvimento Solana](#113-desenvolvimento-solana)
    - [11.4 Desenvolvimento Stellar](#114-desenvolvimento-stellar)
    - [11.5 Bitcoin — protocolo e integração](#115-bitcoin--protocolo-e-integração)
    - [11.6 Segurança de contratos](#116-segurança-de-contratos)

---

## 1. Como usar este documento

O documento está dividido por tipo de recurso: livros, guias de rede, cursos, artigos, whitepapers, ferramentas, comunidades e uso de IA. Cada item tem tags para filtrar por rede, idioma, nível e foco. Para um caminho estruturado, vá direto para a seção [11. Trilha de aprendizagem](#11-trilha-de-aprendizagem) e escolha o perfil que melhor descreve seu objetivo atual.

### 1.1 Sistema de tags e busca

Cada recurso é marcado com tags no formato `#nome`. Para buscar por interesse, use **Ctrl+F** (ou Cmd+F) e pesquise a tag — todos os recursos com aquela tag aparecerão. Combine tags para filtrar com mais precisão: `#ethereum` + `#português` retorna somente materiais de Ethereum em português; `#segurança` + `#avançado` filtra conteúdo avançado de segurança.

**Tags por categoria:**

| Categoria | Tags disponíveis |
|-----------|-----------------|
| **Rede** | `#bitcoin` `#ethereum` `#solana` `#stellar` `#evm` `#l2` |
| **Idioma** | `#português` `#inglês` |
| **Nível** | `#iniciante` `#intermediário` `#avançado` |
| **Tipo de recurso** | `#whitepaper` `#artigos` `#newsletter` `#bootcamp` `#quickstart` `#ide` `#playground` |
| **Foco técnico** | `#fundamentos` `#desenvolvimento` `#segurança` `#smart-contracts` `#infra` `#pesquisa` `#ia` `#zk` `#defi` `#nft` `#payments` |
| **Linguagem / stack** | `#rust` `#solidity` `#anchor` `#soroban` `#foundry` `#hardhat` |
| **Operações** | `#cli` `#api` `#sdk` `#node` `#testes` `#debug` `#deploy` `#monitoring` |
| **Comunidade** | `#comunidade` `#fórum` `#core` `#contribuição` |
| **Outros** | `#criptografia` `#consenso` `#boas-práticas` `#dapps` `#upgrades` |

---

## 2. Livros de referência

Livros trazem profundidade que documentações fragmentadas não cobrem. Os selecionados aqui constroem base sólida de criptografia, sistemas distribuídos e arquitetura das principais redes — do protocolo ao desenvolvimento de aplicações.

- [2.1 Fundamentos gerais](#21-fundamentos-gerais)
- [2.2 Bitcoin](#22-bitcoin)
- [2.3 Ethereum e smart contracts](#23-ethereum-e-smart-contracts)

### 2.1 Fundamentos gerais

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| _Mastering Bitcoin_ — Antonopoulos | Explica transações, script, carteiras e arquitetura do Bitcoin do ponto de vista técnico. | Inglês | Intermediário | `#bitcoin #fundamentos #desenvolvimento #intermediário` | [GitHub / texto aberto](https://github.com/bitcoinbook/bitcoinbook) |
| _Mastering Ethereum_ — Antonopoulos e Wood | Referência para EVM, contas, transações, contratos, padrões e ecossistema Ethereum. | Inglês | Intermediário | `#ethereum #evm #smart-contracts #intermediário` | [GitHub / leitura online](https://github.com/ethereumbook/ethereumbook) |
| _Programming Bitcoin_ — Jimmy Song | Conecta teoria e implementação com foco em criptografia aplicada e código. | Inglês | Intermediário | `#bitcoin #desenvolvimento #criptografia #intermediário` | [O'Reilly](https://www.oreilly.com/library/view/programming-bitcoin/9781492031482/) |
| _Designing Data-Intensive Applications_ — Kleppmann | Base de sistemas distribuídos, consenso, replicação e arquitetura — não é blockchain, mas complementa muito. | Inglês | Avançado | `#fundamentos #consenso #infra #avançado` | [Site oficial](https://dataintensive.net) |

### 2.2 Bitcoin

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| _Mastering Bitcoin_ | Porta de entrada técnica para entender como a rede funciona de fato. | Inglês | Intermediário | `#bitcoin #fundamentos #intermediário` | [GitHub / texto aberto](https://github.com/bitcoinbook/bitcoinbook) |
| _Programming Bitcoin_ | Conecta criptografia aplicada e implementação; útil para quem tem perfil dev. | Inglês | Intermediário | `#bitcoin #desenvolvimento #criptografia` | [O'Reilly](https://www.oreilly.com/library/view/programming-bitcoin/9781492031482/) |
| _The Bitcoin Standard_ — Saifedean Ammous | Aborda a perspectiva monetária e histórica do Bitcoin. Não é técnico, mas útil para contexto. | Inglês | Iniciante | `#bitcoin #fundamentos #iniciante` | [Site oficial](https://saifedean.com/the-book/) |

### 2.3 Ethereum e smart contracts

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| _Mastering Ethereum_ | Cobre EVM, gas, contas, tooling e contratos inteligentes em profundidade. | Inglês | Intermediário | `#ethereum #evm #smart-contracts #intermediário` | [GitHub / leitura online](https://github.com/ethereumbook/ethereumbook) |
| _Smart Contract Security Field Guide_ — Trail of Bits | Guia prático de segurança para contratos inteligentes; cobre vetores de ataque e mitigações. | Inglês | Avançado | `#ethereum #segurança #smart-contracts #avançado` | [Acesse aqui](https://scsfg.io) |

---

## 3. Guias iniciantes de redes importantes

As documentações oficiais de cada rede são o melhor ponto de partida técnico: ensinam a arquitetura, o fluxo de desenvolvimento e as ferramentas padrão do ecossistema. Os quickstarts permitem colocar código rodando rapidamente sem depender de setup avançado.

- [3.1 Bitcoin](#31-bitcoin)
- [3.2 Ethereum](#32-ethereum)
- [3.3 Solana](#33-solana)
- [3.4 Stellar](#34-stellar)

### 3.1 Bitcoin

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| Bitcoin Developer Reference | Explica como o Bitcoin funciona para desenvolvedores: transações, scripts, RPC e APIs. | Inglês | Iniciante/Intermediário | `#bitcoin #desenvolvimento #fundamentos #inglês` | [Acesse aqui](https://developer.bitcoin.org/reference/intro.html) |
| Learn me a Bitcoin | Explicações visuais e progressivas sobre como o Bitcoin funciona internamente, do bloco à carteira. | Inglês | Iniciante | `#bitcoin #fundamentos #iniciante #inglês` | [Acesse aqui](https://learnmeabitcoin.com) |
| Bitcoin Development | Página de entrada para contribuir com o Bitcoin Core e entender o processo de desenvolvimento do protocolo. | Inglês | Intermediário | `#bitcoin #core #contribuição #inglês` | [Acesse aqui](https://bitcoin.org/en/development) |

### 3.2 Ethereum

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| Documentação para desenvolvedores do Ethereum | Documentação oficial em português com módulos progressivos: fundamentos, pilha Ethereum e tópicos avançados. | Português | Iniciante a Avançado | `#ethereum #português #iniciante #intermediário #avançado #desenvolvimento` | [Acesse aqui](https://ethereum.org/pt-br/developers/docs/) |
| Redes de desenvolvimento | Explica ambientes locais e redes próprias para testes em Ethereum. | Português | Iniciante/Intermediário | `#ethereum #português #desenvolvimento #cli #testes` | [Acesse aqui](https://ethereum.org/pt-br/developers/docs/development-networks/) |
| EIPs — Ethereum Improvement Proposals | Repositório oficial de propostas de melhoria da rede; essencial para entender a direção do protocolo. | Inglês | Intermediário/Avançado | `#ethereum #pesquisa #inglês #infra` | [Acesse aqui](https://eips.ethereum.org) |

### 3.3 Solana

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| Solana Quick Start | Guia oficial hands-on para criar o primeiro programa: contas, transações, PDAs e CPIs usando Solana Playground. | Inglês | Iniciante/Intermediário | `#solana #desenvolvimento #quickstart #inglês #rust` | [Acesse aqui](https://solana.com/docs/intro/quick-start) |
| Solana Cookbook | Receitas práticas para operações comuns em Solana: contas, tokens, transações, NFTs e programas. | Inglês | Intermediário | `#solana #desenvolvimento #inglês #intermediário` | [Acesse aqui](https://solanacookbook.com) |
| Blueshift Solana | Trilha em português para fundamentos e desenvolvimento na rede Solana; boa para onboarding inicial. | Português | Iniciante | `#solana #português #iniciante #desenvolvimento` | [Acesse aqui](https://learn.blueshift.gg/pt-BR) |

### 3.4 Stellar

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| Stellar Learn | Hub oficial com conteúdos sobre blockchain basics, smart contracts, stablecoins, wallets, anchors e Stellar Consensus Protocol. | Inglês | Iniciante | `#stellar #fundamentos #inglês #iniciante` | [Acesse aqui](https://stellar.org/learn) |
| Stellar Developer Docs | Documentação oficial para construir aplicações, emitir ativos, escrever smart contracts e configurar validadores. | Inglês | Iniciante a Avançado | `#stellar #desenvolvimento #smart-contracts #infra #inglês` | [Acesse aqui](https://developers.stellar.org) |
| Stellar Quickstart | Ferramenta para rodar a rede Stellar localmente para desenvolvimento e testes. | Inglês | Intermediário | `#stellar #quickstart #desenvolvimento #testes #infra` | [Acesse aqui](https://developers.stellar.org/docs/tools/quickstart) |
| Intro to Stellar | Introdução oficial ao propósito da rede e casos de uso do mundo real. | Inglês | Iniciante | `#stellar #fundamentos #iniciante` | [Acesse aqui](https://stellar.org/learn/intro-to-stellar) |

---

## 4. Cursos em sites

Plataformas com trilhas estruturadas e exercícios práticos para aprender blockchain fazendo. A maioria permite começar sem setup de ambiente, o que acelera o primeiro contato com contratos e transações reais.

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| CryptoZombies | Curso interativo clássico para aprender Solidity criando um jogo; cobre variáveis, herança, padrões e segurança básica. | Português | Iniciante/Intermediário | `#ethereum #solidity #português #iniciante #desenvolvimento #segurança` | [Acesse aqui](https://cryptozombies.io/pt/course) |
| Cyfrin Updraft | Plataforma gratuita com cursos completos de Solidity, Foundry e segurança — curadoria de Patrick Collins. | Inglês | Iniciante a Avançado | `#ethereum #solidity #foundry #segurança #inglês #iniciante #avançado` | [Acesse aqui](https://updraft.cyfrin.io) |
| Ethereum.org Developers Docs | Funciona como trilha estruturada de estudos com módulos progressivos. | Português | Iniciante a Avançado | `#ethereum #português #trilha #desenvolvimento` | [Acesse aqui](https://ethereum.org/pt-br/developers/docs/) |
| Solana Quick Start | Ambiente guiado no navegador; bom para prática imediata sem setup local. | Inglês | Iniciante/Intermediário | `#solana #quickstart #desenvolvimento #rust` | [Acesse aqui](https://solana.com/docs/intro/quick-start) |
| Speedrun Ethereum | Desafios práticos com Solidity e Scaffold-ETH para construir mini-projetos do zero. | Inglês | Intermediário | `#ethereum #solidity #desenvolvimento #intermediário #dapps` | [Acesse aqui](https://speedrunethereum.com) |
| Alchemy University | Cursos gratuitos de Ethereum e Web3 com projetos práticos, criados pela equipe da Alchemy. | Inglês | Iniciante/Intermediário | `#ethereum #desenvolvimento #bootcamp #dapps #inglês` | [Acesse aqui](https://university.alchemy.com) |
| Stellar Learn + Developer Docs | Combinação que cobre fundamentos e prática de construção na rede Stellar. | Inglês | Iniciante/Intermediário | `#stellar #fundamentos #desenvolvimento` | [Acesse aqui](https://stellar.org/learn) |

---

## 5. Cursos em vídeo e bootcamps

Canais e séries em vídeo para quem aprende melhor assistindo. Vídeos envelhecem mais rápido que documentações — verifique sempre a versão dos frameworks antes de replicar o código.

| Recurso | Descrição | Idioma | Nível | Tags | Link |
| ------- | --------- | ------ | ----- | ---- | ---- |
| Patrick Collins — Foundry Full Course | Série completa de desenvolvimento Ethereum com Foundry; referência gratuita mais completa disponível hoje. | Inglês | Iniciante/Intermediário | `#ethereum #solidity #foundry #desenvolvimento #inglês` | [YouTube](https://www.youtube.com/watch?v=umepbfKp5rI) |
| Whiteboard Crypto | Explicações conceituais animadas sobre blockchain, DeFi e criptomoedas. | Inglês | Iniciante | `#fundamentos #defi #inglês #iniciante` | [YouTube](https://www.youtube.com/@WhiteboardCrypto) |
| Finematics | Vídeos sobre arquitetura e funcionamento de protocolos DeFi como Uniswap, Aave e Compound. | Inglês | Intermediário | `#defi #ethereum #inglês #intermediário` | [YouTube](https://www.youtube.com/@Finematics) |
| Solana Foundation — YouTube | Canal oficial com tutoriais, demos de ferramentas e gravações de eventos técnicos. | Inglês | Iniciante a Avançado | `#solana #desenvolvimento #inglês` | [YouTube](https://www.youtube.com/@SolanaFndn) |
| Austin Griffith — Scaffold-ETH | Tutoriais práticos de dapps com foco em prototipagem rápida em Ethereum. | Inglês | Intermediário | `#ethereum #dapps #desenvolvimento #bootcamp` | [YouTube](https://www.youtube.com/@austingriffith3550) |

---

## 6. Artigos, blogs e newsletters

Acompanhar publicações técnicas mantém o conhecimento atual. O ecossistema blockchain muda rápido — novos padrões, propostas de protocolo e vulnerabilidades aparecem constantemente. Os recursos abaixo são bons para leitura recorrente.

- [6.1 Hubs por ecossistema](#61-hubs-por-ecossistema)
- [6.2 Blogs e newsletters técnicas](#62-blogs-e-newsletters-técnicas)

### 6.1 Hubs por ecossistema

| Hub | Motivo para acompanhar | Idioma | Tags | Link |
| --- | ---------------------- | ------ | ---- | ---- |
| Ethereum.org Developers Docs | Reúne explicações atualizadas sobre MEV, rollups, oráculos, bridges e padrões. | Português | `#ethereum #português #artigos #zk #l2` | [Acesse aqui](https://ethereum.org/pt-br/developers/docs/) |
| Stellar Learn | Publica materiais curtos e didáticos sobre casos de uso, stablecoins, anchors e contratos. | Inglês | `#stellar #artigos #fundamentos #payments` | [Acesse aqui](https://stellar.org/learn) |
| Bitcoin Developer Docs | Melhor hub para leitura técnica ligada ao protocolo e APIs. | Inglês | `#bitcoin #artigos #desenvolvimento` | [Acesse aqui](https://developer.bitcoin.org) |
| OpenZeppelin Docs | Fundamental para segurança, padrões, upgrades e boas práticas em contratos EVM. | Inglês | `#ethereum #segurança #smart-contracts #evm` | [Acesse aqui](https://docs.openzeppelin.com) |

### 6.2 Blogs e newsletters técnicas

| Recurso | Descrição | Idioma | Tags | Link |
| ------- | --------- | ------ | ---- | ---- |
| RareSkills Blog | Blog técnico avançado sobre EVM, Solidity, otimização de gas, ZK e segurança. | Inglês | `#ethereum #evm #solidity #zk #segurança #avançado` | [Acesse aqui](https://www.rareskills.io/blog) |
| Bitcoin Optech Newsletter | Newsletter semanal com análise técnica de atualizações, propostas e implementações do Bitcoin. | Inglês | `#bitcoin #newsletter #desenvolvimento #pesquisa` | [Acesse aqui](https://bitcoinops.org) |
| Trail of Bits Blog | Blog da principal empresa de auditoria de segurança do setor; cobre vulnerabilidades, pesquisa e ferramentas. | Inglês | `#segurança #ethereum #pesquisa #avançado` | [Acesse aqui](https://blog.trailofbits.com) |
| Paradigm Research | Pesquisa técnica de ponta sobre DeFi, criptografia, MEV e arquitetura de protocolos. | Inglês | `#pesquisa #defi #ethereum #zk #avançado` | [Acesse aqui](https://www.paradigm.xyz/research) |
| Ethereum Foundation Blog | Atualizações oficiais sobre upgrades, pesquisa e roadmap da rede Ethereum. | Inglês | `#ethereum #pesquisa #infra #newsletter` | [Acesse aqui](https://blog.ethereum.org) |
| Solana Foundation Blog | Atualizações sobre o ecossistema, novos programas e ferramentas da Solana Foundation. | Inglês | `#solana #newsletter #desenvolvimento` | [Acesse aqui](https://solana.com/news) |

---

## 7. Whitepapers fundamentais

Os whitepapers são os documentos que definiram as ideias centrais de cada rede. Lê-los é a diferença entre entender o "o que" e o "por que" de cada protocolo. Os mais técnicos (Yellow Paper, SCP) exigem base matemática ou podem ser abordados com suporte de material explicativo.

| Rede | Recurso | Motivo | Idioma | Nível | Tags | Link |
| ---- | ------- | ------ | ------ | ----- | ---- | ---- |
| Bitcoin | _Bitcoin: A Peer-to-Peer Electronic Cash System_ | Documento fundador do setor; base para consenso, política monetária e arquitetura peer-to-peer. | Inglês | Intermediário | `#bitcoin #whitepaper #fundamentos` | [bitcoin.org](https://bitcoin.org/bitcoin.pdf) |
| Ethereum | _Ethereum Whitepaper_ | Introduz a visão de uma blockchain programável e o conceito de contratos inteligentes generalizados. | Inglês | Intermediário | `#ethereum #whitepaper #smart-contracts` | [ethereum.org](https://ethereum.org/pt-br/whitepaper/) |
| Ethereum | _Yellow Paper_ | Especificação técnica formal da EVM e detalhes de execução. | Inglês | Avançado | `#ethereum #evm #avançado #whitepaper` | [GitHub](https://github.com/ethereum/yellowpaper) |
| Stellar | _Stellar Consensus Protocol (SCP)_ | Fundamental para entender o modelo de consenso federado da rede Stellar. | Inglês | Avançado | `#stellar #consenso #whitepaper #avançado` | [stellar.org](https://www.stellar.org/papers/stellar-consensus-protocol) |
| Solana | _Solana Whitepaper / Proof of History_ | Explica o argumento de desempenho e a noção de relógio criptográfico da rede. | Inglês | Intermediário/Avançado | `#solana #whitepaper #consenso` | [solana.com](https://solana.com/solana-whitepaper.pdf) |

---

## 8. Ferramentas de desenvolvimento e segurança

Ferramentas certas aceleram o aprendizado prático. Esta seção cobre o tooling padrão de cada ecossistema: ambientes de desenvolvimento, frameworks de teste, CLIs, exploradores de bloco e ferramentas de segurança.

- [8.1 Ferramentas EVM](#81-ferramentas-evm)
- [8.2 Ferramentas Bitcoin](#82-ferramentas-bitcoin)
- [8.3 Ferramentas Solana](#83-ferramentas-solana)
- [8.4 Ferramentas Stellar](#84-ferramentas-stellar)
- [8.5 Segurança](#85-segurança)

### 8.1 Ferramentas EVM

| Ferramenta | Função | Tags | Link |
| ---------- | ------ | ---- | ---- |
| OpenZeppelin Contracts | Biblioteca de contratos auditados e padronizados para ERCs e componentes reutilizáveis. | `#ethereum #evm #segurança #smart-contracts` | [Acesse aqui](https://docs.openzeppelin.com/contracts) |
| OpenZeppelin Upgrades Plugins | Plugins para Hardhat e Foundry com verificações de segurança para proxies e upgrades. | `#ethereum #upgrades #segurança #hardhat #foundry` | [Acesse aqui](https://docs.openzeppelin.com) |
| Foundry | Toolkit em Rust para Ethereum: forge (testes e fuzzing), cast (CLI) e anvil (node local). | `#ethereum #foundry #desenvolvimento #testes #cli` | [Acesse aqui](https://book.getfoundry.sh/) |
| Hardhat | Framework amplamente usado para compilar, testar e fazer deploy em EVM. | `#ethereum #hardhat #desenvolvimento #cli` | [Acesse aqui](https://hardhat.org/) |
| Remix IDE | IDE web ideal para primeiros contratos e experimentos em Solidity. | `#ethereum #solidity #iniciante #ide` | [Acesse aqui](https://remix.ethereum.org/) |
| Tenderly | Plataforma para observar, depurar e monitorar contratos e transações em mainnet e testnets. | `#ethereum #debug #monitoring #devtools` | [Acesse aqui](https://tenderly.co/) |
| Etherscan | Explorador de blocos da rede Ethereum; essencial para inspecionar transações, contratos e eventos. | `#ethereum #debug #api #evm` | [Acesse aqui](https://etherscan.io) |

### 8.2 Ferramentas Bitcoin

| Ferramenta | Função | Tags | Link |
| ---------- | ------ | ---- | ---- |
| Bitcoin Core | Cliente de referência para operar nó, testar e entender a rede. | `#bitcoin #node #infra #cli` | [Acesse aqui](https://bitcoincore.org/) |
| Bitcoin Developer Docs | Referência técnica para APIs, conceitos e integração com aplicações. | `#bitcoin #desenvolvimento #api` | [Acesse aqui](https://developer.bitcoin.org/) |
| Mempool.space | Explorador de blocos e mempool com visualizações de transações e taxas em tempo real. | `#bitcoin #debug #monitoring` | [Acesse aqui](https://mempool.space) |

### 8.3 Ferramentas Solana

| Ferramenta | Função | Tags | Link |
| ---------- | ------ | ---- | ---- |
| Solana Playground | Ambiente no navegador para começar sem setup; usado no quickstart oficial. | `#solana #iniciante #playground #desenvolvimento` | [Acesse aqui](https://beta.solpg.io/) |
| Solana CLI | Ferramenta essencial para contas, deploys, airdrops e interação com clusters. | `#solana #cli #desenvolvimento` | [Acesse aqui](https://solana.com/docs/intro/installation) |
| Anchor | Framework amplamente usado para smart contracts/programs em Solana. | `#solana #anchor #rust #desenvolvimento` | [Acesse aqui](https://www.anchor-lang.com/) |
| Solana Explorer | Explorador oficial de blocos e transações da rede Solana. | `#solana #debug #monitoring` | [Acesse aqui](https://explorer.solana.com) |

### 8.4 Ferramentas Stellar

| Ferramenta | Função | Tags | Link |
| ---------- | ------ | ---- | ---- |
| Stellar Quickstart | Ambiente local com Stellar Core, Horizon, RPC e demais serviços para testes. | `#stellar #quickstart #infra #testes` | [Acesse aqui](https://developers.stellar.org/docs/tools/quickstart) |
| Stellar SDKs | SDKs oficiais para JavaScript, Python, Go, Java e outras linguagens. | `#stellar #sdk #desenvolvimento` | [Acesse aqui](https://developers.stellar.org) |
| Soroban CLI | Ferramenta central para o ciclo de desenvolvimento de contratos na stack Stellar/Soroban. | `#stellar #soroban #cli #smart-contracts` | [Acesse aqui](https://developers.stellar.org/docs/tools/soroban-cli) |
| Stellar Expert | Explorador de blocos e analytics para a rede Stellar. | `#stellar #debug #monitoring` | [Acesse aqui](https://stellar.expert) |

### 8.5 Segurança

Ferramentas de análise estática, fuzzing e prática de segurança ofensiva/defensiva em contratos inteligentes.

| Ferramenta | Função | Tags | Link |
| ---------- | ------ | ---- | ---- |
| Slither | Analisador estático de Solidity; detecta vulnerabilidades comuns automaticamente. | `#ethereum #segurança #solidity #testes` | [Acesse aqui](https://github.com/crytic/slither) |
| Echidna | Fuzzer para contratos Solidity; encontra bugs por geração de inputs aleatórios. | `#ethereum #segurança #testes #avançado` | [Acesse aqui](https://github.com/crytic/echidna) |
| Ethernaut | Jogo de segurança com desafios práticos de exploit em contratos reais. | `#ethereum #segurança #iniciante #smart-contracts` | [Acesse aqui](https://ethernaut.openzeppelin.com) |
| Damn Vulnerable DeFi | Desafios de segurança baseados em cenários reais de ataques em DeFi. | `#ethereum #defi #segurança #avançado` | [Acesse aqui](https://www.damnvulnerabledefi.xyz) |
| Immunefi | Plataforma de bug bounty para protocolos blockchain; referência de vulnerabilidades reais reportadas. | `#segurança #ethereum #pesquisa` | [Acesse aqui](https://immunefi.com) |

---

## 9. Comunidades e ecossistemas

Participar de comunidades ativas acelera o aprendizado por exposição a problemas reais e feedback de pessoas experientes. O mais valioso no médio prazo costuma ser acompanhar GitHub, issues, fóruns e mailing lists das redes — onde as decisões de protocolo são discutidas antes de chegarem à documentação.

- [9.1 Comunidades por rede](#91-comunidades-por-rede)
- [9.2 Fóruns e discussões técnicas](#92-fóruns-e-discussões-técnicas)

### 9.1 Comunidades por rede

| Rede | Comunidade / Ecossistema | Motivo | Tags | Link |
| ---- | ------------------------ | ------ | ---- | ---- |
| Bitcoin | bitcoin-dev mailing list e Bitcoin Core | Melhor para discussões técnicas e contribuições ao protocolo. | `#bitcoin #comunidade #core #desenvolvimento` | [Acesse aqui](https://bitcoin.org/en/development) |
| Bitcoin | Bitcoin StackExchange | Base de Q&A técnico com histórico de discussões. | `#bitcoin #fórum #comunidade` | [Acesse aqui](https://bitcoin.stackexchange.com/) |
| Ethereum | Ethereum.org developers portal | Centraliza entrada para ferramentas, docs e tutoriais. | `#ethereum #comunidade #desenvolvimento` | [Acesse aqui](https://ethereum.org/pt-br/developers/) |
| Ethereum | Ethereum Magicians | Fórum onde EIPs e mudanças de protocolo são discutidos. | `#ethereum #pesquisa #infra #comunidade` | [Acesse aqui](https://ethereum-magicians.org) |
| Solana | Solana Stack Exchange | Plataforma de Q&A técnico do ecossistema Solana. | `#solana #comunidade #desenvolvimento #fórum` | [Acesse aqui](https://solana.stackexchange.com) |
| Stellar | Stellar Developer Docs e Stellar Learn | Reúnem documentação, educação e caminhos para contribuição. | `#stellar #comunidade #desenvolvimento` | [Acesse aqui](https://developers.stellar.org) |
| OpenZeppelin | Fórum da comunidade OpenZeppelin | Essencial para segurança, padrões e contratos EVM. | `#ethereum #segurança #comunidade` | [Acesse aqui](https://forum.openzeppelin.com) |

### 9.2 Fóruns e discussões técnicas

| Recurso | Descrição | Tags | Link |
| ------- | --------- | ---- | ---- |
| Ethereum Research | Fórum técnico da Ethereum Foundation para pesquisa de consenso, criptografia e escalabilidade. | `#ethereum #pesquisa #zk #l2 #consenso` | [Acesse aqui](https://ethresear.ch) |
| Bitcoin StackExchange | Arquivo de perguntas e respostas técnicas sobre Bitcoin, com respostas de contribuidores experientes. | `#bitcoin #fórum #desenvolvimento` | [Acesse aqui](https://bitcoin.stackexchange.com) |
| Ethereum StackExchange | Equivalente para o ecossistema Ethereum. | `#ethereum #fórum #desenvolvimento` | [Acesse aqui](https://ethereum.stackexchange.com) |

---

## 10. IA para desenvolvimento blockchain

Ferramentas de IA aceleram onboarding, explicam conceitos, geram testes e ajudam na leitura de documentação técnica. Em blockchain, o melhor uso é como copiloto técnico — não substitui auditoria nem validação manual contra documentação oficial e ambiente de testnet.

- [10.1 Onde IA ajuda de verdade](#101-onde-ia-ajuda-de-verdade)
- [10.2 Ferramentas e materiais](#102-ferramentas-e-materiais)
- [10.3 Prompts úteis](#103-prompts-úteis)
- [10.4 Skills para alunos](#104-skills-para-alunos)

### 10.1 Onde IA ajuda de verdade

IA ajuda bastante em: explicação de conceitos em camadas (simples → técnica → produção), geração de testes, scaffolding de projetos, tradução de docs complexas, revisão inicial de contratos e transformação de código entre frameworks. Não substitui auditoria profissional nem validação em ambiente real.

### 10.2 Ferramentas e materiais

| Recurso | Descrição | Idioma | Tags | Link |
| ------- | --------- | ------ | ---- | ---- |
| OpenZeppelin Contracts MCP | Recurso da OpenZeppelin para escrever contratos seguros com assistência de IA seguindo seus padrões. | Inglês | `#ia #ethereum #segurança #smart-contracts` | [Acesse aqui](https://docs.openzeppelin.com) |
| Documentações oficiais das redes | Base para grounding ao usar IA na geração de código. | Português/Inglês | `#ia #documentação` | [Acesse aqui](https://ethereum.org/pt-br/developers/docs/) |
| Repositórios de referência no GitHub | Alimentar prompts com contexto real de arquitetura, testes e padrões. | Inglês | `#ia #github #boas-práticas` | [GitHub Ethereum](https://github.com/ethereum) |

### 10.3 Prompts úteis

**Prompt 1 — Explicação beginner friendly**

```text
Explique o conceito de [tema] em blockchain como se a pessoa soubesse programação básica, mas nunca tivesse visto Web3. Use analogias simples, depois conecte com a implementação real em [Bitcoin/Ethereum/Solana/Stellar].
```

**Prompt 2 — Leitura guiada de documentação**

```text
Resuma esta página de documentação em português claro. Separe em: o que é, quando usar, pré-requisitos, passos práticos, erros comuns e dicionário mínimo.
```

**Prompt 3 — Geração de exercício**

```text
Crie 3 exercícios progressivos sobre [tema], um iniciante, um intermediário e um avançado, com objetivo, passos esperados, dicas e critérios de correção.
```

**Prompt 4 — Segurança de contratos**

```text
Revise este contrato inteligente com foco em: controle de acesso, validação de inputs, reentrância, pausabilidade, upgrades, eventos, testes necessários e riscos de produção. Não assuma que o código está correto.
```

**Prompt 5 — Pair programming blockchain**

```text
Atue como pair programmer para construir um projeto em [rede]. Primeiro proponha a arquitetura, depois gere estrutura de pastas, dependências, contratos/programas, testes, scripts de deploy e checklist de segurança. Explique cada decisão.
```

### 10.4 Skills para alunos

**Saber usar IA em blockchain:**

- Pedir explicação em camadas: visão simples → visão técnica → visão de produção.
- Colar contexto suficiente: versão da linguagem, framework, rede, objetivo e erro encontrado.
- Pedir testes antes de pedir deploy.
- Pedir análise de ameaça, não apenas "corrija o código".
- Validar toda resposta contra docs oficiais e ambiente local/testnet.
- Informar stack exata: Solidity/Foundry, Solidity/Hardhat, Rust/Anchor, Soroban, Bitcoin Core.
- Solicitar referências para a doc oficial correspondente.

---

## 11. Trilha de aprendizagem

Caminhos recomendados baseados em objetivo e nível atual. Cada caminho cita materiais diretos listados nas seções anteriores. Escolha o perfil que melhor descreve seu ponto de partida e objetivo.

- [11.1 Quero entender a tecnologia](#111-quero-entender-a-tecnologia)
- [11.2 Desenvolvimento Ethereum / EVM](#112-desenvolvimento-ethereum--evm)
- [11.3 Desenvolvimento Solana](#113-desenvolvimento-solana)
- [11.4 Desenvolvimento Stellar](#114-desenvolvimento-stellar)
- [11.5 Bitcoin — protocolo e integração](#115-bitcoin--protocolo-e-integração)
- [11.6 Segurança de contratos](#116-segurança-de-contratos)

---

### 11.1 Quero entender a tecnologia

**Perfil:** sem foco em desenvolvimento; quer entender como blockchain funciona, seus casos de uso e por que importa.

```
[1] Ethereum Docs (PT)       → como blockchain funciona: contas, transações, carteiras
     ethereum.org/pt-br/developers/docs/

[2] Bitcoin Whitepaper       → a lógica original do consenso descentralizado (9 páginas)
     bitcoin.org/bitcoin.pdf

[3] Stellar Learn             → casos de uso reais: pagamentos, stablecoins, inclusão financeira
     stellar.org/learn

[4] Whiteboard Crypto        → vídeos animados sobre DeFi, NFTs e como as redes funcionam
     youtube.com/@WhiteboardCrypto

[5] Finematics               → arquitetura de protocolos DeFi em vídeo (Uniswap, Aave, etc.)
     youtube.com/@Finematics
```

---

### 11.2 Desenvolvimento Ethereum / EVM

**Perfil:** quer desenvolver contratos inteligentes em Solidity e construir aplicações em Ethereum ou redes EVM-compatíveis.

```
INICIANTE
─────────────────────────────────────────────────────────────────
  [1] Ethereum Docs (PT)          → fundamentos: EVM, gas, contas, ciclo de vida de tx
       ethereum.org/pt-br/developers/docs/

  [2] CryptoZombies (PT)          → Solidity na prática criando um jogo
       cryptozombies.io/pt/course

  [3] Remix IDE                   → primeiros deploys em testnet no navegador
       remix.ethereum.org

INTERMEDIÁRIO
─────────────────────────────────────────────────────────────────
  [4] Cyfrin Updraft              → curso completo gratuito de Solidity + Foundry
       updraft.cyfrin.io

  [5] Foundry                     → testes, scripts e deploy com a stack mais rápida do ecossistema
       book.getfoundry.sh

  [6] OpenZeppelin Contracts      → padrões auditados: ERC-20, ERC-721, controle de acesso
       docs.openzeppelin.com/contracts

  [7] Speedrun Ethereum           → desafios práticos com Scaffold-ETH
       speedrunethereum.com

AVANÇADO
─────────────────────────────────────────────────────────────────
  [8] Mastering Ethereum          → arquitetura EVM, oráculos, padrões e segurança em profundidade
       github.com/ethereumbook/ethereumbook

  [9] Ethernaut                   → desafios de segurança: aprenda como contratos são explorados
       ethernaut.openzeppelin.com

 [10] Damn Vulnerable DeFi        → cenários reais de ataques em protocolos DeFi
       damnvulnerabledefi.xyz

 [11] Ethereum Yellow Paper       → especificação técnica formal da EVM
       github.com/ethereum/yellowpaper

 [12] RareSkills Blog             → otimização de gas, EVM internals, ZK
       rareskills.io/blog
```

---

### 11.3 Desenvolvimento Solana

**Perfil:** quer desenvolver programas em Rust/Anchor e construir aplicações na rede Solana.

```
INICIANTE
─────────────────────────────────────────────────────────────────
  [1] Blueshift Solana (PT)       → fundamentos da rede em português
       learn.blueshift.gg/pt-BR

  [2] Solana Quick Start          → primeiro programa no Solana Playground (sem setup local)
       solana.com/docs/intro/quick-start

  [3] Solana Playground           → ambiente no navegador para experimentar
       beta.solpg.io

INTERMEDIÁRIO
─────────────────────────────────────────────────────────────────
  [4] Anchor                      → framework padrão para programas Solana em Rust
       anchor-lang.com

  [5] Solana Cookbook             → receitas práticas: tokens, NFTs, contas, PDAs, CPIs
       solanacookbook.com

  [6] Solana CLI                  → deploys, airdrops e interação com clusters
       solana.com/docs/intro/installation

AVANÇADO
─────────────────────────────────────────────────────────────────
  [7] Solana Foundation YouTube   → tutoriais avançados e atualizações do ecossistema
       youtube.com/@SolanaFndn

  [8] Solana Whitepaper           → Proof of History e arquitetura da rede
       solana.com/solana-whitepaper.pdf
```

---

### 11.4 Desenvolvimento Stellar

**Perfil:** quer construir aplicações de pagamento, emitir ativos ou desenvolver smart contracts com Soroban.

```
INICIANTE
─────────────────────────────────────────────────────────────────
  [1] Intro to Stellar            → propósito da rede e casos de uso
       stellar.org/learn/intro-to-stellar

  [2] Stellar Learn               → blockchain basics, stablecoins, wallets, anchors
       stellar.org/learn

  [3] Stellar Developer Docs      → ponto de entrada para desenvolvimento
       developers.stellar.org

INTERMEDIÁRIO
─────────────────────────────────────────────────────────────────
  [4] Stellar Quickstart          → rede local para desenvolvimento e testes
       developers.stellar.org/docs/tools/quickstart

  [5] Soroban CLI                 → ciclo de desenvolvimento de smart contracts Soroban
       developers.stellar.org/docs/tools/soroban-cli

  [6] Stellar SDKs                → integre aplicações com a rede (JS, Python, Go, Java)
       developers.stellar.org

AVANÇADO
─────────────────────────────────────────────────────────────────
  [7] SCP Whitepaper              → modelo de consenso federado da rede
       stellar.org/papers/stellar-consensus-protocol
```

---

### 11.5 Bitcoin — protocolo e integração

**Perfil:** quer entender o protocolo Bitcoin em profundidade ou integrar aplicações com a rede.

```
INICIANTE
─────────────────────────────────────────────────────────────────
  [1] Learn me a Bitcoin          → como o Bitcoin funciona internamente (visual e progressivo)
       learnmeabitcoin.com

  [2] Bitcoin Whitepaper          → o documento original de Satoshi (9 páginas)
       bitcoin.org/bitcoin.pdf

INTERMEDIÁRIO
─────────────────────────────────────────────────────────────────
  [3] Bitcoin Developer Reference → transações, scripts, RPC e APIs
       developer.bitcoin.org/reference/intro.html

  [4] Mastering Bitcoin           → fundo técnico completo da rede
       github.com/bitcoinbook/bitcoinbook

  [5] Programming Bitcoin         → criptografia aplicada e implementação em código
       oreilly.com/library/view/programming-bitcoin/9781492031482/

AVANÇADO
─────────────────────────────────────────────────────────────────
  [6] Bitcoin Optech Newsletter   → análise semanal de atualizações e propostas (BIPs)
       bitcoinops.org

  [7] Bitcoin Core + bitcoin-dev  → contribuição ao protocolo e discussões técnicas
       bitcoin.org/en/development
```

---

### 11.6 Segurança de contratos

**Perfil:** quer aprender segurança de contratos inteligentes — para auditar, desenvolver com mais cuidado ou participar de bug bounty.

```
PRÉ-REQUISITO
─────────────────────────────────────────────────────────────────
  → Siga o caminho 11.2 até o nível INTERMEDIÁRIO antes de continuar

INICIANTE EM SEGURANÇA
─────────────────────────────────────────────────────────────────
  [1] OpenZeppelin Contracts      → use bibliotecas auditadas como referência de padrão
       docs.openzeppelin.com/contracts

  [2] Ethernaut                   → aprenda explorando contratos vulneráveis
       ethernaut.openzeppelin.com

INTERMEDIÁRIO
─────────────────────────────────────────────────────────────────
  [3] Damn Vulnerable DeFi        → ataques reais em cenários de DeFi
       damnvulnerabledefi.xyz

  [4] Slither                     → análise estática de contratos Solidity
       github.com/crytic/slither

  [5] Cyfrin Updraft — Security   → módulo de segurança do curso de Foundry
       updraft.cyfrin.io

AVANÇADO
─────────────────────────────────────────────────────────────────
  [6] Echidna                     → fuzzing de contratos Solidity
       github.com/crytic/echidna

  [7] Trail of Bits Blog          → pesquisa e vulnerabilidades descobertas em auditorias reais
       blog.trailofbits.com

  [8] Smart Contract Security Field Guide  → referência técnica de segurança
       scsfg.io

  [9] Immunefi                    → plataforma de bug bounty; referência de vulnerabilidades reais
       immunefi.com
```

---
