#### ⚠️ You should be aware that the contract has not been auditized and that there may be a bug in the action.

# Solana Token Sale Program

<p align="center">
  <a href="https://solana.com">
    <img alt="Solana" src="https://i.imgur.com/uBVzyX3.png" width="250" />
  </a>
</p>

<p><p>

## Prerequisite

- Install node (v14 recommended)
- Install npm
- Install the latest Rust stable from https://rustup.rs/
- Install Solana v1.7.11 or later from https://docs.solana.com/cli/install-solana-cli-tools

## Quick Start

- Build Rust
- Setup Solana Config and Test-Validator(Single node cluster)
- Set Environment
- Run RPC Client

### Build Rust

Build Rust and get `.so` file. You should conduct following command on `contract` folder

```
cargo build-bpf
```

Run test-validator

```
solana-test-validator -r --bpf-program 5yznMbghv1Z2Gb4uaKkY9fxb9PkLMrSn9xgjswucHq4X ${.so}
```

> If you want to get more information about validator. <p>
> Use `solana-test-validator -h`

### Setup Solana

Set CLI config url to localhost cluster

```
solana config set --url localhost
```

Create CLI Keypair
If this is your first time using the Solana CLI, you will need to generate a new keypair:

```
solana-keygen new
```

> This program need two account which are seller and buyer. You should create two account, if you don't have any

### Set Environment

Before running RPC Client, Change `.example-env` to `.env`.<p>
And refer to the below and fill NEEDED section.

```

```

### Run RPC Client

Install the necessary dependencies for running RPC Client. You should conduct following command on `client` folder

```
npm install
```

Run RPC Client for interaction with on-chain program what you published.

```
npm run setup
npm run startTokenSale (which include setup process also)
npm run buyToken
```

## Further

### SmartContract

- Nothing

### RPC Client

- Nothing
