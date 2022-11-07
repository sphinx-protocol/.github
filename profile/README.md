# Stark X - Cross-chain Orderbook DEX

<img width="1512" alt="image" src="https://user-images.githubusercontent.com/27808560/200228537-407e7aec-2390-4ab3-a8fb-7027274863e1.png">

## Links

* Website: [https://www.starkx.xyz/](https://www.starkx.xyz/)
* Documentation: [Link](https://stark-x.gitbook.io/docs/)
* Pitch deck: [Link](https://app.pitch.com/app/presentation/82d36efd-f5f4-43cd-b2a8-b058dfa5db37/3388fefa-2114-4c39-8c73-f749f8dc7f42)
* Twitter: [@starkxdex](https://twitter.com/starkxdex)
* Discord: [Link](https://discord.gg/vgEzd8ddAC)
* Email: team@starkx.xyz

Built by [@remi_gai](https://twitter.com/remi_gai) & [@park_eth](https://twitter.com/park_eth)

---

## What is Stark X?

Stark X is a natively cross-chain Central Limit Order Book (CLOB) DEX on StarkNet that allows users from other chains (Ethereum, Polygon, Arbitrum, etc.) to remotely deposit assets and trade using just their Metamask or local wallet. The DEX is a composable liquidity layer for aggregating cross-chain liquidity, without the impermanence loss or slippage of AMMs.

## How does it work?

The cross-chain concept is demonstrated through Ethereum's EIP-712. The user can sign a message that specifies an action (ex: place buy limit order, cancel order or withdraw funds). The signed message is then verified and executed on StarkNet through a third-party account (currently by us, but this step can be executed by anyone in a trustless manner or through an EIP-4337 paymaster).

We bridge assets using state proofs (enabled by Herodotus), which implements bridging at the consensus layer of the blockchain. This is a StarkNet-native solution enabled by the networks’ cheap compute to prove state transitions on-chain. Please note that as this integration is still ongoing, we have used the native Starknet L1<>L2 messaging instead for this POC.

## Demo

You can find a full product demo [here]().

![](https://github.com/stark-dex/.github/blob/main/profile/dexDemo-short.gif)

## Technical Architecture

You can find a more detailed explanation of the technical architecture in our [deck](https://app.pitch.com/app/presentation/82d36efd-f5f4-43cd-b2a8-b058dfa5db37/3388fefa-2114-4c39-8c73-f749f8dc7f42) and [documentation](https://stark-x.gitbook.io/docs/).

<img width="1512" alt="image" src="https://user-images.githubusercontent.com/27808560/200229141-20278ed6-1d6b-4e4c-8e69-bbb39e190caf.png">
<img width="1512" alt="image" src="https://user-images.githubusercontent.com/27808560/200229157-a1b74477-6d0a-4a8b-a3aa-2123fcdb53f4.png">

## Contact us

Get in touch if you are:
- An AMM who would like to integrate with STARKX’s order book for deeper liquidity
- A market maker who would like to partner with us to provide liquidity on STARKX
- A trader who would like to understand more about the benefits of STARKX

* Twitter: [@starkxdex](https://twitter.com/starkxdex)
* Discord: [https://discord.gg/vgEzd8ddAC](https://discord.gg/vgEzd8ddAC)
* Email: team@starkx.xyz


