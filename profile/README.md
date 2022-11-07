# Stark X - Cross-chain Orderbook DEX

<img width="1512" alt="image" src="https://user-images.githubusercontent.com/27808560/200228537-407e7aec-2390-4ab3-a8fb-7027274863e1.png">

## Links

* Website: [https://www.starkx.xyz/](https://www.starkx.xyz/)
* Documentation: [Link](https://stark-x.gitbook.io/docs/)
* Pitch deck: [Link](https://pitch.com/public/3388fefa-2114-4c39-8c73-f749f8dc7f42)
* Demo: [Link](https://www.youtube.com/watch?v=WOqnYq6oTE0&ab_channel=RemiGai)
* Twitter: [@starkxdex](https://twitter.com/starkxdex)
* Discord: [Link](https://discord.gg/vgEzd8ddAC)
* Email: team@starkx.xyz

Built by [@remi_gai](https://twitter.com/remi_gai) and [@park_eth](https://twitter.com/park_eth) for the October 2022 StarkNet Online Hackathon.

---

## What is Stark X?

Stark X is the first natively cross-chain and composable Central Limit Order Book (CLOB) DEX deployed on StarkNet for trustless settlement and asset liquidity. Using trustless bridging, we allow users from other chains (Ethereum, Polygon, Arbitrum, etc.) to remotely deposit assets and trade using just their Metamask or local wallet. In this way, the DEX acts as a composable liquidity layer for aggregating cross-chain liquidity, without the impermanence loss or slippage of AMMs.

StarkNet is a Layer 2 blockchain that publishes validity proofs (sometimes known as ZK proofs) of its state transitions to Ethereum. This means it inherits the strong security properties of Ethereum while benefiting from the unprecedented scalability and cross-chain composability enabled by L2 StarkNet.

## How does it work?

We implement cross-chain messaging using Ethereum's EIP-712. The user signs a message from Ethereum to specify a particular action to be performed(ex: place buy limit order, cancel order or withdraw funds). The signed message is then verified on StarkNet and executed through a third-party (currently us, but this step can be fully decentralised, or implemented as an EIP-4337 paymaster).

Assets are bridged across chain using state proofs, enabled by Herodotus. State proofs are a solution for implementing bridging at the consensus layer of the blockchain. It leverages StarkNet's cheap compute to prove state transitions through an on-chain smart contract. Please note that as this integration is still ongoing, for purposes of the hackathon we have used the native Starknet L1<>L2 messaging instead for this POC.

## Demo

You can find a full product demo [here](https://youtu.be/WOqnYq6oTE0).

![](https://github.com/stark-dex/.github/blob/main/profile/dexDemo-short.gif)

## Technical Architecture

You can find a more detailed explanation of the technical architecture in our [deck](https://pitch.com/public/3388fefa-2114-4c39-8c73-f749f8dc7f42) and [documentation](https://stark-x.gitbook.io/docs/).

<img width="1512" alt="image" src="https://user-images.githubusercontent.com/27808560/200229141-20278ed6-1d6b-4e4c-8e69-bbb39e190caf.png">
<img width="1512" alt="image" src="https://user-images.githubusercontent.com/27808560/200229157-a1b74477-6d0a-4a8b-a3aa-2123fcdb53f4.png">

## Contact us

Get in touch if you are:
- An AMM who would like to integrate with STARKX’s order book for deeper liquidity
- A market maker who would like to partner with us to provide liquidity on STARKX
- A trader who would like to understand more about the benefits of STARKX

Twitter: [@starkxdex](https://twitter.com/starkxdex)
Discord: [https://discord.gg/vgEzd8ddAC](https://discord.gg/vgEzd8ddAC)
Email: team@starkx.xyz

