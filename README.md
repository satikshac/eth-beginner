# eth-beginner

This contract defines a basic token system with public variables,balances mapping,mint function and burn function.This contract provides aa basic functional framework for creating and managing a custom cryptocurrency token on ethereum blockchain.It's simplicity makes it a good starting point for understanding how token contracts work.

## Description

The 'MyToken' contract is a basic implementation of a cryptocurrency on Ethereum, featuring public variables for token name, abbreviation, and total supply. It includes a mint function to create tokens and assign them to a specified address, increasing both the total supply and the address's balance. The burn function destroys tokens, reducing the address's balance and the total supply, with checks to ensure sufficient balance. Balances are tracked using a mapping from addresses to token amounts.

## Output of the program

![Screenshot (176)](https://github.com/satikshac/eth-beginner/assets/170428250/cb40e293-fcc4-4111-a945-0825684b0fb3)

![Screenshot (177)](https://github.com/satikshac/eth-beginner/assets/170428250/8df793cf-48b6-4e9b-8cba-2511bc323df2)

![Screenshot (178)](https://github.com/satikshac/eth-beginner/assets/170428250/74e2a79f-4586-4d6e-9a6e-872259a711dc)



*To run this program, Remix, an online Solidity IDE is used. To get started, go to the Remix website at https://remix.ethereum.org/.

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" , and then click on the "myToken.sol" button.
Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "myToken" contract from the dropdown menu, and then click on the "Deploy" button.
## Authors
Satiksha Choudhary
(satikshac@gmail.com)


## License

This project is licensed under the MIT License.
