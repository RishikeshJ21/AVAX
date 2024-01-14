# AVAX MOD-1

This Solidity program is a simple "AVAX ERROR HANDLING" program that demonstrates the basic syntax and functionality of the Solidity programming language. The purpose of this program is to serve to understand the concept of  require(), assert(), revert() statements

## Description
The revert, require, and assert functions are used in this Solidity contract to handle errors based on predefined criteria. Through their handling of various scenarios, these functions are essential to maintaining the integrity of the contract.

## Getting Started

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., AVAX.sol). Copy and paste the following code into the file:

```
//SPDX-License-Identifier: MIT
pragma solidity = 0.8.23;

contract RenamedErrors {
    uint256 publicVariable = 1;

    function requireFunction(uint256 _input) public pure {
        require(_input > 200, "Input must be greater than 200"); // Checks if the input is greater than 200 using the require statement.
    }

    function assertFunction() public view {
        assert(publicVariable == 0); //It takes only one parameter
    }

    function revertFunction(uint256 _input) public pure {
        if (_input < 300) {
            revert("Input must be greater than 300");   //  Reverts the transaction with an error message if the input is less than 300.
        }
    }
}

```

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.23" (or another compatible version), and then click on the "Compile AVAX.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "HelloWorld" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling all the 3 function, Understanding the working 

## Authors

Rishikesh Jadhav
[@Rish_21_](https://twitter.com/Rish_21_)


## License

This project is licensed under the MIT License - see the LICENSE.md file for details
