- [Developers](#developers)
  - [Other Pages](#other-pages)
  - [Hackathons](#hackathons)
  - [Resources](#resources)
- [Software Development Kit](#software-development-kit)
  - [Appkit](#appkit)
- [Sigma Language](#sigma-language)
  - [ErgoScript](#ergoscript)
  - [Languages](#languages)
    - [Scala](#scala)
    - [Rust](#rust)
    - [JS/TS](#jsts)
    - [C](#c)
- [Tools, Services & Resources](#tools-services--resources)
  - [Services](#services)
  - [Utilities](#utilities)
  - [Tools](#tools)
  - [Articles](#articles)
# Developers 

This page provides a curated page of resources for developers. Please submit a PR if anything is missing!

For most developers, [Appkit](#appkit) is the best entry point unless you're wanting to dive straight into [ErgoScript](#ergoscript).

# Resources
- [ErgoWiki](https://github.com/ergoplatform/ergo/wiki) | The official ergoplatform GitHub wiki
- [r/ergonauts/wiki](https://www.reddit.com/r/ergonauts/wiki/index) | Community Wiki
- [ergosites.github.io](https://ergosites.github.io/) | Resource page which links to various websites and utilities. 
- [ergohack.io/resources](https://ergohack.io/resources)

## Other Pages

- See this resource page on [ergohack.io](https://ergohack.io/resources)
- See [wallets.md](/wallets.md) for developer resources within that area
- See [apps.md](/apps.md) for developer resources relating to Oracles, Ergo Auctions, SigmaUSD, or any existing applications built ontop Ergo.
- [Documentation](pages/docs.md) | Whitepapers

## ERGOHACK


- [ERGOHACK I](https://ergoplatform.org/en/blog/2021-06-19-ergohack/) (May, 2021)
- ERGOHACK II (Oct 8-10, 2021)
- Q1 2022 (TBC)

Join the [Discord](https://discord.gg/qxdrHM2eHv) to participate. 
**GitHubs**
- [ergoplatform](https://github.com/ergoplatform/) | Ergo protocol description & reference client implementation.
- [Emurgo](https://github.com/Emurgo/) | AgeUSD, Oracle Pools, Yoroi
- [ScorexFoundation](https://github.com/ScorexFoundation/)

# Software Development Kit
## Appkit

[Appkit: A Library for Polyglot Development of Ergo Applications](https://github.com/aslesarenko/ergo-appkit) has idiomatic Java API and is written in Java/Scala. It is a thin wrapper around core components provided by ErgoScript interpreter and Ergo protocol implementations which are written in Scala. It is published on [maven repository](https://mvnrepository.com/artifact/org.ergoplatform/ergo-appkit)) and cross compiled to both Java 7 and Java 8+ jars.

The Appkit library is also compatible with [GraalVM](https://www.graalvm.org/) - a novel next generation approach to implement software which is reusable across several programming languages and execution environments. For example if Node.js application is run on GraalVM, then it can use Appkit to interact with Ergo Blockchain.

Using Appkit Ergo applications can be written in one of the languages supported by GraalVM (i.e. Java, JavaScript, C/C++, Python, Ruby, R) and using this library applications can communicate with Ergo nodes via unified API and programming model provided by Appkit. In addition Appkit based Ergo applications can be compiled into native code using native-image ahead of time compiler and then executed without Java VM with very fast startup time and lower runtime memory overhead compared to a Java VM. This is attractive option for high-performance low-latency microservices.

**Resources**
- [Ergo Appkit (Polyglot library)](https://github.com/aslesarenko/ergo-appkit) - Appkit: A Library for Polyglot Development of Ergo Applications using either [GraalVM](https://www.graalvm.org/) or stock Java 1.7 and above. Read the [introduction](https://ergoplatform.org/en/blog/2019_12_03_top5/).
- [Appkit Examples](https://github.com/aslesarenko/ergo-appkit-examples) - Examples of using Ergo Appkit for Polyglot Development of Ergo Applications
- [ErgoTool](https://github.com/aslesarenko/ergo-tool) - A Command Line Interface for Ergo based on Appkit and [GraalVM](https://www.graalvm.org/) native-image. Read the [introduction and overview](https://ergoplatform.org/en/blog/2019_12_31_ergo_tool/).
- [Ergo Android](https://github.com/aslesarenko/ergo-android) - Example Android application which demonstrates how Ergo Appkit can be used to develop Ergo applications running on Android.
- [Multi-Stage Contracts in the UTXO Model: Delivery by Alexander Chepurnoy & Amitabh Saxena](https://www.youtube.com/watch?v=g3FlM_WOwBU)


# ErgoScript

> [ErgoScript, a Cryptocurrency Scripting Language Supporting Noninteractive Zero-Knowledge Proofs](https://ergoplatform.org/docs/ErgoScript.pdf)

Learn [Ergoscript by reading example smart contracts](https://github.com/ergoplatform/ergoscript-by-example) powered by the Ergo Playground. Each contract example includes a link which allows you to instantly edit and run the smart contract code inside of your browser.

If you ever need clarity about how specific types/functions/operators in ErgoScript work, please reference the [ErgoScript Language Description](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md). For an overarching summary, please reference this [video](https://www.youtube.com/watch?v=8l2v1asHgyA)

Learn the basics of ErgoScript quickly and create your first contract

- [A Quick Primer on ErgoScript](https://github.com/ergoplatform/ergo/wiki/ErgoScript-Overview) 
- [ErgoScript tutorial](https://ergoplatform.org/docs/ErgoScript.pdf) | describes an Ergo Scripting Language supporting Noninteractive Zero-Knowledge Proofs
- [ErgoScript Design patterns](https://www.ergoforum.org/t/ergoscript-design-patterns/222)
- [Advanced ErgoScript Tutorial](https://ergoplatform.org/docs/AdvancedErgoScriptTutorial.pdf)
- [SigmaState Protocols](https://docs.ergoplatform.com/sigmastate_protocols.pdf)
- [(Video) Learn ErgoScript By Example Via The Ergo Playground with Robert Kornacki](https://www.youtube.com/watch?v=8l2v1asHgyA)
- [Building Ergo: ErgoScript](https://ergoplatform.org/en/blog/2021-06-09-building-ergo-ergoscript/)
- [Multi-Stage Contracts in the UTXO Model: Delivery by Alexander Chepurnoy & Amitabh Saxena](https://www.youtube.com/watch?v=g3FlM_WOwBU)


## Languages
### Scala

- [Sigmastate-Interpreter](https://github.com/ScorexFoundation/sigmastate-interpreter) | The Sigmastate-Interpreter is a ErgoScript compiler and ErgoTree Interpreter implementation for Ergo blockchain's *Sigma Language*  For development of Ergo applications using JVM languages a better alternative is to use [Appkit](#appkit).
- [ScoreX](https://github.com/scorexfoundation/scorex), the open-source, modular blockchain & cryptocurrency framework.
- [Scrypto](https://github.com/input-output-hk/scrypto) | Scrypto is an open source cryptographic toolkit designed to make it easier and safer for developers to use cryptography in their applications based on Scorex

This library is used internally in [Ergo Node](https://github.com/ergoplatform/ergo) and [ergo-wallet](https://github.com/ergoplatform/ergo/tree/master/ergo-wallet), the public interfaces are subject to change.

### Rust

[sigma-rust](https://github.com/ergoplatform/sigma-rust)  is an alternative and simple implementation of ErgoTree interpreter and transaction building tools. The goal for the Rust version is to be on par with Scala version feature-wise. At the moment, the Rust version is still significantly behind. Also the goal for the Rust version is to have bindings for web, iOS and Android. The Scala version will continue to be the primary choice for JVM ecosystem with Rust version covering the rest. To get better understanding on how to use it in your project check see [Usage Examples](https://github.com/ergoplatform/sigma-rust#usage-examples)

> A list of "*good first*" issues for Sigma-Rust is [available on GitHub](https://github.com/ergoplatform/sigma-rust/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) - @greenhat on [Discord](https://discord.gg/Q86PNMwRsu) is ready to assist anyone who is interested.

### JS/TS

 - [ergo-ts (TypeScript)](https://github.com/coinbarn/ergo-ts) with support of tokens and complex transactions
 - [ergo-js (JavaScript)](https://github.com/ergoplatform/ergo-js) with basic transaction operations
 - [Ergo JS Template](https://github.com/anon-real/ergo-js-template)

### C#

There is a great video series by Razor-sharp Solution | [Ergo with C# 101](https://www.youtube.com/watch?v=aUuki-fAxwc&list=PLUWruihtE-HtL-JZk8Vb4Yn_H18aE3rb6)

Stay tuned - A C# interpreter, cross-platform wallet, management and miner platform is in development!



  

# Sigmastate-Interpreter

Interpreter for a family of Sigma-State authentication languages.

- Smart contract language: [sigmastate-interpreter](https://github.com/ScorexFoundation/sigmastate-interpreter)
- [ScoreX](https://github.com/scorexfoundation/scorex), The modular blockchain framework
- Basic cryptography library: [scrypto](https://github.com/input-output-hk/scrypto)

## Rust
> [sigma-rust](https://github.com/ergoplatform/sigma-rust) - implementation of ErgoScript cryptocurrency scripting language. A list of "*good first*" issues for Sigma-Rust is [available on GitHub](https://github.com/ergoplatform/sigma-rust/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) - @greenhat on [Discord](https://discord.gg/Q86PNMwRsu) is ready to assist anyone who is interested.

sigma-rust is an alternative and simple implementation of ErgoTree interpreter and transaction building tools. The goal for the Rust version is to be on par with Scala version feature-wise. Now Rust version is still significantly behind. Also the goal for the Rust version is to have bindings for web, iOS and Android. The Scala version will continue to be the primary choice for JVM ecosystem with Rust version covering the rest.

To get better understanding on how to use it in your project check out how its being used in the following projects:

- [Ergo Headless dApp Framework](https://github.com/Emurgo/ergo-headless-dapp-framework);
- [Ergo Node Interface Library](https://github.com/Emurgo/ergo-node-interface);
- [Oracle Core](https://github.com/ergoplatform/oracle-core);
- [AgeUSD Stablecoin Protocol](https://github.com/Emurgo/age-usd);
- [Yoroi wallet](https://github.com/Emurgo/yoroi-frontend) (WASM bindings);
- [Ergo Desktop Wallet](https://github.com/ErgoWallet/ergowallet-desktop) (WASM bindings);
- [Ergo Utilities](https://github.com/robkorn/ergo-utilities-rust/) - General utilities to make writing off-chain Ergo code in Rust simpler 


# Tools, Services & Resources

## Services
- [Mainnet explorer](https://explorer.ergoplatform.com/)
- [Testnet explorer](https://testnet.ergoplatform.com/)
  - [Using Ergo-Testnet](https://github.com/ergoplatform/ergo/wiki/Ergo-Testnet)
- [API Docs](https://api.ergoplatform.com/api/v1/docs/)
  - [Node API](https://git.io/fjqwb)
  - [Explorer API](https://git.io/fjqwN)
  - 
**Test vectors:**
- [Ergo transaction serialization](https://git.io/fjqwX)
- [Signature scheme](https://git.io/fjqwH)
## Utilities 
 - [Miner rewards script](https://github.com/lorien/ergotools) Simple command-line tool to find miner rewards not spent and form withdrawing transaction requests for them
 - [Ergo P2S Playground](https://wallet.plutomonkey.com/p2s/?source=dHJ1ZQ==) | A web-based tool to quickly get the address corresponding to some script  



