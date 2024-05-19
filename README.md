Ethereum-Programming-Language-and-Solidity-MyToken-Method-Walkthrough

This Solidity Program is used to demonstrate the transaction in NFTs revolving around the digital currency we call tokens.

## Description

It focuses on the process of transaction between the user and its system. Acting purposefully to check, add, remove said balances of tokens to which is approriately correct at situation at the time.

## Getting Started

### Installing

* Go to the website: https://remix.ethereum.org/
* Follow along the video walkthrough

### Executing program

* How to run the program
* Step-by-step bullets
```
contract MyToken {

    // public variables here
    string public tokenName = "META";
    string public tokenAbbrv = "MTA";
    uint public totalSupply = 0;

    // mapping variable here
    mapping(address => uint) public balances;


    // mint function
    function mint (address _address, uint _value ) public {
      totalSupply += _value;
      balances[_address] +=_value;
    }

    // burn function
    function burn (address _address, uint _value) public {
      if (balances[_address] >= _value) {
        totalSupply -= _value;
        balances[_address] -= _value;
    }

}
}
```

## Help

Make sure of the line of code and symbols used to avoid errors.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

Simon Tuazon
@itsmonskers(https://www.instagram.com/itsmonskers/)


## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
