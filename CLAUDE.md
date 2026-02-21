# My Dapp

> A Web3 application - composed with [N]skills

**Network**: Arbitrum Sepolia (Chain ID: 421614) — Testnet
**Keywords**: web3, dapp

---

## Architecture

```mermaid
graph TD
  4accaf4a["ERC-20 Token"]
  15f54cfe["ERC-721 NFT"]
  9e7924e0["ERC-1155 Multi-Token"]
  34140e81["Network Config"]
  0893ddc4["Auditware Analyzer"]
  f3d0d92d["Contract Addresses"]
  f41c86f5["Frontend"]
  f3399a44["Deployment Guide"]
  f5b1a79a["OpenClaw"]
  7fc516d0["Wallet Auth"]
  d81dacd9["Transaction History"]
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

## Components

| Component | Type | Category | User Prompt |
|-----------|------|----------|-------------|
| ERC-20 Token | `erc20-stylus` | contracts | (none) |
| ERC-721 NFT | `erc721-stylus` | contracts | (none) |
| ERC-1155 Multi-Token | `erc1155-stylus` | contracts | (none) |
| Network Config | `robinhood-network` | robinhood | (none) |
| Auditware Analyzer | `auditware-analyzing` | contracts | (none) |
| Contract Addresses | `robinhood-contracts` | robinhood | (none) |
| Frontend | `frontend-scaffold` | app | (none) |
| Deployment Guide | `robinhood-deployment` | robinhood | (none) |
| OpenClaw | `openclaw-agent` | agents | (none) |
| Wallet Auth | `wallet-auth` | app | (none) |
| Transaction History | `dune-transaction-history` | analytics | (none) |

## Implementation Order

Build the project in this order (respects dependencies):

1. **ERC-20 Token** (`erc20-stylus`) — see `.cradle/components/erc20-stylus--4accaf4a.md`
2. **ERC-721 NFT** (`erc721-stylus`) — see `.cradle/components/erc721-stylus--15f54cfe.md`
3. **ERC-1155 Multi-Token** (`erc1155-stylus`) — see `.cradle/components/erc1155-stylus--9e7924e0.md`
4. **Network Config** (`robinhood-network`) — see `.cradle/components/robinhood-network--34140e81.md`
5. **Auditware Analyzer** (`auditware-analyzing`) — see `.cradle/components/auditware-analyzing--0893ddc4.md`
6. **Contract Addresses** (`robinhood-contracts`) — see `.cradle/components/robinhood-contracts--f3d0d92d.md`
7. **Frontend** (`frontend-scaffold`) — see `.cradle/components/frontend-scaffold--f41c86f5.md`
8. **Deployment Guide** (`robinhood-deployment`) — see `.cradle/components/robinhood-deployment--f3399a44.md`
9. **OpenClaw** (`openclaw-agent`) — see `.cradle/components/openclaw-agent--f5b1a79a.md`
10. **Wallet Auth** (`wallet-auth`) — see `.cradle/components/wallet-auth--7fc516d0.md`
11. **Transaction History** (`dune-transaction-history`) — see `.cradle/components/dune-transaction-history--d81dacd9.md`

## Environment Variables

| Key | Description | Required | Default |
|-----|-------------|----------|---------|
| `NEXT_PUBLIC_TOKEN_ADDRESS` | Deployed ERC20 token address | No |  |
| `PRIVATE_KEY` | Private key for deployment and transactions | Yes |  |
| `ERC20_DEPLOYMENT_API_URL` | URL of the ERC20 deployment API | No | http://localhost:4000 |
| `NEXT_PUBLIC_NFT_ADDRESS` | Deployed ERC721 NFT address | No |  |
| `ERC721_DEPLOYMENT_API_URL` | URL of the ERC721 deployment API | No | http://localhost:4001 |
| `NEXT_PUBLIC_ERC1155_ADDRESS` | Deployed ERC1155 multi-token address | No |  |
| `ERC1155_DEPLOYMENT_API_URL` | URL of the ERC1155 deployment API | No | http://localhost:4002 |
| `NEXT_PUBLIC_ROBINHOOD_NETWORK` | Robinhood network (testnet) | No | testnet |
| `NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID` | WalletConnect Cloud project ID for wallet connections | Yes |  |
| `NEXT_PUBLIC_APP_NAME` | Application name displayed in wallet dialogs | No | My DApp |
| `DUNE_API_KEY` | Dune Analytics API key for blockchain data queries | Yes |  |

## Key Dependencies

| Package | Version |
|---------|---------|
| `next` | `^14.2.0` |
| `react` | `^18.3.0` |
| `react-dom` | `^18.3.0` |
| `wagmi` | `^2.12.0` |
| `viem` | `^2.21.0` |
| `@tanstack/react-query` | `^5.51.0` |
| `@rainbow-me/rainbowkit` | `^2.1.0` |
| `clsx` | `^2.1.0` |
| `tailwind-merge` | `^2.2.0` |
| `ethers` | `^6.13.0` |
| `lucide-react` | `^0.400.0` |
| `@types/node` | `^20.0.0` |
| `@types/react` | `^18.3.0` |
| `@types/react-dom` | `^18.3.0` |
| `typescript` | `^5.4.0` |
| `eslint` | `^8.57.0` |
| `eslint-config-next` | `^14.2.0` |
| `tailwindcss` | `^3.4.0` |
| `postcss` | `^8.4.0` |
| `autoprefixer` | `^10.4.0` |

## Detailed Component Specs

- [ERC-20 Token](.cradle/components/erc20-stylus--4accaf4a.md)
- [ERC-721 NFT](.cradle/components/erc721-stylus--15f54cfe.md)
- [ERC-1155 Multi-Token](.cradle/components/erc1155-stylus--9e7924e0.md)
- [Network Config](.cradle/components/robinhood-network--34140e81.md)
- [Auditware Analyzer](.cradle/components/auditware-analyzing--0893ddc4.md)
- [Contract Addresses](.cradle/components/robinhood-contracts--f3d0d92d.md)
- [Frontend](.cradle/components/frontend-scaffold--f41c86f5.md)
- [Deployment Guide](.cradle/components/robinhood-deployment--f3399a44.md)
- [OpenClaw](.cradle/components/openclaw-agent--f5b1a79a.md)
- [Wallet Auth](.cradle/components/wallet-auth--7fc516d0.md)
- [Transaction History](.cradle/components/dune-transaction-history--d81dacd9.md)

## Additional Context

- [Project Configuration](.cradle/project.md)
- [Full Architecture Details](.cradle/architecture.md)
- [All Environment Variables](.cradle/environment.md)
- [Verified Dependencies](.cradle/dependencies.md)
- [Scripts Reference](.cradle/scripts.md)
- [Integration Map](.cradle/integration-map.md)

---

*Generated by [[N]skills](https://www.nskills.xyz) — Compose N skills for your Web3 project.*
