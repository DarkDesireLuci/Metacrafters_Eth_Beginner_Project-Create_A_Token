# Metacrafters_Eth_Beginner_Project-Create_A_Token

https://www.loom.com/share/4e8318d42d7844c4ba1360457b07ac7f?sid=f8bf44fa-35b0-4a16-a279-7943f683c6cc

## Solidity Contract: Legend_Cars

This Solidity contract, named `Car`, represents a simple token contract with the following features:

### Public Variables
1. `Name`: The name of the token, set to "Legend_Cars".
2. `Abrv`: The abbreviation of the token, set to "Cars". 
3. `ttlsupply`: The total supply of the token, is set to 0.

### Mapping
The contract uses a mapping `balances` to store token balances of individual address.

### Mint Function
The `mint` function creates new tokens and assign them to a specified address. It takes two parameters:
- `_add`: The address to which the tokens will be minted.
- `_val`: The number of tokens to be minted.

The function updates the `ttlsupply` by adding the `_val` and increases the balance of the specified `_add` by the same `_val` in the balances mapping.

### Burn Function
The `burn` function destroys existing tokens. It takes two parameters:
- `_add`: The address from which the tokens will be burned.
- `_val`: The number of tokens to be burned.

1. The function first checks if the balance of the specified `_add` is greater than or equal to the `_val` to be burned. 
2. If the condition is met, it decreases the `ttlsupply` by the `_val` and decreases the balance of the specified `_add` by the same `_val`.

This contract provides a basic implementation of a token with the ability to mint and burn tokens.
