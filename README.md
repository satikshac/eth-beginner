# eth-beginner

This contract defines a basic token system with public variables,balances mapping,mint function and burn function.This contract provides aa basic functional framework for creating and managing a custom cryptocurrency token on ethereum blockchain.It's simplicity makes it a good starting point for understanding how token contracts work.

## Description

The 'MyToken' contract is a basic implementation of a cryptocurrency on Ethereum, featuring public variables for token name, abbreviation, and total supply. It includes a mint function to create tokens and assign them to a specified address, increasing both the total supply and the address's balance. The burn function destroys tokens, reducing the address's balance and the total supply, with checks to ensure sufficient balance. Balances are tracked using a mapping from addresses to token amounts.

## Getting Started

*To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" , and then click on the "myToken.sol" button.
Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "myToken" contract from the dropdown menu, and then click on the "Deploy" button.
## Authors
Satiksha Choudhary
(satikshac@gmail.com)


## License

This project is licensed under the MIT License.
