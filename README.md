# CounterWithLimit.sol
Contract deployed via Web3  CounterWithLimit.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract CounterWithLimit {
    uint public count;

    function increment() public {
        require(count < 100, "Limit reached");
        count++;
    }
}
