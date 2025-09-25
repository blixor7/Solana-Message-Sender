
# Solana-Message-Sender

A demo toolkit for sending messages to Solana wallets on-chain, featuring basic program deployment and wallet interaction.

## Features

- Connect to Solana clusters (devnet, mainnet-beta, testnet)
- Send and receive messages via wallet instructions
- Reference server/client setup for rapid prototyping

## Getting Started

**1. Install dependencies:**
```bash
npm install
```

**2. Start local devnet client/server:**
```bash
npm run cluster:devnet
npm run server
```
Server will start at [http://localhost:8888](http://localhost:8888).

**3. Build the on-chain Solana program:**
```bash
npm run build:program-rust
```

## Project Structure

- `src/` – main message-sending logic and wallet utils
- `dist/program` – built Solana program artifacts
- `*.env` – cluster configuration files for devnet, testnet, and mainnet-beta

## Usage Roadmap

- Compose and sign transactions with wallet adapters
- List messages sent/received by connected wallets (to be added)

## Resources

- [Solana Wallet Adapter Guide](https://docs.cdp.coinbase.com/coinbase-wallet/solana-developers/solana-wallet-adapter/getting-started-guide)[1]
- [Solana Connection Providers and Wallet Context](https://solana.com/developers/courses/intro-to-solana/interact-with-wallets)[3]
- [How to Connect Wallets with React](https://solana.com/developers/cookbook/wallets/connect-wallet-react)[6]

## Contributing

Feel free to fork or open issues to improve on-chain message utilities, add support for more wallets, or contribute UI enhancements.
