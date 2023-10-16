MyToken Solidity Smart Contract
Overview
This is a basic Solidity smart contract for a custom token named "MyToken." It represents a simplified ERC-20 token with features for minting and burning tokens.

Contract Details
Compiler Version: Solidity 0.8.18
License: MIT
Public Variables
tokenName: A public string variable representing the name of the token. It is set to "butterfly."

tokenAbbrv: A public string variable representing the abbreviation of the token. It is set to "but."

totalSupply: A public uint variable representing the total supply of the token. Initially, it is set to 0.

Mapping Variable
balances: A public mapping that associates Ethereum addresses with their respective token balances. It maps an address to a uint, representing the balance of tokens for that address.
Mint Function
Function Name: mint
Description: This function is used to create new tokens and assign them to a specified address. It increases the total supply and updates the balance for the specified address.
Parameters:
_address: The address to which tokens will be minted.
_value: The number of tokens to be minted.
Burn Function
Function Name: burn
Description: This function allows an address to burn (destroy) a specific number of tokens from their balance. It checks if the address has a sufficient balance before reducing the total supply and updating the balance accordingly. If the balance is insufficient, the function will revert with an "Insufficient balance" error.
Parameters:
_address: The address that will burn tokens.
_value: The number of tokens to be burned.
Important Notes
This contract is a basic example and lacks several important functionalities that a production-ready ERC-20 token should have, such as events, transfer functions, and approvals.
It is essential to carefully consider the security and functionality requirements when creating a real token contract.
The Solidity compiler version used in this contract is outdated; you may want to use a more recent version of Solidity for better compatibility and security.
