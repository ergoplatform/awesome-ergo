
# dApps
- [sigmaverse.io](https://sigmaverse.io/) - *your portal to the Ergo Universe*
- [ErgoFaucet.org](https://github.com/zargarzadehm/ergo-faucet)

## Tokenisation

This service will provide a way for dapps to distribute gains among dapps' token holders.

The first user of this service will be the ErgoMixer. 

Ergomixer's income (in ERG and other tokens) is currently received by its creator, aka 'anon2020s', since it has only one stakeholder at the moment. He has announced that he is willing to create and sell some tokens in the near future to obtain more stakeholders; let's call this token MIX. later, anyone having the MIX tokens can stake these tokens in the Profit Sharing contract and obtain the mixer's incomes proportional to their staked tokens.

So, it is NOT a way to stake ERG at first. But, it CAN BE USED in the future in some creative services to provide ERG-staking.

- [A solution for staking](https://www.ergoforum.org/t/a-solution-for-staking/1057)
- [Ergo Profit Sharing dApp](https://github.com/mhssamadani/ErgoProfitSharingDapp)


# ErgoMixer

[ErgoMixer](https://github.com/ergoMixer/ergoMixBack) is the first working non-custodial, programmable, non-interactive mixer in the cryptocurrency space. 

**Resources**
- Technical Slides: [ZeroJoin: Combining Zerocoin and Coinjoin](https://ergoplatform.org/docs/CBT_2020_ZeroJoin_Combining_Zerocoin_and_CoinJoin_v3.pdf)
- [Video tutorial](https://www.youtube.com/watch?v=03_2HH82Plw)



# ErgoAuctions

The [Ergo Auction House](http://ergoauctions.org/#/auction/active) lets you buy and sell collectible tokens, art and much more.

- [Source code](https://github.com/anon-real/ErgoAuctionHouse)
- [v2 contracts](https://github.com/ergoplatform/eips/pull/39/files)
- More information available at [ergonaut.space/en/ErgoAuctions](https://ergonaut.space/en/ErgoAuctions)

# Stablecoins

## SigmaUSD
> The first UTxO-based stable coin - an instantiation of the [AgeUSD protocol](https://github.com/Emurgo/age-usd). Its economic model designed in partnership between IOHK, Ergo, and Emurgo maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup.

The UI for the front-end is available at [anon-real/sigma-usd](https://github.com/anon-real/sigma-usd) 

**Resources**
- [Ergo Summit 2021 - The IOHK Perspective - Designing the AgeUSD StableCoin](https://youtu.be/zG-rxMCDIa0?t=9247)
- [Overview Video (with diagrams)](https://www.youtube.com/watch?v=O3hPEp3tzoU)
- [Building Ergo: How the AgeUSD stablecoin works](https://ergoplatform.org/en/blog/2021-02-05-building-ergo-how-the-ageusd-stablecoin-works/)

## Dexy

- [Dexy: USD Simplest Stablecoin](https://www.ergoforum.org/t/dexy-usd-simplest-stablecoin-design/1430
)
# ErgoDex

The [ErgoLabs](https://github.com/ergolabs) contains all the related code for ErgoDex


- [EIP-0014: Decentalized Exchange Contracts](https://github.com/ergoplatform/eips/pull/27)
- [Single-Chain Swap Contracts (DEX basis) by Alex Chepurnoy](https://www.youtube.com/watch)


# Oracles

See this [overview](https://github.com/Emurgo/Emurgo-Research/blob/master/oracles/Oracle-Pools.md) by Robert Kornacki.


When external oracle data is posted on-chain, it needs to be encoded in a very precise way within a transaction. Furthermore, oracle pools have a bunch of different moving parts which require transactions to be issued to move between the different stages of the pool protocol. [Oracle Core](https://github.com/ergoplatform/oracle-core) creates all of the complex transactions which posts the data on-chain & runs the oracle pool protocol on-chain (such as averaging datapoints). This comes bundled with [Oracle Pool Bootstrap](https://github.com/ergoplatform/oracle-core/tree/master/oracle-pool-bootstrap) and a [Connector Library](https://github.com/ergoplatform/oracle-core/tree/master/connectors/connector-lib). The [ada-usd-oracle](https://github.com/ergoplatform/oracle-core/blob/master/scripts/ada-usd-oracle/oracle-config.yaml) source can be seen here. Currently only the erg-usd-oracle is live as seen in the [Oracle Pool List](https://explorer.ergoplatform.com/en/oracle-pools-list)


## v2
- [Oracle pool 2.0 contracts finalized (for initial draft).](https://github.com/ergoplatform/eips/blob/eip23/eip-0023.md)
- [Tests for oracle pool 2.0](https://github.com/scalahub/OraclePool/tree/v2/src/test/scala/oraclepool/v2)


**Resources**
- [eth/usd connector](https://github.com/Luivatra/oracle-core/tree/eth-connector)
- [Ergo oracles](https://github.com/sininen-taivas/ergo-oracle) - simple command-line tool to launch oracles. Inbuilt implementations for USD/ERG, EUR/ERG, BTC/ERG, AUG/ERG (gold) prices delivery. 
- Learn about data inputs and the truly novel innovations they bring to UTXO-based Blockchains like #Cardano by reading our latest research [here](https://github.com/Emurgo/Emurgo-Research/blob/master/smart-contracts/Unlocking%20The%20Potential%20Of%20The%20UTXO%20Model.md)
 - [Ergo oracles](https://github.com/sininen-taivas/ergo-oracle) - simple command-line tool to launch oracles. Inbuilt implementations for USD/ERG, EUR/ERG, BTC/ERG, AUG/ERG (gold) prices delivery. See also a [forum topic with example](https://www.ergoforum.org/t/erg-usd-oracle-on-top-of-ergo/119)


**Articles**
- [Chainlink Oracles vs. Ergo Oracle Pools](https://ergoplatform.org/en/blog/2021-04-27-chainlink-oracles-vs-ergo-oracle-pools/)
- [Oracle Pools - A New Oracle Model](https://www.ergoforum.org/t/oracle-pools-a-new-oracle-model/263)
- [First steps towards interoperability with Cardano oracles](https://ergoplatform.org/en/blog/2020-11-09-first-steps-towards-interoperability-with-cardano-oracles/)
- [Ergo Blockchain: Oracle Pool Governance Update](https://curiaregiscrypto.medium.com/ergo-blockchain-oracle-pool-governance-update-d078d58571b0)
- [The role of Ergo Oracles](https://veriumfellow.medium.com/oracle-special-4e36cfa6a852)

# ErgoFund

- [Ergo Crowdfunding CLI](https://github.com/robkorn/ergo-crowdfunding-cli) | Command-line tool which enables participating and interacting with crowdfunding campaigns on Ergo
- [Scanner](https://github.com/ergoplatform/scanner) 
- ZK Treasury |  a tool for joint spendings with on-chain privacy 
  - [Server](https://github.com/anon-real/DistributedSigsServer) 
  - [Client](https://github.com/anon-real/DistributedSigsClient)
- 'A Collective Spending Appproach' | In development, [more details](https://www.reddit.com/r/ergonauts/comments/ohftim/ergoteam_a_simpler_collective_spending_approach/)


# ErgoLend
- [ErgoLend](https://github.com/Ergo-Lend/)

# ErgoRaffle

- [ErgoRaffle](https://github.com/ErgoRaffle)

# Many more possible!
- [Bonds based on Ergo (or the “Yield protocol”)](https://www.ergoforum.org/t/bonds-based-on-ergo-or-the-yield-protocol/128)
- [An ICO Example On Top Of Ergo](https://github.com/ergoplatform/ergo/wiki/An-ICO-Example-On-Top-Of-Ergo)
- [A Local Exchange Trading System On Top Of Ergo](https://github.com/ergoplatform/ergo/wiki/A-Local-Exchange-Trading-System-On-Top-Of-Ergo)
- [A Trustless Local Exchange Trading System](https://github.com/ergoplatform/ergo/wiki/A-Trustless-Local-Exchange-Trading-System)
- [(E)mail Client for Limited or Blocked Internet](https://www.ergoforum.org/t/e-mail-client-for-limited-or-blocked-internet/134)
- [LETS start the discussion](https://ergoplatform.org/en/blog/2021-07-01-lets-start-the-discussion/)
- ErgoFans | Decentralised content producer platform | Patreon/Onlyfans
- ErgoGigs | Decentralised gigs! (Fiverr)
- ErgoEarn | earn for learning (Coinbase Earn)
- ErgoStats | on-chain analysis (glassnode)