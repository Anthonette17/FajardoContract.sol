# FajardoContract.sol
The contract TheNumberGame is a simple game where players guess a number. If the guessed number matches the target number set by the game owner, the game ends.

# Description
The TheNumberGame contract is a simple guessing game with controlled state changes. It uses Solidity's require, assert, and revert functions to enforce rules and ensure the contract behaves correctly. The game owner has special privileges to set the target number, and the game can only end once a correct guess is made.

# Getting Started

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract TheNumberGame {
    address public gameOwner;
    uint256 public targetNumber;
    bool public isGameEnded;

    event GameOver(address indexed winner, uint256 targetNumber);

    constructor() {
        gameOwner = msg.sender;
        targetNumber = 42; // Initial target number
        isGameEnded = false;
    


## Authors

Metacrafter Anthonette

## License
This project is licensed under the MIT License - see the LICENSE.md file for details
    
