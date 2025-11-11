# s7__crypto__2025__m5

A Solidity development environment using Hardhat for smart contract development, testing, and deployment.

## Prerequisites

- Node.js (v14 or higher)
- npm

## Installation

Install dependencies:

```bash
npm install
```

## Project Structure

```
.
├── contracts/          # Solidity smart contracts
├── scripts/           # Deployment scripts
├── test/              # Test files
├── hardhat.config.js  # Hardhat configuration
└── package.json       # Project dependencies and scripts
```

## Available Commands

### Compile Contracts

```bash
npm run compile
```

### Run Tests

```bash
npm test
```

### Run Hardhat Node

Start a local Ethereum network:

```bash
npm run node
```

### Deploy Contracts

Deploy to local network:

```bash
npx hardhat run scripts/deploy.js --network localhost
```

### Other Hardhat Commands

```bash
npx hardhat help
npx hardhat accounts
npx hardhat clean
npx hardhat coverage
```

## Sample Contract

The project includes a sample `Lock` contract that demonstrates:
- Time-locked withdrawals
- Payable constructors
- Event emissions
- Access control

## Testing

The test suite uses:
- Mocha test framework
- Chai assertions
- Hardhat Network Helpers for time manipulation
- Ethers.js for contract interactions

## Contributing

Feel free to submit issues or pull requests.

## License

ISC