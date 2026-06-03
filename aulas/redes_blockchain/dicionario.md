<p align="center">
    <img src="../../others/assets/banner_blockas.png" alt="Banner Blockas">
</p>

# Dicionário de Redes Blockchain e Arquiteturas

Este dicionário reúne os principais termos técnicos, conceitos de consenso e arquiteturas abordados no estudo comparativo de redes. Cada termo acompanha uma definição clara e um link para material de aprofundamento.

Para voltar ao material principal [clique aqui](./material_didatico_redes_blockchain.md)

**Índice Remissivo:**
[ A ](#a) | [ E ](#e) | [ H ](#h) | [ M ](#m) | [ P ](#p) | [ R ](#r) | [ S ](#s) | [ U ](#u) | [ W ](#w)

---

### A

**Abstração de Conta (Account Abstraction)**
Uma evolução na arquitetura de contas da blockchain (especialmente no Ethereum via ERC-4337) que permite que as carteiras dos usuários funcionem como contratos inteligentes, possibilitando recuperação social, pagamento de taxas por terceiros e maior facilidade de uso.

- [Aprofunde-se em Account Abstraction](https://ethereum.org/pt-br/roadmap/account-abstraction/)

### E

**EVM (Ethereum Virtual Machine)**
A máquina de estado global do Ethereum. É o ambiente de execução onde todos os contratos inteligentes e regras da rede são computados e processados.

- [Aprofunde-se na EVM](https://ethereum.org/pt-br/developers/docs/evm/)

### H

**Halving**
Evento programado no protocolo do Bitcoin que reduz pela metade a recompensa (subsídio de bloco) concedida aos mineradores. Ocorre a cada 210.000 blocos (aprox. 4 anos) e garante a deflação e escassez do ativo.

- [Aprofunde-se sobre o Halving](https://www.investopedia.com/bitcoin-halving-4843769)

**HTLCs (Hash Timelock Contracts)**
Contratos inteligentes baseados em travas de tempo e de hash. São essenciais para o funcionamento da Lightning Network, permitindo que pagamentos sejam roteados de forma segura entre vários usuários sem risco de roubo.

- [Aprofunde-se em HTLCs](https://en.bitcoin.it/wiki/Hash_Time_Locked_Contracts)

### M

**Mempool (Memory Pool)**
A "sala de espera" de uma rede blockchain. É o local onde as transações não confirmadas ficam armazenadas pelos nós da rede até que um minerador ou validador as selecione para serem incluídas no próximo bloco. Redes como a Solana (via Gulf Stream) dispensam o uso do mempool tradicional.

- [Aprofunde-se no Mempool](https://www.investopedia.com/terms/m/mempool.asp)

### P

**PoH (Proof of History)**
Mecanismo criptográfico introduzido pela Solana que atua como um relógio descentralizado. Ele cria um registro histórico sequencial (carimbo de tempo) que prova que um evento ocorreu em um momento específico, permitindo altíssima velocidade de rede.

- [Aprofunde-se no Proof of History](https://solana.com/news/proof-of-history)

**PoS (Proof of Stake)**
Mecanismo de consenso onde os validadores da rede bloqueiam uma quantia financeira de tokens (*staking*) como garantia de honestidade para criar novos blocos, dispensando o gasto energético massivo da mineração.

- [Aprofunde-se no Proof of Stake](https://ethereum.org/pt-br/developers/docs/consensus-mechanisms/pos/)

**PoW (Proof of Work)**
O mecanismo de consenso original do Bitcoin. Exige que os mineradores compitam para resolver problemas matemáticos complexos gastando energia computacional para validar blocos e proteger a rede contra ataques.

- [Aprofunde-se no Proof of Work](https://ethereum.org/pt-br/developers/docs/consensus-mechanisms/pow/)

### R

**Rollups (Layer-2)**
Soluções de escalabilidade que executam milhares de transações fora da camada principal (Layer-1) e agrupam (rolam) os dados resultantes em uma única prova criptográfica enviada de volta à rede principal, barateando os custos drasticamente.

- [Aprofunde-se em Rollups](https://ethereum.org/pt-br/developers/docs/scaling/rollups/)

### S

**SCP (Stellar Consensus Protocol)**
O algoritmo de consenso da rede Stellar. Baseado no Acordo Bizantino Federado, não exige mineração ou staking. O consenso é alcançado rapidamente através de círculos de confiança sobrepostos (*Quorum Slices*) entre os validadores.

- [Aprofunde-se no SCP](https://stellar.org/learn/stellar-consensus-protocol)

**State Bloat (Inchaço de Estado)**
O problema de crescimento insustentável do tamanho do histórico de dados que os nós de uma blockchain precisam armazenar para manter a rede funcionando. Redes como a Stellar/Soroban utilizam exclusão de estados inativos para combater isso.

- [Aprofunde-se no State Bloat](https://www.coindesk.com/tech/2021/02/10/what-is-state-bloat-a-guide-to-ethereums-hidden-crisis/)

### U

**UTXO (Unspent Transaction Output)**
O modelo de contabilidade utilizado pelo Bitcoin. Nele, não existem "saldos de conta". O saldo de um usuário é simplesmente a soma de todas as saídas de transações passadas que ele recebeu e que ainda não gastou (como moedas físicas de diferentes valores na carteira).

- [Aprofunde-se no Modelo UTXO](https://academy.binance.com/pt/articles/utxo-model-explained)

### W

**Wasm (WebAssembly)**
Um formato de instrução binária projetado como um alvo de compilação portátil de alto desempenho. Na Web3, permite que contratos inteligentes sejam escritos em linguagens tradicionais poderosas, como Rust, e executados com velocidade quase nativa em blockchains como a Soroban/Stellar.

- [Aprofunde-se no WebAssembly](https://webassembly.org/)