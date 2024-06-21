# Lottery Smart Contract
# Overview
This project is a simple Lottery smart contract implemented in Solidity. Participants can enter the lottery by sending 0.01 ether to the contract. The contract manager can select a winner from the participants and transfer the total balance to the winner.

# Features
Enter the Lottery: Participants enter the lottery by sending 0.01 ether to the contract address.
View Contract Balance: The contract manager can view the total balance of the contract.
Select Winner: The contract manager can randomly select a winner from the participants and transfer the total balance to the winner.

# Prerequisites
Solidity compiler version 0.5.0 to 0.9.0
Ethereum development environment (e.g., Remix, Truffle)
MetaMask or any other Ethereum wallet for interacting with the contract

# Contract Details

# Variables
manager: The address of the contract manager (deployer of the contract).
participants: A dynamic array of participant addresses.
Constructor
constructor(): Sets the contract deployer as the manager.
Functions
receive() external payable: Allows participants to enter the lottery by sending 0.01 ether to the contract. The participant's address is added to the participants array.
