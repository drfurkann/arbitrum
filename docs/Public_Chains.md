---
id: Public_Chains
title: Public Arbitrum Chains
sidebar_label: Public Arbitrum Chains
---

The following is a comprehensive list of all of the currently live Arbitrum chains:

<em id="public-chains-table" class="arb-docs-table">
| Name                            | RPC Url(s)                                                                                                                                       | ID     | Native Currency | Explorer(s)                                                             | Underlying L1 | Current Tech Stack | Sequencer Feed                         | Nitro Seed Database URLs                 | Retryable Dashboard                                                                   |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------ | --------------- | ----------------------------------------------------------------------- | ------------- | ------------------ | -------------------------------------- | ---------------------------------------- | ------------------------------------------------------------------------------------- |
| Arbitrum One                    | `https://arb1.arbitrum.io/rpc`<br>`https://arbitrum-mainnet.infura.io/v3/YOUR-PROJECT-ID`<br>`https://arb-mainnet.g.alchemy.com/v2/-KEY`         | 42161  | ETH             | `https://arbiscan.io/`<br>`https://explorer.arbitrum.io/`               | Ethereum      | Classic Rollup     | `wss://arb1.arbitrum.io/feed`          | Not Available Yet                        | [retryable-dashboard.arbitrum.io](https://retryable-dashboard.arbitrum.io/)           |
| Arbitrum Nova                   | `https://nova.arbitrum.io/rpc`                                                                                                                   | 42170  | ETH             | `https://nova-explorer.arbitrum.io/`                                    | Ethereum      | Nitro AnyTrust     | `wss://nova.arbitrum.io/feed`          | N/A                                      | [retryable-dashboard.arbitrum.io](https://retryable-dashboard.arbitrum.io/) |
| RinkArby^                       | `https://rinkeby.arbitrum.io/rpc`                                                                                                                | 421611 | RinkebyETH      | `https://testnet.arbiscan.io`<br>`https://rinkeby-explorer.arbitrum.io` | Rinkeby       | Nitro Rollup       | `wss://rinkeby.arbitrum.io/feed`       | `snapshot.arbitrum.io/rinkeby/nitro.tar` | [retryable-dashboard.arbitrum.io](https://retryable-dashboard.arbitrum.io/) |
| Nitro Goerli Rollup Testnet^    | `https://goerli-rollup.arbitrum.io/rpc`                                                                                                          | 421613 | GoerliETH       | `https://goerli-rollup-explorer.arbitrum.io`                            | Goerli        | Nitro Rollup       | `wss://goerli-rollup.arbitrum.io/feed` | N/A                                      | [retryable-dashboard.arbitrum.io](https://retryable-dashboard.arbitrum.io/) |
</em>

^ Testnet

For a list of useful contract addresses, see [here](Useful_Addresses.md).

### Arbitrum Chains Summary

**Arbitrum One**: Arbitrum One is the flagship Arbitrum mainnet chain; it is an Optimistic Rollup chain running on top of Ethereum Mainnet, and is open to all users. In an upcoming upgrade, the Arbitrum One chain will be upgraded to use the [Nitro](https://medium.com/offchainlabs/its-nitro-time-86944693bf29) tech stack, maintaining the same state. (Stay tuned for updates!)
Users can now use [Alchemy](https://alchemy.com/?a=arbitrum-docs), [Infura](https://infura.io/), [QuickNode](https://www.quicknode.com), [Moralis](https://moralis.io/), [Ankr](https://www.ankr.com/), [BlockVision](https://blockvision.org/), and [GetBlock](https://getblock.io/) to interact with the Arbitrum One. See [node providers](Node_Providers.md) for the full guide. 

**Arbitrum Nova**: Arbitrum Nova is the first mainnet [AnyTrust](AnyTrust.md) chain.
Usres can now use [QuickNode](https://www.quicknode.com) to interact with the Arbitrum Nova chain. For a full guide of how to set up an Arbitrum node on QuickNode, see the QuickNode's Arbitrum RPC documentation.

**RinkArby**: RinkArby is the longest running Arbitrum testnet. It previously ran on the classic stack, but at block 7/28/2022 it was migrated use the Nitro stack! Rinkarby will be deprecated [when Rinkeby itself gets deprecated](https://blog.ethereum.org/2022/06/21/testnet-deprecation/); plan accordingly!
Users can now use [Alchemy](https://alchemy.com/?a=arbitrum-docs), [Infura](https://infura.io/), [QuickNode](https://www.quicknode.com), [Moralis](https://moralis.io/), [Ankr](https://www.ankr.com/), [BlockVision](https://blockvision.org/), and [GetBlock](https://getblock.io/) to interact with the Arbitrum One. See [node providers](Node_Providers.md) for the full guide. 

**Nitro Goerli Rollup Testnet**: This testnet (421613) uses the Nitro rollup tech stack; it is expected to be the primary, stable Arbitrum testnet moving forward.
Users can now use [Alchemy](https://alchemy.com/?a=arbitrum-docs), [Infura](https://infura.io/), and [QuickNode](https://www.quicknode.com) to interact with the Arbitrum One. See [node providers](Node_Providers.md) for the full guide. 

### Using Arbitrum

_**Note: before interacting with a mainnet chain, users should familiarize themselves with the risks; see [Mainnet Beta](Mainnet.md)**_.

#### Connect Your Wallet

Connect [your wallet](https://portal.arbitrum.one/#wallets) to an Arbitrum chain, adding the chain's RPC endpoint if required.

#### Get Some Native Currency

You'll need a chain's native currency to transact. You can either acquire funds directly on an Arbitrum chain, or get funds on a chain's underlying L1 and bridge it across. You can get testnet Ether from the following faucets:

- [Goerli](https://goerlifaucet.com/)
- [Rinkeby](https://faucet.rinkeby.io/)
- [Nitro Goerli Rollup](https://twitter.com/intent/tweet?text=ok%20I%20need%20@arbitrum%20to%20give%20me%20Nitro%20testnet%20gas.%20like%20VERY%20SOON.%20I%20cant%20take%20this,%20I%E2%80%99ve%20been%20waiting%20for%20@nitro_devnet%20release.%20I%20just%20want%20to%20start%20developing.%20but%20I%20need%20the%20gas%20IN%20MY%20WALLET%20NOW.%20can%20devs%20DO%20SOMETHING??%20%20SEND%20HERE:%200xAddA0B73Fe69a6E3e7c1072Bb9523105753e08f8)

[Supported centralized exchanges](https://portal.arbitrum.one/#centralizedexchanges) allow you to purchase (mainnet) Ether and withdraw it directly onto Arbitrum one.

#### Deposit And Withdraw

To move your Ether and Tokens between Arbitrum and Ethereum chains, visit [bridge.arbitrum.io](https://bridge.arbitrum.io/).

#### Use L2 Dapps!

Interacting with Arbitrum chains will feel very similar to using Ethereum, just cheaper and faster! To get a sense of what's out there, you can check out our [portal page](https://portal.arbitrum.one/), where we showcase some of the dApps, wallets, and infrastructure currently live on Arbitrum One.

#### Build on Arbitrum

Dapp developers can build on Arbitrum seamlessly using their favorite Ethereum tooling; see [here](Contract_Deployment.md) for contract deployment and [here](Frontend_Integration.md) for frontend integration.

#### What's Next

The team working on Arbitrum is always interested and looking forward to engage with its users.
Why not follow us on [Twitter](https://twitter.com/arbitrum) or join our community on [Discord](https://discord.gg/5KE54JwyTs)?
