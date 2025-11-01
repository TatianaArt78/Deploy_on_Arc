## 🚀 HelloArchitect — Smart Contract on Arc Testnet

This project demonstrates how to deploy a simple Solidity contract to the **Arc Testnet** using **Foundry** and **GitHub Actions**, without installing anything locally.

---

### 🧱 Contract

**File:** `src/HelloArchitect.sol`

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.30;

contract HelloArchitect {
    string private greeting = "Hello Architect!";

    event GreetingChanged(string newGreeting);

    function getGreeting() public view returns (string memory) {
        return greeting;
    }

    function setGreeting(string memory newGreeting) public {
        greeting = newGreeting;
        emit GreetingChanged(newGreeting);
    }
}
