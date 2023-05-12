# Sphinx

![](https://github.com/sphinx-dex/.github/blob/main/profile/Sphinx-short-video.gif)

## Links

* Website: [https://www.sphnx.xyz/](https://www.sphnx.xyz/)
* Documentation: [Link](https://sphinx-docs.gitbook.io/)
* Pitch deck: [Link](https://pitch.com/public/2b9a6244-de76-4ab5-a725-c32ad00214b4)
* Demo: [Link](https://youtu.be/hxNjCYst1K4Q)
* Twitter: [@sphinxdex](https://twitter.com/sphinxdex)
* Discord: [Link](https://discord.gg/vgEzd8ddAC)
* Email: founders@sphinxlabs.xyz

1st place win at the October 2022 StarkNet Autumn Hackathon. Built by [@remi_gai](https://twitter.com/remi_gai) and [@park_eth](https://twitter.com/park_eth).

---

## What is Sphinx?

Sphinx is the first natively cross-chain and composable Central Limit Order Book (CLOB) DEX deployed on StarkNet for trustless settlement and asset liquidity. Using trustless bridging, we allow users from other chains (Ethereum, Polygon, Arbitrum, etc.) to remotely deposit assets and trade using just their Metamask or local wallet. In this way, the DEX acts as a composable liquidity layer for aggregating cross-chain liquidity, without the impermanence loss or slippage of AMMs.

StarkNet is a Layer 2 blockchain that publishes validity proofs (sometimes known as ZK proofs) of its state transitions to Ethereum. This means it inherits the strong security properties of Ethereum while benefiting from the unprecedented scalability and cross-chain composability enabled by L2 StarkNet.

## How does it work?

We implement cross-chain messaging using Ethereum's EIP-712. The user signs a message from Ethereum to specify a particular action to be performed(ex: place buy limit order, cancel order or withdraw funds). The signed message is then verified on StarkNet and executed through a third-party (currently us, but this step can be fully decentralised, or implemented as an EIP-4337 paymaster).

Assets are bridged across chain using state proofs, enabled by Herodotus. State proofs are a solution for implementing bridging at the consensus layer of the blockchain. It leverages StarkNet's cheap compute to prove state transitions through an on-chain smart contract. Please note that as this integration is still ongoing, for purposes of the hackathon we have used the native Starknet L1<>L2 messaging instead for this POC.

## Technical Architecture

You can find a more detailed explanation of the technical architecture in our [deck](https://pitch.com/public/2b9a6244-de76-4ab5-a725-c32ad00214b4) and [documentation](https://sphinx-docs.gitbook.io/).

<img width="1230" alt="image" src="https://user-images.githubusercontent.com/27808560/206443870-ddb4b807-d22f-4879-8651-9ea0df6fff7f.png">
<img width="1230" alt="image" src="https://user-images.githubusercontent.com/27808560/205241937-7f9fb296-18b3-4e6a-aeba-174ec4ae7e47.png">

## Demo

We have created a mock frontend to demonstrate the functionality of the DEX. You can find a full product demo [here](https://www.youtube.com/watch?v=5iFHXK6_lEQ).

## Contact us

Get in touch if you are:
- An AMM who would like to integrate with Sphinx’s order book for deeper liquidity
- A market maker who would like to partner with us to provide liquidity on Sphinx
- A trader who would like to understand more about the benefits of Sphinx

Twitter: [@sphinxdex](https://twitter.com/sphinxdex)\
Discord: [https://discord.gg/vgEzd8ddAC](https://discord.gg/vgEzd8ddAC)\
Email: founders@sphinxlabs.xyz

