## Introduction

Solidity is the main programming language used for writing smart contracts on various blockchain platforms, including Celo. This challenge focuses on understanding Solidity inheritance and the interaction between multiple contracts.

## Problem Statement

Create two interacting contracts that demonstrate inheritance with the following requirements:

1. The first contract, named "Base", should implement a basic counter functionality with increment, decrement, and get counter functions.
2. The second contract, named "Derived", should inherit from the "Base" contract and introduce an additional function to reset the counter.
3. The "Derived" contract should only allow the contract owner to reset the counter.
4. Demonstrate interaction between these two contracts from another (third) contract named "Interaction".
5. The "Interaction" contract should be able to call all functions from the "Derived" contract and also update the counter.

## Hints

- Use Solidity's `is` keyword to inherit from the "Base" contract in the "Derived" contract.
- Make use of the `msg.sender` global variable to keep track of the contract owner.
- Use `require()` to enforce contract rules, such as ensuring only the owner can reset the counter.
- Instantiate the "Derived" contract within the "Interaction" contract to interact with its functions.
- Use `import` keyword to use contracts from different files if necessary.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and meet all requirements.
- **Readability**: The contract should be easy to understand, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Keep in mind that this challenge is a fundamental exercise and doesn't cover important aspects such as security, gas optimization, and contract upgradability, which are critical for a real-world contract on the Celo platform.

For a comprehensive understanding of Celo smart contracts and Solidity, please refer to the Celo and Solidity documentation.

## Submission

Please reply with a link to your PR on GitHub, including your "Base", "Derived", and "Interaction" contracts. Along with that, provide any notes or comments you think are necessary for understanding your design and choices. Also, provide a brief explanation about how each function of the contract should be tested.
