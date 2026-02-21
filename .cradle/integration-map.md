# Integration Map

How components connect and what data flows between them.

### Frontend-scaffold --> Openclaw-agent

- **Source**: Frontend-scaffold (`f41c86f5`)
  - Output ports: App Context (config)
- **Target**: Openclaw-agent (`f5b1a79a`)
  - Input ports: Agent Prompt (config)

### Erc20-stylus --> Auditware-analyzing

- **Source**: Erc20-stylus (`4accaf4a`)
  - Output ports: Token Contract (contract)
- **Target**: Auditware-analyzing (`0893ddc4`)
  - Input ports: Contract Input (contract)

### Erc721-stylus --> Auditware-analyzing

- **Source**: Erc721-stylus (`15f54cfe`)
  - Output ports: NFT Contract (contract)
- **Target**: Auditware-analyzing (`0893ddc4`)
  - Input ports: Contract Input (contract)

### Erc1155-stylus --> Auditware-analyzing

- **Source**: Erc1155-stylus (`9e7924e0`)
  - Output ports: Multi-Token Contract (contract)
- **Target**: Auditware-analyzing (`0893ddc4`)
  - Input ports: Contract Input (contract)

### Erc20-stylus --> Frontend-scaffold

- **Source**: Erc20-stylus (`4accaf4a`)
  - Output ports: Token Contract (contract)
- **Target**: Frontend-scaffold (`f41c86f5`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Erc721-stylus --> Frontend-scaffold

- **Source**: Erc721-stylus (`15f54cfe`)
  - Output ports: NFT Contract (contract)
- **Target**: Frontend-scaffold (`f41c86f5`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Erc1155-stylus --> Frontend-scaffold

- **Source**: Erc1155-stylus (`9e7924e0`)
  - Output ports: Multi-Token Contract (contract)
- **Target**: Frontend-scaffold (`f41c86f5`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Robinhood-network --> Frontend-scaffold

- **Source**: Robinhood-network (`34140e81`)
  - Output ports: Chain Config (config), Contract Constants (config)
- **Target**: Frontend-scaffold (`f41c86f5`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Robinhood-contracts --> Frontend-scaffold

- **Source**: Robinhood-contracts (`f3d0d92d`)
  - Output ports: Contract Constants (config), Types (types)
- **Target**: Frontend-scaffold (`f41c86f5`)
  - Input ports: Contract ABI (contract), Network Config (config)

### Robinhood-network --> Robinhood-contracts

- **Source**: Robinhood-network (`34140e81`)
  - Output ports: Chain Config (config), Contract Constants (config)
- **Target**: Robinhood-contracts (`f3d0d92d`)
  

### Robinhood-contracts --> Robinhood-deployment

- **Source**: Robinhood-contracts (`f3d0d92d`)
  - Output ports: Contract Constants (config), Types (types)
- **Target**: Robinhood-deployment (`f3399a44`)
  

### Frontend-scaffold --> Wallet-auth

- **Source**: Frontend-scaffold (`f41c86f5`)
  - Output ports: App Context (config)
- **Target**: Wallet-auth (`7fc516d0`)
  

### Frontend-scaffold --> Dune-transaction-history

- **Source**: Frontend-scaffold (`f41c86f5`)
  - Output ports: App Context (config)
- **Target**: Dune-transaction-history (`d81dacd9`)
  
