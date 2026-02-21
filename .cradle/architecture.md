# Architecture

## Dependency Graph

```mermaid
graph TD
  4accaf4a["Erc20-stylus (erc20-stylus)"]
  15f54cfe["Erc721-stylus (erc721-stylus)"]
  9e7924e0["Erc1155-stylus (erc1155-stylus)"]
  34140e81["Robinhood-network (robinhood-network)"]
  0893ddc4["Auditware-analyzing (auditware-analyzing)"]
  f3d0d92d["Robinhood-contracts (robinhood-contracts)"]
  f41c86f5["Frontend-scaffold (frontend-scaffold)"]
  f3399a44["Robinhood-deployment (robinhood-deployment)"]
  f5b1a79a["Openclaw-agent (openclaw-agent)"]
  7fc516d0["Wallet-auth (wallet-auth)"]
  d81dacd9["Dune-transaction-history (dune-transaction-history)"]
  f41c86f5 --> f5b1a79a
  4accaf4a --> 0893ddc4
  15f54cfe --> 0893ddc4
  9e7924e0 --> 0893ddc4
  4accaf4a --> f41c86f5
  15f54cfe --> f41c86f5
  9e7924e0 --> f41c86f5
  34140e81 --> f41c86f5
  f3d0d92d --> f41c86f5
  34140e81 --> f3d0d92d
  f3d0d92d --> f3399a44
  f41c86f5 --> 7fc516d0
  f41c86f5 --> d81dacd9
```

## Execution / Implementation Order

1. **Erc20-stylus** (`4accaf4a`)
2. **Erc721-stylus** (`15f54cfe`)
3. **Erc1155-stylus** (`9e7924e0`)
4. **Robinhood-network** (`34140e81`)
5. **Auditware-analyzing** (`0893ddc4`)
6. **Robinhood-contracts** (`f3d0d92d`)
7. **Frontend-scaffold** (`f41c86f5`)
8. **Robinhood-deployment** (`f3399a44`)
9. **Openclaw-agent** (`f5b1a79a`)
10. **Wallet-auth** (`7fc516d0`)
11. **Dune-transaction-history** (`d81dacd9`)
