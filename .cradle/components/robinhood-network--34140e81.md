# Network Config

| Field | Value |
|-------|-------|
| Type | `robinhood-network` |
| ID | `34140e81` |
| Category | robinhood |
| Tags | robinhood, network, config, rpc, orbit |
| Description | Robinhood Chain testnet RPC and chain configuration |

## Environment Variables

| Key | Description | Required | Secret | Default |
|-----|-------------|----------|--------|---------|
| `NEXT_PUBLIC_ROBINHOOD_NETWORK` | Robinhood network (testnet) | No | No | testnet |

## Documentation

### Robinhood Chain Integration

# Robinhood Chain Integration

This module provides configuration for the Robinhood Chain testnet.

## Overview

Robinhood Chain Testnet is an Arbitrum Orbit Layer 2 built on Ethereum, using ETH as the native gas token.

## Network Details

- **Chain ID**: 46630
- **RPC URL**: https://rpc.testnet.chain.robinhood.com
- **WebSocket**: wss://feed.testnet.chain.robinhood.com
- **Explorer**: https://explorer.testnet.chain.robinhood.com
- **Faucet**: Deposit testnet funds via the official faucet or bridge Sepolia ETH

## Usage

```typescript
import { robinhoodTestnet } from './lib/chains';
import { createConfig } from 'wagmi';

const config = createConfig({
  chains: [robinhoodTestnet],
  // ... other config
});
```

## Resources

- [Robinhood Chain Explorer](https://explorer.testnet.chain.robinhood.com)

## File Structure

This component would generate the following files:

- `chains.ts` (frontend-lib)
- `wagmi-robinhood.ts` (frontend-lib)
- `robinhood-constants.ts` (frontend-lib)
- `useRobinhoodNetwork.ts` (frontend-hooks)
- `robinhood.ts` (frontend-lib)

## Integration Points

**Provides to:**
- Frontend-scaffold (`f41c86f5`)
- Robinhood-contracts (`f3d0d92d`)

