# Orxu Contracts

Smart contract repository for the Orxu ecosystem built with Aiken.

## Overview

This repository contains on-chain Cardano smart contracts powering the Orxu ecosystem.

Current and planned modules include:

* Token minting and burning policies
* Treasury management
* Rewards distribution
* Governance mechanisms
* Vesting contracts
* Staking integrations
* Access control validators

All contracts are implemented in Aiken and compiled to Plutus-compatible scripts for deployment on the Cardano blockchain.

## Project Structure

```text
.
├── validators/     # On-chain validators and minting policies
├── lib/            # Shared libraries and utility functions
├── env/            # Network-specific configuration
├── aiken.toml      # Project configuration
└── README.md
```

## Requirements

* Aiken
* Cardano tooling (optional for deployment)
* Git

Verify installation:

```sh
aiken --version
```

## Development

Build all contracts:

```sh
aiken build
```

Run tests:

```sh
aiken check
```

Run a specific test module:

```sh
aiken check -m <module_name>
```

Generate documentation:

```sh
aiken docs
```

## Configuration

Network configuration can be defined in `aiken.toml`:

```toml
[config.default]
network_id = 1
```

Or through environment-specific modules inside the `env/` directory.

## Security

Security is a primary concern for all contracts in this repository.

Before deployment:

* Review all validator logic
* Execute comprehensive test coverage
* Validate treasury permissions
* Audit minting policies
* Verify upgrade and governance procedures

## License

MIT License

## Author

Orxu

