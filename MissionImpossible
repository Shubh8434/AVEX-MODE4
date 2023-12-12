// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/access/Ownable.sol";

contract MissionImpossible is ERC20, Ownable(msg.sender) {

    uint public constant LootAmount = 10;
    mapping(address => bool) private LootRedeemed;


    constructor() ERC20("MissionImpossible", "MI") {
        _mint(msg.sender, LootAmount);
    }

    function mintLoot(address account, uint amount) public onlyOwner {
        _mint(account, amount);
    }

    function redeemItem() public {

        require(balanceOf(msg.sender) >= LootAmount, "Balance is less");
        require(!LootRedeemed[msg.sender], "Loot is redeemed already");
        LootRedeemed[msg.sender] = true;
        _burn(msg.sender, LootAmount);
    }

   function burnLoot(uint amount) public {
        _burn(msg.sender, amount);
    }

}
