# Datcoin.sol

This is a solidity contract to create our own ERC20 token. This beginner-friendly program explores the process to create our very own cryptocurrency.

## Description

Solidity is a programming language used for creating smart contracts on the Ethereum blockchain network. This is a simple Solidity program to create a smart contract named "Datcoin" to create a cryptocurrency by the name of "DATCOIN" abbreviated as "DTC". It makes use of ERC20.sol contract from Openzappelin. It has a constructor which inherits form ERC20 contract and mints 100 DTC.

## Getting Started

### Executing the contract

Remix is an online Solidity IDE available at https://remix.ethereum.org/. It has the look of Visual Studio Code and can be used to get started with Web3 Development. Go to the before stated website and create a new file with a .sol extension (e.g., Token.sol). Copy and paste the following code.

```javascript
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.13;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.0.0/contracts/token/ERC20/ERC20.sol";

contract Datcoin is ERC20 {
    constructor() ERC20("DATCOIN", "DTC") {
        _mint(msg.sender, 100 * 10**uint(decimals()));
    }
}
```

Hit Control + S to compile. Then deploy the contract by clicking "Deploy & run transactions" on the left hand side bar. Click on the "Deploy" button. The contract is now deployed. 

## Authors

Aditya
