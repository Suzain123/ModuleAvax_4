# Points Smart Contract

This is a Solidity smart contract called "Points" that extends the functionality of ERC-20 tokens. It allows for minting, transferring, burning, and redeeming tokens, and it also provides a way to check the balance of tokens held by an address. The contract is named "Degen" with the symbol "DGN."

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Functions](#functions)
- [License](#license)

## Introduction

The Points smart contract is designed to be a simple ERC-20 token with additional functionality. It is implemented using Solidity and inherits from two OpenZeppelin contracts: `ERC20` and `Ownable`. The contract provides the owner with the ability to mint new tokens, while users can transfer, burn, and redeem tokens as needed.

## Features

1. **Minting Tokens**: The contract owner can mint new tokens by calling the `mint` function, specifying the recipient's address and the amount to mint.

2. **Transferring Tokens**: Users can transfer tokens to another address using the `transferTokens` function. This function requires the sender to have a sufficient balance.

3. **Burning Tokens**: Users can burn their own tokens using the `burnTokens` function, effectively reducing the total token supply.

4. **Redeeming Tokens**: Users can redeem tokens by transferring them to the contract itself using the `redeemTokens` function.

5. **Balance Inquiry**: Users can check their token balance using the `getBalance` function.

## Getting Started

To use this smart contract, you can follow these steps:

1. Deploy the contract to the Ethereum blockchain, specifying the initial token supply, name, and symbol.

2. As the contract owner, you can mint new tokens to distribute to users or perform other operations.

3. Users can interact with the contract by transferring, burning, or redeeming tokens as needed.

## Functions

Here is a brief description of the contract's functions:

- `mint(address to, uint256 amount)`: Mint new tokens and assign them to the specified address. Only the contract owner can call this function.

- `getBalance()`: Get the token balance of the caller's address.

- `transferTokens(address _rec, uint256 _value)`: Transfer tokens to another address. The caller must have a sufficient balance and approve the contract to spend their tokens.

- `burnTokens(uint _value)`: Burn tokens from the caller's balance. This operation reduces the total supply of tokens.

- `redeemTokens(uint _value)`: Redeem tokens by transferring them to the contract. This can be useful for various purposes like staking or participation in other contract functions.

## License

This contract is released under the MIT License. You can find the full license text in the SPDX-License-Identifier comment at the beginning of the contract.

