# eth-beginner

This contract defines a basic token system with public variables,balances mapping,mint function and burn function.This contract provides aa basic functional framework for creating and managing a custom cryptocurrency token on ethereum blockchain.It's simplicity makes it a good starting point for understanding how token contracts work.

## Description

The 'MyToken' contract is a basic implementation of a cryptocurrency on Ethereum, featuring public variables for token name, abbreviation, and total supply. It includes a mint function to create tokens and assign them to a specified address, increasing both the total supply and the address's balance. The burn function destroys tokens, reducing the address's balance and the total supply, with checks to ensure sufficient balance. Balances are tracked using a mapping from addresses to token amounts.

## Getting Started
### Executing program

// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

/*
       REQUIREMENTS
    1. Your contract will have public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply)
    2. Your contract will have a mapping of addresses to balances (address => uint)
    3. You will have a mint function that takes two parameters: an address and a value. 
       The function then increases the total supply by that number and increases the balance 
       of the “sender” address by that amount
    4. Your contract will have a burn function, which works the opposite of the mint function, as it will destroy tokens. 
       It will take an address and value just like the mint functions. It will then deduct the value from the total supply 
       and from the balance of the “sender”.
    5. Lastly, your burn function should have conditionals to make sure the balance of "sender" is greater than or equal 
       to the amount that is supposed to be burned.
*/

contract MyToken {

    // public variables here
    string public tokenName = "SATIKSHA";
    string public tokenAbbrv = "STA";
    uint public totalSupply = 0;
    // mapping variable here
    mapping(address => uint)public balances;
    // mint function
    function mint (address _address, uint _value)public{
        totalSupply += _value;
        balances[_address] += _value;
    }
    // burn function
    function burn (address _address, uint _value)public{
        if (balances[_address] >= _value){
         totalSupply -= _value;
         balances[_address] -= _value;
        }
    }

}

*To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" , and then click on the "myToken.sol" button.
Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "myToken" contract from the dropdown menu, and then click on the "Deploy" button.
## Authors
Satiksha Choudhary
(satikshac@gmail.com)


## License

This project is licensed under the MIT License.
