# s7__crypto__2025__m5

A Solidity development environment using Hardhat for smart contract development and deployment to Blast Sepolia network.

## Prerequisites

- Node.js (v14 or higher)
- npm
- A wallet with Blast Sepolia testnet ETH

## Installation

Install dependencies:

```bash
npm install
```

## Configuration

Create a `.env` file in the root directory with your private key:

```bash
cp .env.example .env
```

Then edit `.env` and add your private key:

```
PRIVATE_KEY=your_private_key_here
```

**⚠️ Warning:** Never commit your `.env` file or share your private key!

## Project Structure

```
.
├── contracts/          # Solidity smart contracts
├── scripts/           # Deployment scripts
├── hardhat.config.js  # Hardhat configuration with Blast Sepolia network
└── package.json       # Project dependencies and scripts
```

## Available Commands

### Compile Contracts

```bash
npm run compile
```

### Run Hardhat Node

Start a local Ethereum network:

```bash
npm run node
```

### Deploy to Blast Sepolia

Deploy contracts to Blast Sepolia testnet:

```bash
npm run deploy:blast-sepolia
```

Or using hardhat directly:

```bash
npx hardhat run scripts/deploy.js --network blastSepolia
```

### Other Hardhat Commands

```bash
npx hardhat help
npx hardhat accounts
npx hardhat clean
```

## Networks

### Blast Sepolia Testnet
- **RPC URL:** https://sepolia.blast.io
- **Chain ID:** 168587773
- **Block Explorer:** https://testnet.blastscan.io

To get Blast Sepolia testnet ETH, visit the Blast Sepolia faucet.

## Sample Contract

The project includes a sample `Lock` contract that demonstrates:
- Time-locked withdrawals
- Payable constructors
- Event emissions
- Access control

## Contributing

Feel free to submit issues or pull requests.

## License

ISC