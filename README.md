# Lottery-Smart-Contract-

# Lottery Smart Contract

This is a simple Ethereum smart contract written in Solidity for a lottery game. Players can participate by sending 1 ether, and the contract manager can pick a random winner from the pool of participants.

## Contract Details

- **Contract Address:** [Insert Contract Address]
- **Solidity Version:** 0.7.0 - 0.9.0
- **License:** GPL-3.0

## Features

- Participants can join the lottery by sending 1 ether.
- The contract manager can check the current balance.
- The manager can pick a random winner when there are at least 3 participants.
- The winner receives the entire contract balance.

## Usage

1. Deploy the smart contract to the Ethereum network.
2. Set the contract manager during deployment.
3. Participants can join by calling the `participate` function with 1 ether.
4. The manager can check the contract balance using the `getBalance` function.
5. When there are at least 3 participants, the manager can call the `pickWinner` function to select a random winner.

## Smart Contract Security Considerations

- **Randomness:** The contract uses a simple random function based on block information. For more secure randomness, consider using an external oracle or chainlink VRF.
- **Manager Privileges:** Ensure that only the intended manager can execute privileged functions.

## Development

To set up the development environment and run tests:

1. Install [Truffle](https://www.trufflesuite.com/truffle) and [Ganache](https://www.trufflesuite.com/ganache).
2. Run Ganache to start a local blockchain.
3. In the project directory, run `truffle compile` and `truffle migrate` to deploy the smart contract.
4. Run `truffle test` to execute the test suite.

## License

This smart contract is released under the [GPL-3.0 License](https://opensource.org/licenses/GPL-3.0).

Feel free to contribute, report issues, or suggest improvements!
