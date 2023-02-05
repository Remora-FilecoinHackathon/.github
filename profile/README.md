## Remora - FVM Space Warp Hackathon Project 👋

## Demo

## Inspiration
Storage providers (SPs) have to post $FIL collateral to onboard network storage capacity and accept storage deals. This collateral incentivizes the storage provider to behave
correctly, by presenting timely proofs of the health of the data (PoRep, PoSt), or they risk getting slashed.
While important, the need to pledge collateral creates friction and an immediate barrier that
throttles SP participation and growth. On the other hand, the Filecoin network has a large base
of long-term token holders that would like to see the network grow, and are willing to lend their
FIL to reputable and growth-oriented SPs.
A lending protocol can solve this issue. Storage providers can borrow collateral from lenders and
the smart contract will lock the future income until the storage providers have repaid their loan.

Remora allows a user with liquidity to lend out his $FILs and enhance the network and an SP to borrow collateral-free $FILs and become an SP (or improve its $FIL collateral) by repaying his debt through the rewards it gets from his storage-providing activity.

The idea comes from the following: [https://fvm-forum.filecoin.io/t/lending-pool-cookbook/114](https://fvm-forum.filecoin.io/t/lending-pool-cookbook/114)

## What it does
Remora is a collateral-free $FIL lending and borrowing protocol to facilitate network storage providing. Remora works following an order book model where lenders create loan positions making $FIL available with a certain interest rate and borrowers can take a designated amount based on pledging and collateral requirements in offering computer storage services.

The borrower must repay its debt and the loan interest through the rewards it gets from its storage-providing activity. 

Under the hood, Remora smart contracts interact with the built-in Miner Actor using Filecoin Solidity API libraries.
