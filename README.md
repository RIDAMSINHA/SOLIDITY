# MyToken Contract

## Overview
This repository contains the smart contract code for the MyToken token. MyToken is an ERC20 compatible token with the symbol "EON" and the name "EPSILON".

The contract allows the owner to mint new tokens and burn existing tokens. Only the owner has the authority to mint tokens, ensuring the integrity and controlled supply of the token.

## Contract Details

- **Token Name**: EPSILON
- **Token Symbol**: EON

## Functionalities

### Minting Tokens
The `mint` function allows the contract owner to create and assign new tokens to a specific address. The function increases the total supply and updates the balance of the target address.

### Burning Tokens
The `burn` function allows the contract owner to remove existing tokens from a specific address. The function reduces the total supply and updates the balance of the target address.

### Token Balance
The `balances` mapping allows anyone to query the token balance of a specific address.

## Deployment and Usage

To deploy the contract, follow these steps:

1. Compile the smart contract code using a Solidity compiler (e.g., Remix, Truffle).
2. Deploy the contract to an Ethereum network of your choice (e.g., local development network, public testnet, or mainnet) using a compatible Ethereum client or development framework (e.g., Remix, Truffle, Hardhat).

Once deployed, you can interact with the contract using the provided functions:

- To mint new tokens, call the `mint` function and provide the target address and the number of tokens to mint. Only the contract owner can perform this action.
- To burn existing tokens, call the `burn` function and provide the target address and the number of tokens to burn. Only the contract owner can perform this action.
- To query the balance of a specific address, access the `balances` mapping.

## Development Environment

The contract is developed using Solidity version 0.8.0. It follows the ERC20 token standard for compatibility with other Ethereum contracts and services.

## License

This project is licensed under the [MIT License](LICENSE).
