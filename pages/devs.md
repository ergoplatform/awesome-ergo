- [Developers](#developers)
  - [Hackathons](#hackathons)
  - [Resources](#resources)
- [GitHubs](#githubs)
  - [Devs](#devs)
  - [Resources](#resources-1)
- [Future applications](#future-applications)
- [ErgoScript](#ergoscript)
- [Contracts and Scripts](#contracts-and-scripts)
- [Tools and Libraries](#tools-and-libraries)
- [Appkit](#appkit)
- [Sigmastate-Interpreter](#sigmastate-interpreter)
  - [Rust](#rust)
- [JS/TS](#jsts)
- [Resources](#resources-2)
  - [Services](#services)
- [Ergo Bootstrap](#ergo-bootstrap)
- [Misc](#misc)
- [Existing Applications](#existing-applications)
    - [Oracle Pools](#oracle-pools)
    - [ErgoMixer](#ergomixer)
    - [ErgoAuctions](#ergoauctions)
    - [SigmaUSD](#sigmausd)
    - [ErgoDex](#ergodex)
    - [ErgoFund](#ergofund)

# Developers



## Hackathons

- May (Completed) - see [ErgoHack](https://ergoplatform.org/en/blog/2021-06-19-ergohack/)
- September (TBC)

## Resources

- Using [Ergo-TestNet](https://github.com/ergoplatform/ergo/wiki/Ergo-Testnet)
- [Building Ergo: Developer Tools](https://ergoplatform.org/en/blog/2021-06-10-building-ergo-developer-tools/)
- [Building Ergo: ErgoScript](https://ergoplatform.org/en/blog/2021-06-09-building-ergo-ergoscript/)
- [LETS start the discussion](https://ergoplatform.org/en/blog/2021-07-01-lets-start-the-discussion/)

# GitHubs
- [ergoplatform](https://github.com/ergoplatform/) | Ergo protocol description & reference client implementation.
- [ergolabs](https://github.com/ergolabs) | ErgoDex
- [Emurgo](https://github.com/Emurgo/) | AgeUSD, Oracle Pools, Yoroi

## Devs

- [scalahub](https://github.com/scalahub/) | AppKit
- [mhssamadani](https://github.com/mhssamadani/) | gravity-core
- [anon-real](https://github.com/anon-real) | SigmaUSD

## Resources
- [ErgoWiki](https://github.com/ergoplatform/ergo/wiki)
- [ScorexFoundation](https://github.com/ScorexFoundation/)
- [/r/ergonauts - FAQ](https://www.reddit.com/r/ergonauts/wiki/faq)
# Future applications

See the [Ergo: Decentralized Applications Framework](https://ergoplatform.org/en/blog/2021-07-02-ergo-decentralized-applications-framework/) articles on the ergo blog for an overview of what's possible on Ergo

- [Bonds based on Ergo (or the “Yield protocol”)](https://www.ergoforum.org/t/bonds-based-on-ergo-or-the-yield-protocol/128)
- [An ICO Example On Top Of Ergo](https://github.com/ergoplatform/ergo/wiki/An-ICO-Example-On-Top-Of-Ergo)
- [A Local Exchange Trading System On Top Of Ergo](https://github.com/ergoplatform/ergo/wiki/A-Local-Exchange-Trading-System-On-Top-Of-Ergo)
- [A Trustless Local Exchange Trading System](https://github.com/ergoplatform/ergo/wiki/A-Trustless-Local-Exchange-Trading-System)
- [(E)mail Client for Limited or Blocked Internet](https://www.ergoforum.org/t/e-mail-client-for-limited-or-blocked-internet/134)

Loads more on [ergoforum: research & development](https://www.ergoforum.org/c/research-and-development/7?order=views)


# ErgoScript

Learn [Ergoscript by reading example smart contracts](https://github.com/ergoplatform/ergoscript-by-example) powered by the Ergo Playground. Each contract example includes a `Ergo Playground` link which allows you to instantly edit and run the smart contract code inside of your browser.

- If you ever need clarity about how specific types/functions/operators in ErgoScript work, please reference the [ErgoScript Language Description](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md).
- For an overarching summary, please reference this [video](https://www.youtube.com/watch?v=8l2v1asHgyA)
- [A Quick Primer on ErgoScript](https://github.com/ergoplatform/ergo/wiki/ErgoScript-Overview) Learn the basics of ErgoScript quickly and create your first contract
- [ErgoScript Design patterns](https://www.ergoforum.org/t/ergoscript-design-patterns/222)
- [ErgoScript, a Cryptocurrency Scripting Language Supporting Noninteractive Zero-Knowledge Proofs](https://ergoplatform.org/docs/ErgoScript.pdf)
- [Advanced ErgoScript Tutorial](https://ergoplatform.org/docs/AdvancedErgoScriptTutorial.pdf)
- [ErgoScript advanced tutorial]( https://docs.ergoplatform.com/sigmastate_protocols.pdf)

- [Learn ErgoScript By Example Via The Ergo Playground with Robert Kornacki](https://www.youtube.com/watch?v=8l2v1asHgyA)
# Contracts and Scripts 
 - [ErgoScript tutorial](https://ergoplatform.org/docs/ErgoScript.pdf) - describes an Ergo Scripting Language supporting Noninteractive Zero-Knowledge Proofs
 - [ErgoScript by Example](https://github.com/ergoplatform/ergoscript-by-example) - repository with ErgoScript examples you can play with in Ergo Playground 
 - [A Quick Primer on ErgoScript](https://github.com/ergoplatform/ergo/wiki/ErgoScript-Overview) Learn the basics of ErgoScript quickly and create your first contract
 - [Ergo notary](https://github.com/sininen-taivas/ergo-notary) - simple command-line tool to certificate files on the Ergo blockchain. 
 See also [forum topic](https://www.ergoforum.org/t/ergo-notary-command-line-tool/75) on a particular example
 - [Ergo oracles](https://github.com/sininen-taivas/ergo-oracle) - simple command-line tool to launch oracles. Inbuilt implementations for USD/ERG, EUR/ERG, BTC/ERG, AUG/ERG (gold) prices delivery. See also a [forum topic with example](https://www.ergoforum.org/t/erg-usd-oracle-on-top-of-ergo/119)
 - [Ergo Crowdfunding CLI](https://github.com/robkorn/ergo-crowdfunding-cli) Command-line tool which enables participating and interacting with crowdfunding campaigns on Ergo 
 - [Miner rewards script](https://github.com/lorien/ergotools) Simple command-line tool to find miner rewards not spent and form withdrawing transaction requests for them

# Tools and Libraries
 - [Sigma-Rust](https://github.com/ergoplatform/sigma-rust/) - Alternative and simple implementation of ErgoTree interpreter and transaction building tools
 - [Ergo Utilities](https://github.com/robkorn/ergo-utilities-rust/) - General utilities to make writing off-chain Ergo code in Rust simpler 
 - [Ergo Appkit](https://github.com/aslesarenko/ergo-appkit) - Appkit is a Java7/Java8A Library for Development of Ergo Applications (also supports [GraalVM](https://www.graalvm.org/), Android and JavaFX)
 - [ergo-ts (TypeScript)](https://github.com/coinbarn/ergo-ts)
 - [ergo-js (JavaScript)](https://github.com/ergoplatform/ergo-js) 
 - [Kiosk](https://github.com/scalahub/Kiosk) - interface to Ergo node with additional features for a developer. See this [forum post](https://www.ergoforum.org/t/ergoscript-playground-using-kiosk/96) about particular example 
 - [Appkit Examples](https://github.com/aslesarenko/ergo-appkit-examples) - Examples of using Ergo Appkit for Polyglot Development of Ergo Applications
 - [Ergo Android](https://github.com/aslesarenko/ergo-android) - Example Android application which uses [Appkit](https://github.com/aslesarenko/ergo-appkit)
 - [ErgoTool](https://github.com/aslesarenko/ergo-tool) - A Command Line Interface for Ergo based on Appkit and [GraalVM native-image](https://www.graalvm.org/examples/native-image-examples/)
 - [Ergo P2S Playground](https://wallet.plutomonkey.com/p2s/?source=dHJ1ZQ==) - A web-based tool to quickly get the address corresponding to some script  

# Appkit

Appkit has idiomatic Java API and is written in Java/Scala. It is a thin wrapper around core components provided by ErgoScript interpreter and Ergo protocol implementations which are written in Scala. It is [published](https://mvnrepository.com/artifact/org.ergoplatform/ergo-appkit) on maven repository and cross compiled to both Java 7 and Java 8+ jars.

The Appkit library is compatible with GraalVM - a novel next generation approach to implement software which is reusable across several programming languages and execution environments. For example if Node.js application is run on GraalVM, then it can use Appkit to interact with Ergo Blockchain.

Using Appkit Ergo applications can be written in one of the languages supported by GraalVM (i.e. Java, JavaScript, C/C++, Python, Ruby, R) and using this library applications can communicate with Ergo nodes via unified API and programming model provided by Appkit. In addition Appkit based Ergo applications can be compiled into native code using native-image ahead of time compiler and then executed without Java VM with very fast startup time and lower runtime memory overhead compared to a Java VM. This is attractive option for high-performance low-latency microservices.

In addition Appkit is compatible with Android and can be used from Android applications.

**Resources**
- [Ergo Appkit (Polyglot library)](https://github.com/aslesarenko/ergo-appkit) - Appkit: A Library for Polyglot Development of Ergo Applications using either [GraalVM](https://www.graalvm.org/) or stock Java 1.7 and above. Read the [introduction](https://ergoplatform.org/en/blog/2019_12_03_top5/).
- [Appkit Examples](https://github.com/aslesarenko/ergo-appkit-examples) - Examples of using Ergo Appkit for Polyglot Development of Ergo Applications
- [ErgoTool](https://github.com/aslesarenko/ergo-tool) - A Command Line Interface for Ergo based on Appkit and [GraalVM](https://www.graalvm.org/) native-image. Read the [introduction and overview](https://ergoplatform.org/en/blog/2019_12_31_ergo_tool/).
- [Ergo Android](https://github.com/aslesarenko/ergo-android) - Example Android application which demonstrates how Ergo Appkit can be used to develop Ergo applications running on Android.
- [Multi-Stage Contracts in the UTXO Model: Delivery by Alexander Chepurnoy & Amitabh Saxena](https://www.youtube.com/watch?v=g3FlM_WOwBU)


# Sigmastate-Interpreter

Interpreter for a family of Sigma-State authentication languages, [a list of good first issues is available on Github](https://github.com/ScorexFoundation/sigmastate-interpreter/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22)


- Smart contract language: https://github.com/ScorexFoundation/sigmastate-interpreter
- [ScoreX](https://github.com/scorexfoundation/scorex), The modular blockchain framework
- Basic cryptography library: https://github.com/input-output-hk/scrypto

## Rust
sigma-rust is an alternative and simple implementation of ErgoTree interpreter and transaction building tools. The goal for the Rust version is to be on par with Scala version feature-wise. Now Rust version is still significantly behind. Also the goal for the Rust version is to have bindings for web, iOS and Android. The Scala version will continue to be the primary choice for JVM ecosystem with Rust version covering the rest.

[sigma-rust](https://github.com/ergoplatform/sigma-rust) - implementation of ErgoScript cryptocurrency scripting language. To get better understanding on how to use it in your project check out how its being used in the following projects:

- [Ergo Headless dApp Framework](https://github.com/Emurgo/ergo-headless-dapp-framework);
- [Ergo Node Interface Library](https://github.com/Emurgo/ergo-node-interface);
- [Oracle Core](https://github.com/ergoplatform/oracle-core);
- [AgeUSD Stablecoin Protocol](https://github.com/Emurgo/age-usd);
- [Yoroi wallet](https://github.com/Emurgo/yoroi-frontend) (WASM bindings);
- [Ergo Desktop Wallet](https://github.com/ErgoWallet/ergowallet-desktop) (WASM bindings);
- [Ergo Utilities](https://github.com/robkorn/ergo-utilities-rust/) - General utilities to make writing off-chain Ergo code in Rust simpler 


> A list of "*good first*" issues for Sigma-Rust is [available on GitHub](https://github.com/ergoplatform/sigma-rust/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) - @greenhat on [Discord](https://discord.gg/Q86PNMwRsu) is ready to assist anyone who is interested.




# JS/TS

 - [ergo-ts (TypeScript)](https://github.com/coinbarn/ergo-ts) with support of tokens and complex transactions
 - [ergo-js (JavaScript)](https://github.com/ergoplatform/ergo-js) with basic transaction operations
 - [Ergo JS Template](https://github.com/anon-real/ergo-js-template)


# Resources
## Services
- [Mainnet explorer](https://explorer.ergoplatform.com/)
- [Testnet explorer](https://testnet.ergoplatform.com/) 
- [Node API](https://git.io/fjqwb)
- [Explorer API](https://git.io/fjqwN)
- [API Docs](https://api.ergoplatform.com/api/v1/docs/)
- [Ergo Addresses](https://ergoplatform.org/en/blog/2019_07_24_ergo_address/)
- [Ergo terminology: a Box and a Register](https://www.ergoforum.org/t/ergo-terminology-a-box-and-a-register/32)



# Ergo Bootstrap
The Ergo ecosystem is quickly growing with new design patterns, tools, dApps, and more every single month. This is an exciting point in time for developers to jump in and get started.

That said, while building dApps on top of Ergo, vital infrastructure components to develop and run your dApp might be intimidating to set up for someone who is unfamiliar with the existing tooling. Between an Ergo full node, explorer back end, explorer front end, logging, and metrics, it can become quite overwhelming for a nascent dApp developer entering into the ecosystem.

For this reason, we are introducing [ergo-bootstrap](https://github.com/ergoplatform/ergo-bootstrap), an easy-to-use tool that enables quick and clean Ergo blockchain cluster deployments which supports a variety of useful infrastructure components you will need on your path of dApp development. This was developed by Marek of Five Binaries thanks to a grant given by the Ergo Foundation and their latest push to empower the ecosystem via funding key projects.

Ergo bootstrap tool, build on top of ergo-nix, will help you to quickly deploy an Ergo blockchain cluster with a handful of useful tools you might need to start developing your dApps.

Read more on the blog - [Ergo Bootstrap, Streamlining Ergo dApp Infrastructure With One Simple Tool](https://ergoplatform.org/en/blog/2020-12-11-ergo-bootstrap-streamlining-ergo-dapp-infrastructure-with-one-simple-tool/)

# Misc

**Utilities**
- [Ergo notary](https://github.com/sininen-taivas/ergo-notary) - simple command-line tool to certificate files on the Ergo blockchain. See also [forum topic](https://www.ergoforum.org/t/ergo-notary-command-line-tool/75) on a particular example
 - [ErgoTool](https://github.com/aslesarenko/ergo-tool) - A Command Line Interface for Ergo based on Appkit and [GraalVM](https://www.graalvm.org/)
- [Kiosk](https://github.com/scalahub/Kiosk) - interface to Ergo node with additional features for a developer. See this [forum post](https://www.ergoforum.org/t/ergoscript-playground-using-kiosk/96) about particular example 
- [Ergo Utilities](https://github.com/robkorn/ergo-utilities-rust/) - General utilities to make writing off-chain Ergo code in Rust simpler. 
- [JSON dApp Environment (JDE) first release](https://www.ergoforum.org/t/json-dapp-environment-jde-first-release/1373)


 **Test vectors:**
- [Ergo transaction serialization](https://git.io/fjqwX)
- [Signature scheme](https://git.io/fjqwH)




# Existing Applications
> [sigmaverse](sigmaverse.io/) - Your portal to the Ergo Universe

### Oracle Pools
- [Oracle Core](https://github.com/ergoplatform/oracle-core) - Run your oracle pools!
- [Ergo oracles](https://github.com/sininen-taivas/ergo-oracle) - simple command-line tool to launch oracles. Inbuilt implementations for USD/ERG, EUR/ERG, BTC/ERG, AUG/ERG (gold) prices delivery. 
- [Oracle Pool List](https://explorer.ergoplatform.com/en/oracle-pools-list)


**Articles**
- [Emurgo Research: Oracle Pools](https://github.com/Emurgo/Emurgo-Research/blob/master/oracles/Oracle-Pools.md)
- [Chainlink Oracles vs. Ergo Oracle Pools](https://ergoplatform.org/en/blog/2021-04-27-chainlink-oracles-vs-ergo-oracle-pools/)
- [Oracle Pools - A New Oracle Model](https://www.ergoforum.org/t/oracle-pools-a-new-oracle-model/263)
- [First steps towards interoperability with Cardano oracles](https://ergoplatform.org/en/blog/2020-11-09-first-steps-towards-interoperability-with-cardano-oracles/)
- [Ergo Blockchain: Oracle Pool Governance Update](https://curiaregiscrypto.medium.com/ergo-blockchain-oracle-pool-governance-update-d078d58571b0)
- [The role of Ergo Oracles](https://veriumfellow.medium.com/oracle-special-4e36cfa6a852)

### ErgoMixer

> The first working non-custodial, programmable, non-interactive mixer in the cryptocurrency space. 


There have been requests from the community to understand the mixer, why it is an important piece of tech, and why people would choose to use it. 

- [ErgoMixer ELI5](https://ergoplatform.org/en/blog/2021-05-12-ergomixer/)
- [Ergo: What are *'Mixers'* ?](https://ergoplatform.org/en/blog/2021-05-19-ergo-what-are-bitcoin-mixers/)
- [ErgoMixer](https://github.com/ergoMixer/ergoMixBack) -  [Video tutorial #1](https://www.youtube.com/watch?v=03_2HH82Plw)
- [A solution for staking](https://www.ergoforum.org/t/a-solution-for-staking/1057)
- [ZeroJoin: Combining Zerocoin and Coinjoin](https://ergoplatform.org/docs/CBT_2020_ZeroJoin_Combining_Zerocoin_and_CoinJoin_v3.pdf)

### ErgoAuctions
- [Ergo Auctions House](http://ergoauctions.org/#/auction/active) - Buy and sell collectible tokens and more [Source code](https://github.com/anon-real/ErgoAuctionHouse)
- [ergonaut.space/en/ErgoAuctions](https://ergonaut.space/en/ErgoAuctions)

### SigmaUSD
> The first UTxO-based stable coin - an instantiation of the [AgeUSD protocol](https://github.com/Emurgo/age-usd). Its economic model designed in partnership between IOHK, Ergo, and Emurgo maintains the conservative settings for collateral reserves and avoids the need for liquidations. Along with that, it supports a fully decentralised stablecoin emission setup.

- [anon-real/sigma-usd](https://github.com/anon-real/sigma-usd) 

**Resources**
- [Ergo Summit 2021 - The IOHK Perspective - Designing the AgeUSD StableCoin](https://youtu.be/zG-rxMCDIa0?t=9247)
- [Overview Video (with diagrams)](https://www.youtube.com/watch?v=O3hPEp3tzoU)
- [Building Ergo: How the AgeUSD stablecoin works](https://ergoplatform.org/en/blog/2021-02-05-building-ergo-how-the-ageusd-stablecoin-works/)
- [Emurgo announcement blog post](https://ergoplatform.org/en/blog/2021_02_26-sigmausd-released/)
- [Finding The Right Balance](https://ergoplatform.org/en/blog/2021_03_04-finding-right-balance/)
    - [Community Discussion on Reddit](https://www.reddit.com/r/ergonauts/comments/lx7an4/sigmausd_dao_bank_is_a_complex_beast_highlevel/gpr96fq/?context=3)
- [SigmaUSD (v1) Release](https://ergoplatform.org/en/blog/2021_02_26-sigmausd-released/)
 
### ErgoDex
- [ErgoDex](https://github.com/ergolabs) 
- [EIP-0014: Decentalized Exchange Contracts](https://github.com/ergoplatform/eips/pull/27)
- [Single-Chain Swap Contracts (DEX basis) by Alex Chepurnoy](https://www.youtube.com/watch?v=Wn_w9F_MX8w)

### ErgoFund
- [Ergo Crowdfunding CLI](https://github.com/robkorn/ergo-crowdfunding-cli) Command-line tool which enables participating and interacting with crowdfunding campaigns on Ergo
- [Scanner](https://github.com/ergoplatform/scanner)
- ZK Treasury: [Server](https://github.com/anon-real/DistributedSigsServer) and [Client](https://github.com/anon-real/DistributedSigsClient) - a tool for joint spendings with on-chain privacy 
