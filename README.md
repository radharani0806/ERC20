# Token Smart Contract

This is a basic ERC-20 token smart contract written in Solidity. The contract includes features like token minting, burning, transferring, and emergency transfer by the owner. It also extends the OpenZeppelin ERC20 and Ownable contracts to leverage established standards and ownership control.

## Table of Contents

- [Overview](#token-smart-contract)
- [Features](#features)
- [Usage](#usage)
- [Functions](#functions)
- [Deployment](#deployment)
- [License](#license)

## Features

1. **Minting and Burning:** The contract allows the owner to mint new tokens and burn existing tokens.
2. **Transferring Tokens:** Users can transfer tokens to other addresses using the standard ERC-20 `transfer` function.
3. **Emergency Transfer:** The owner has the ability to perform an emergency transfer to a specified address.
4. **Increase Total Supply:** The owner can increase the total supply of tokens.

## Usage

To use this smart contract, you can deploy it to a compatible Ethereum blockchain. The contract can be interacted with through Ethereum wallets, smart contract interactions, or dApps.

## Functions

### `mintTokens(address claimant, uint256 amount) external onlyOwner`

Mints a specified amount of tokens and assigns them to the specified address.

### `burnTokens(uint256 amount) external`

Burns a specified amount of tokens, reducing the total supply.

### `increaseTotalSupply(uint256 amount) external onlyOwner`

Increases the total supply of tokens by minting new tokens to the owner's address.

### `transfer(address claimant, uint256 amount) public virtual override returns (bool)`

Transfers a specified amount of tokens from the sender's address to the specified address.

### `emergencyTransfer(address receiver, uint256 amount) external onlyOwner`

Performs an emergency transfer of a specified amount of tokens to the specified address. Only the owner can execute this function.

## Deployment

The contract is intended to be deployed on an Ethereum-compatible blockchain. Make sure to set the appropriate constructor parameters, such as the title, code, and initial supply, when deploying the contract.

## License

This smart contract is distributed under the MIT License. See `LICENSE` for more information.

## Author 

radhakrishna3722@gmail.com
