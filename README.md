// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract amount{
    uint public money;
    string name;

    function getmoney(uint _money, string memory _name) public
    {
        name=_name;
        money=_money;
    }
    //increase money by 5 times;
    function increase() public returns(uint){
        money=money*5;
        return money;
    }
    function showUser() public view returns(string memory newName) {

        return name;
    }
    function showMoney() public view returns(uint newmoney) {

        return money;
    }
}
