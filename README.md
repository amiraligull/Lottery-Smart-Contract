<!-- @format -->

# Lottery Contract

This is a simple Ethereum smart contract written in Solidity for organizing a lottery. The contract allows participants to enter the lottery by sending a specific amount of Ether and enables the manager (the creator of the contract) to pick a winner randomly once there are at least three participants.

## How to Use

To participate in the lottery:

1. Make sure you have an Ethereum wallet set up (such as MetaMask).
2. Access the contract through an Ethereum-compatible interface.
3. Send exactly 0.1 Ether to the contract address.

To pick a winner:

1. Only the manager (the one who deployed the contract) can execute the `pickWinner` function.
2. Ensure there are at least three participants in the lottery.
3. Call the `pickWinner` function, which will randomly select a winner among the participants.
4. The entire balance of the contract will be transferred to the chosen winner.
5. The lottery will reset for the next round.

## Contract Details

- **Manager**: The address of the manager is the one who deployed the contract. This address has privileges to pick a winner and check the contract's balance.
- **Participants**: Participants are represented by their Ethereum addresses. Anyone can become a participant by sending 0.1 Ether to the contract.
- **Winning Mechanism**: The winner is selected randomly using a pseudo-random number generator. This randomness is based on factors like block difficulty, timestamp, and the number of participants.
- **Balance**: The contract maintains a balance in Ether, which is accumulated from the participants' entry fees. This balance is transferred entirely to the winner upon selection.

## Smart Contract Information

- **SPDX-License-Identifier**: GPL-3.0
- **Solidity Version**: >=0.5.0 <0.9.0

## Contact

If anyone needs any kind of smart contract development service or full-stack developer, feel free to contact Amir Ali at Amirgull422@gmail.com or send directly what's App : +923196468462 .

## Disclaimer

This contract is provided as an educational example and should not be used in a production environment without thorough testing and auditing. Smart contracts handle real funds and must be carefully reviewed to ensure they function as intended and do not contain security vulnerabilities. The developer(s) and owner(s) of this contract are not responsible for any loss of funds or damages resulting from its use.
