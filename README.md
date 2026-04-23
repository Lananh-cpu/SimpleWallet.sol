# SimpleWallet.sol
SimpleWallet.sol
pragma solidity ^0.8.20;
contract SimpleWallet {
    function deposit() public payable {}

    function withdraw(address payable to, uint amount) public {
        to.transfer(amount);
    }
}
