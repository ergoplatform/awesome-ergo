<p align="center">
  <img src="https://raw.githubusercontent.com/ergoplatform/ergodocs/master/docs/assets/logo.png" width="120" alt="Ergo logo"/>
</p>

<h1 align="center">🌟 Awesome <span style="color:#f04e23">Ergo</span></h1>

<p align="center">
  A hand‑picked treasure chest of projects, tools & resources powering the <strong>Ergo Blockchain</strong> ecosystem.<br/>
  Every link is community‑verified & battle‑tested — pull requests are very welcome!
</p>

<p align="center">
  <a href="https://github.com/ergoplatform/awesome-ergo/pulls"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen?logo=github" alt="PRs welcome"></a>
  <a href="https://github.com/ergoplatform/awesome-ergo/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-CC0_1.0-lightgrey.svg" alt="License: CC0"></a>
</p>

> **Contributing:** open a PR to add or update projects. Items must be active & have a working URL.
> Docs live in <https://github.com/ergoplatform/ergodocs>, while this list lives in <https://github.com/ergoplatform/awesome-ergo>.

---

## 📚 Table of Contents

- 🏗️ [Core Infrastructure](#core-infrastructure)
  - ⚙️ [Nodes](#nodes)
  - 🔮 [Oracles](#oracles)
  - 🌉 [Bridges](#bridges)
- 💼 [Wallets](#wallets)
  - 🖥️ [Browser & Desktop](#browser--desktop)
  - 📱 [Mobile](#mobile)
  - 🛟 [Utilities & Recovery](#utilities--recovery)
- 📚 [SDKs & Libraries](#sdks--libraries)
  - 🎯 [Primary SDKs](#primary-sdks)
  - 🔒 [Core Libraries & Cryptography](#core-libraries--cryptography)
  - 🔗 [Language Bindings & Wrappers](#language-bindings--wrappers)
  - 🤝 [Community SDKs/Libraries](#community-sdkslibraries)
- 🛠️ [Development Tooling](#development-tooling)
  - 📜 [Smart Contracts & ErgoScript](#smart-contracts--ergoscript)
  - 🧱 [Frameworks](#frameworks-dev)
  - 📄 [Templates](#templates)
  - 🔧 [Utilities](#utilities)
  - ⌨️ [CLI Tools](#cli-tools)
  - 🔌 [Node Interaction & APIs](#node-interaction--apis)
  - 🧪 [Testing & Debugging](#testing--debugging)
  - 💳 [Payments](#payments)
  - ✨ [Examples & Snippets](#examples--snippets)
- 💸 [DeFi & dApps](#defi--dapps)
  - 💹 [DEXs & Swaps](#dexs--swaps)
  - 🏦 [Stablecoins & Lending](#stablecoins--lending)
  - 🚀 [Launchpads](#launchpads)
  - 🆔 [Identity & DNS](#identity--dns)
  - 🤫 [Privacy](#privacy)
  - 🎮 [Gaming & Metaverse](#gaming--metaverse)
  - 🏛️ [DAO Frameworks](#dao-frameworks)
  - 🧩 [Other dApps & Services](#other-dapps--services)
- 🖼️ [NFT Ecosystem](#nft-ecosystem)
  - 🛒 [Marketplaces & Auctions](#marketplaces--auctions)
  - 🎨 [Minting & Utilities](#minting--utilities)
  - 🗿 [NFT Projects](#nft-projects)
- ⛏️ [Mining](#mining)
  - 🏊 [Pools](#pools)
  - 💻 [Software](#software)
  - 🔧 [Utilities & Tooling](#utilities--tooling)
  - 🧠 [Smart Pooling](#smart-pooling)
  - 🔐 [Hardware Wallet Support](#hardware-wallet-support) <!-- Moved Here -->
- 📜 [Standards (EIPs)](#standards-eips)
- 🔍 [Explorers & Dashboards](#explorers--dashboards)
  - 🔭 [Explorers](#explorers) <!-- Renamed for clarity -->
  - 📈 [Dashboards & Network Stats](#dashboards--network-stats) <!-- Renamed for clarity -->
- 📊 [Analytics](#analytics)
- 🤝 [Community & Resources](#community--resources)
  - 📰 [Information Hubs](#information-hubs)
  - 💰 [Contribution Platforms](#contribution-platforms)
  - 🎓 [Education & Tutorials](#education--tutorials)
  - 📄 [Papers & Specifications](#papers--specifications)
  - 🔩 [Utilities](#utilities)

---

## 🏗️ Core Infrastructure <a id="core-infrastructure"></a>

> See also: [Protocol Overview on ErgoDocs](https://docs.ergoplatform.com/dev/protocol/protocol-overview/)

### ⚙️ Nodes <a id="nodes"></a>

- 🥇 **[Reference Client (Node)](https://github.com/ergoplatform/ergo)** – Official Scala implementation of the Ergo protocol. [`Scala`] *(Active)*
  - *See [Ergo Documentation](https://docs.ergoplatform.com/node/install/) for installation guides, including [bootstrapping from a UTXO snapshot](https://docs.ergoplatform.com/node/pruned-full-node/).*
- [Ergode](https://github.com/ross-weir/ergode) – An experimental full node implementation written in TypeScript. [`TS`] *(Experimental, ErgoHack)*

### 🔮 Oracles <a id="oracles"></a>

- 🥇 **[Oracle Core](https://github.com/ergoplatform/oracle-core)** – Core implementation for Oracle Pools V2, written in Rust. Enables robust decentralized data feeds. [`Rust`] *(Active)*
  - [Oracle Pool Bootstrap](https://github.com/ergoplatform/oracle-core/tree/master/oracle-pool-bootstrap) – Tools for initializing new oracle pools. (Also [scalahub fork](https://github.com/scalahub/oracle-pool-bootstrap))
  - [Connector Library](https://github.com/ergoplatform/oracle-core/tree/master/connectors/connector-lib) – Library for creating connectors to external data sources.
  - [How-To Guide](https://github.com/ergoplatform/oracle-core/blob/develop/docs/how_to_bootstrap.md) – Guide on bootstrapping an oracle pool.
  - [Tutorial: How I bootstrapped an ERG/XAU pool on testnet](https://github.com/ergoplatform/oracle-core/blob/develop/docs/how_to_bootstrap.md) – Practical example of pool creation.
- [EIP-23 Oracle Pools 2.0 Spec](https://github.com/ergoplatform/eips/pull/41) – Specification detailing the design of Oracle Pools V2.
- [Ergo Oracles V1 Overview](https://github.com/Emurgo/Emurgo-Research/blob/master/oracles/Oracle-Pools.md) – Research paper describing the first version of Ergo's oracle pools.
- [Ergo Easy Oracle](https://github.com/reqlez/ergo-easy-oracle) – Docker-based helper script for deploying oracle core components. [`Docker`] *(Community)*
  - [Testnet Version](https://github.com/reqlez/tn-ergo-easy-oracle) – Version configured for testnet deployment.
- [Oracle Core ETH Connector Fork](https://github.com/Luivatra/oracle-core/tree/eth-connector) – Fork adding an Ethereum connector. [`Rust`] *(Community Fork)*
- [Sininen Taivas Oracle CLI](https://github.com/sininen-taivas/ergo-oracle) – Command-line interface for interacting with oracle pools. [`Go`?] *(Community)*
- [Oracle Pool V1 Kiosk Example](https://github.com/scalahub/Kiosk/tree/master/src/test/scala/kiosk/oraclepool/v4a) – Example implementation using the Kiosk framework (V1). [`Scala`] *(Archived)*
- [Oracle Pool Stats Backend (Delphi)](https://github.com/thedelphiproject/ergo-oracle-stats-backend) – Backend service for Delphi oracle pool statistics dashboard. *(Community)*
- [Oracle Tools JS (Delphi)](https://github.com/thedelphiproject/ergo-oracle-tools-js) – JavaScript library for interacting with Delphi oracle tools. [`JS`] *(Community)*
- [OraclePoolHub](https://github.com/abchrisxyz/OraclePoolHub) – Dashboard/Hub for Oracle Pools? [`JS`/`Vue`?] *(Community)*
- [Delphi Connector Builder](https://github.com/thedelphiproject/connector-builder) - Tool for building oracle connectors for the Delphi project. *(Community)*
- [Delphi Website](https://github.com/thedelphiproject/website) - Source code for the Delphi Project website. *(Community)*
- [Scalahub Oracle Pool V1 Example](https://github.com/scalahub/OraclePool) – Example implementation of Oracle Pools V1. [`Scala`] *(Archived)*
- [Sininen Taivas Pricing Feeds](https://github.com/sininen-taivas/pricing-feeds) - Data feeds potentially used for oracles. [`Go`?] *(Community)*

### 🌉 Bridges <a id="bridges"></a>

- 🥇 **[Rosen Bridge](https://rosen.tech/)** – Primary cross-chain bridge connecting Ergo with other blockchains *(Live)*. [GitHub Org](https://github.com/rosen-bridge) *(Active)*
  - [Contracts](https://github.com/rosen-bridge/contract) – Smart contracts powering the Rosen Bridge. [`JS/TS`, `Scala`]
  - [Watcher & Guard](https://github.com/rosen-bridge/operation) – Off-chain components responsible for monitoring and securing the bridge. [`Scala`?]
  - [CLI Utils](https://github.com/rosen-bridge/utils/tree/dev/packages/cli) – Command-line utilities for bridge operations. [`TS`?]
  - [Docker Deploy Guide](https://github.com/rosen-bridge/operation/blob/dev/docs/watcher/deploy-docker.md) – Guide for deploying bridge components using Docker.
- [ErgoGravity Gateway Proxy](https://github.com/ErgoGravity/gateway-proxy) - Proxy component potentially related to cross-chain communication or bridging. *(Community, Context Needed)*

## 💼 Wallets <a id="wallets"></a>

> See also: [Wallets Overview on ErgoDocs](https://docs.ergoplatform.com/dev/wallets/)

### 🖥️ Browser & Desktop <a id="browser--desktop"></a>

- **[Nautilus Wallet](https://nautilus-wallet.io/)** – Feature-rich browser extension wallet with dApp Connector support *(Live)*. [GitHub](https://github.com/nautls/nautilus-wallet) [`JS/TS`] *(Active)*
- **[Satergo](https://satergo.com/)** – Privacy-focused desktop wallet that includes a full Ergo node *(Live)*. [GitHub](https://github.com/Satergo/Satergo) [`Java`] *(Active)*
- [Minotaur Wallet](https://minotaur-wallet.io/) – Multi-platform wallet (Android, iOS, Desktop) with multi-signature capabilities *(Live)*. [GitHub](https://github.com/minotaur-ergo/minotaur-wallet) | [Fork](https://github.com/lazypinkpatrick/minotaur-wallet) [`JS/TS`] *(Active)*
  - [Multi-Sig Server](https://github.com/minotaur-ergo/Minotaur-Signing-Server) / [Alternative](https://github.com/lazypinkpatrick/cosigning-server) – Backend server for coordinating multi-signature transactions.
- [SAFEW](https://chrome.google.com/webstore/detail/safew/lmjcdljhgidjbcpdkfknpfknbbkfpogg) – Simple browser extension wallet with dApp Connector *(Live)*. [GitHub](https://github.com/ThierryM1212/SAFEW) | [EWC Fork?](https://github.com/ThierryM1212/ewc) [`JS/TS`] *(Active)*
- [Coinbarn Wallet Extension](https://github.com/coinbarn/coinbarn-extension) - Browser wallet extension from CoinBarn. [`TS`] *(Community, Inactive?)*
- [Ergo URL Wallet](https://github.com/scalahub/erg-urlwallet) - Simple wallet concept using URLs. [`JS`?] *(Archived)*
- [Ergo Wallet V2 Concept (ladopixel)](https://github.com/ladopixel/ergowalletv2) - Conceptual work for a wallet. [`TS`] *(Community, Concept)*

### 📱 Mobile <a id="mobile"></a>

- **[Ergo Mobile Wallet (Android)](https://play.google.com/store/apps/details?id=org.ergoplatform.android)** – Official Android wallet developed by the core team *(Live)*. [GitHub](https://github.com/ergoplatform/ergo-wallet-app) [`Kotlin`] *(Active)*
- **[Ergo Mobile Wallet (iOS)](https://apps.apple.com/us/app/ergo-wallet-app/id1569044501)** – Official iOS wallet developed by the core team *(Live)*. [GitHub](https://github.com/ergoplatform/ergo-wallet-app) [`Swift`] *(Active)*
- [Minotaur Wallet](https://minotaur-wallet.io/) – Also available on Android & iOS (see Desktop section). [`JS/TS`] *(Active)*

### 🛟 Wallet Utilities & Recovery <a id="utilities--recovery"></a>

- 🥇 **[Ergo Paper Wallet Generator](https://anon-br.github.io/ergo-paper-wallet/)** – Securely generate paper wallets offline *(Live)*. [GitHub](https://github.com/anon-br/ergo-paper-wallet) | [Fork](https://github.com/platypus45/ergo-paper-wallet) [`JS/TS`]
- [Yoroi Wallet Recovery Tool](https://github.com/satsen/yoroi-ergo-wallet-recover) – Tool to recover funds sent to legacy Yoroi Ergo wallets. [`Java`]
- [Stealth Address Generator](https://ergomixer.github.io/stealth/) – Web tool for generating EIP-41 stealth addresses.
- [Cold Wallet Setup Guide (Wiki)](https://github.com/ergoplatform/ergo-wallet-app/wiki/Cold-wallet) – Guide for setting up cold storage using the official mobile apps.
- [Ergo Poor Man's Wallet (EPMW)](https://github.com/epmw/epmw) – An ultra-low-cost, DIY hardware wallet project using commodity hardware. [`Hardware`] *(Experimental)*
- [Ergo Light Client (iOS Beta)](https://github.com/bjenkinsgit/ErgoIOSLiteClient) – Community-developed lightweight iOS client. [`Swift`] *(Beta)*
- [Ergo Wallet Duster](https://github.com/mgpai22/ergo-wallet-duster) - Tool to consolidate small UTXOs (dust) in a wallet. [`Scala`] *(Community Tool)*
- [Koinly CSV Extractor](https://github.com/Luivatra/koinly-csv-extract) - Tool to extract Ergo transaction data for Koinly tax software. [`Python`] *(Community Tool)*
- [Export Ergo Transactions](https://github.com/crystoll/export-erg-transactions) - Script to export transaction history. [`Python`] *(Community Tool)*
- [Wallet Explorer (ross-weir)](https://github.com/ross-weir/wallet-ex) - Experimental wallet explorer tool. [`TS`] *(Community, Experimental)*

---

## 📚 SDKs & Libraries <a id="sdks--libraries"></a>

> See also: [Libraries Overview on ErgoDocs](https://docs.ergoplatform.com/dev/libraries/)

### 🎯 Primary SDKs

- 🥇 **[AppKit](https://github.com/ergoplatform/ergo-appkit)** – Official Java/Scala SDK for building off-chain applications and interacting with the Ergo blockchain. [`Java`, `Scala`] *(Active)* | [Scalahub Fork](https://github.com/scalahub/ergo-appkit)
- 🥇 **[Fleet SDK](https://fleet-sdk.github.io/docs/)** – Official JavaScript/TypeScript SDK optimized for building web-based dApps and browser extensions. [GitHub](https://github.com/fleet-sdk/fleet) [`JS/TS`] *(Active)*
- 🥇 **[Sigma-Rust](https://github.com/ergoplatform/sigma-rust/)** – Core Ergo primitives, cryptographic functions, and serialization implemented in Rust, forming the basis for many other libraries. [`Rust`] *(Active)* | [Aslesarenko Fork](https://github.com/aslesarenko/sigma)

### 🔒 Core Libraries & Cryptography

- 🥇 **[Sigmastate Interpreter](https://github.com/ScorexFoundation/sigmastate-interpreter)** – The core engine that interprets and validates ErgoScript contracts. Defines the language types and semantics. [`Scala`, `ErgoScript`] *(Active)* | [Dmdv Fork (Server?)](https://github.com/Dmdv/server-interpreter)
- [Scrypto](https://github.com/input-output-hk/scrypto/) – Cryptographic primitives library used by Ergo, developed by IOG. [`Scala`]
- [Scrypto Cookbook (kushti)](https://github.com/kushti/scapi-cookbook) - Examples and usage patterns for Scrypto. [`Scala`] *(Community)*
- [Scryptx](https://github.com/aslesarenko/scryptx) – Scrypto extensions or related cryptographic utilities? [`Scala`?] *(Community)*
- [Scorex Util](https://github.com/ScorexFoundation/scorex-util) – Utility classes shared across Scorex-based blockchain projects. [`Scala`]
- [Debox](https://github.com/ScorexFoundation/debox) – Library providing efficient primitive type Boxes (alternatives to Scala's standard boxing). [`Scala`]
- [BouncyCastle JS](https://github.com/aslesarenko/bouncycastle-js) – BouncyCastle cryptography library compiled for JavaScript environments. [`JS`]
- [Scorex Crypto AVLTree](https://github.com/knizhnik/scorex_crypto_avltree) – Rust implementation of the authenticated AVL+ Tree used in Ergo's state. [Paper](https://github.com/knizhnik/scorex_crypto_avltree/blob/main/crypto_avltree.md) [`Rust`]
- [AVLIODB](https://github.com/ScorexFoundation/AVLIODB) – Authenticated dictionary implementation based on AVL+ trees, used in the Ergo reference node. [`Scala`]
- [Scorex ProofOfStake Example](https://github.com/ScorexFoundation/ProofOfStake) – Example implementation of a Proof-of-Stake consensus mechanism using the Scorex framework. [`Scala`]
- [Scorex SimpleTransactions Example](https://github.com/ScorexFoundation/SimpleTransactions) – Simple transaction example using the Scorex framework. [`Scala`]

### 🔗 Language Bindings & Wrappers

- 🥇 **[ErgoLib (sigma-rust)](https://github.com/ergoplatform/sigma-rust/tree/develop/ergo-lib)** – High-level Rust abstractions built on top of `sigma-rust` primitives. [Docs](https://docs.rs/ergo-lib/) [`Rust`] *(Active)*
- 🥇 **[ergo-lib-wasm](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-wasm)** – WebAssembly bindings for `ergo-lib`, enabling its use in JavaScript/TypeScript environments. [NPM (Browser)](https://www.npmjs.com/package/ergo-lib-wasm-browser) | [NPM (NodeJS)](https://www.npmjs.com/package/ergo-lib-wasm-nodejs) [`JS/TS`, `Rust`] *(Active)*
- [ergo-lib-jni](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-jni) – Java Native Interface (JNI) bindings for `ergo-lib`, allowing use from JVM languages (Java, Scala, Kotlin). [Docs](https://docs.rs/ergo-lib-jni/) [`Java`, `Rust`] *(Active)*
- 🥇 **[ergo-lib-python](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-python)** – Python bindings for `ergo-lib` (recommended for Python development). [PyPI](https://pypi.org/project/ergo-lib/) [`Python`, `Rust`] *(Active)*
- [ergo-lib-c](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-c) – C bindings for `ergo-lib`, enabling integration with C/C++ and other languages via FFI. [Docs](https://docs.rs/ergo-lib-c/) [`C`, `Rust`] *(Active)*
- [ergo-lib-go](https://github.com/sigmaspace-io/ergo-lib-go) – Community-maintained Go bindings for `ergo-lib` (utilizing the C bindings). [Docs](https://pkg.go.dev/github.com/ergoplatform/ergo-lib-go) [`Go`, `C`, `Rust`] *(Community)*
- [Ergo Wallet Core (JVM)](https://mvnrepository.com/artifact/org.ergoplatform/ergo-wallet) – Core wallet logic extracted from the reference node, usable in JVM projects. [Source](https://github.com/ergoplatform/ergo/tree/master/ergo-wallet) [`Java`]

### 🤝 Community SDKs/Libraries <a id="community-sdkslibraries"></a>

- **[FleetSharp](https://github.com/pulsarz/FleetSharp)** – C#/.NET transaction builder library inspired by Fleet SDK, enabling dApp development in the .NET ecosystem. [`C#`] *(Community)*
  - [SigmaFi Plugin](https://github.com/pulsarz/FleetSharp.SigmaFi) | [Spectrum Plugin](https://github.com/pulsarz/FleetSharp.SpectrumFi) | [CoinGecko Plugin](https://github.com/pulsarz/FleetSharp.CoinGecko) – Plugins for interacting with specific dApps/services.
- [RustKit](https://github.com/rust-ergo/rustkit) – Community-driven Rust SDK built upon `sigma-rust`, offering higher-level abstractions. [`Rust`] *(Community)*
- [Ergpy](https://github.com/mgpai22/ergpy) – Older Python wrapper using JPype to interface with AppKit (consider using the official `ergo-lib-python` bindings instead). [`Python`, `Java`] *(Community, Legacy)* | [Native Fork](https://github.com/mgpai22/ergpy-native) | [Peixoto Fork](https://github.com/rf-peixoto/ergopy)
- [ergopyng](https://github.com/andyceo/ergopyng) – Python library for Ergo. [`Python`] *(Community)*
- [ergo-golang](https://github.com/azhiganov/ergo-golang) – Early-stage Go library for interacting with the Ergo blockchain. [`Go`] *(Community, Early Stage)* | [Pepenger Fork](https://github.com/pepenger/ergo-golang)
- [sigma_rb](https://github.com/thedlop/sigma_rb) – Ruby bindings for `sigma-rust` via the C interface. [`Ruby`, `C`, `Rust`] *(Community, ErgoHack)*
- [sigma-rust-mini](https://github.com/aslesarenko/sigma-rust-mini) – Minified version of `sigma-rust` intended for resource-constrained environments. [`Rust`] *(Community, Experimental)*
  - [No-Std Fork](https://github.com/Alesfatalis/sigma-rust-mini/tree/no_std) – Fork focusing on `no_std` compatibility for embedded systems.
- [ergo-python-appkit](https://github.com/ergo-pad/ergo-python-appkit) – Alternative Python wrapper for AppKit using JPype (consider `ergo-lib-python` instead). [`Python`, `Java`] *(Community, Legacy)*
- [ogre](https://github.com/ross-weir/ogre) – TypeScript node client library compatible with Web, Deno, and Native JS environments. [`JS/TS`] *(Community)*
- [ergo_client](https://github.com/ross-weir/ergo_client) – Rust library providing HTTP clients for interacting with Ergo node and explorer APIs. [`Rust`] *(Community)*
- [sigma-builders](https://github.com/GuapSwap/sigma-builders) – Scala library providing protocol-level abstractions on top of AppKit for dApp development. [`Scala`] *(Community)*
- [eip12-types](https://github.com/capt-nemo429/eip12-types) – TypeScript types for implementing the EIP-12 dApp Connector standard. [`TS`] *(Community)*
- [GetBlok Plasma](https://github.com/GetBlok-io/GetBlok-Plasma) – AppKit-based library for working with Plasma L2 sidechains using authenticated AVL Trees. [`Scala`] *(Community)* | [K-Singh Fork](https://github.com/K-Singh/Plasma-Toolkit)
- [sigmajs-crypto-facade](https://github.com/anon-br/sigmajs-crypto-facade) – Project aiming to replace the BouncyCastle dependency in SigmaJS (WASM bindings). [`JS/TS`] *(Community, Experimental)*
- [ScalaSigmaParticle](https://github.com/dzyphr/ScalaSigmaParticle) – Ergpy-based framework designed for building cross-chain atomic swap pipelines. [`Python`] *(Community)* | [Original?](https://github.com/dzyphr/SigmaParticle)
- [dApp Connector React Package (NightOwl)](https://github.com/nightowlcasino/dApp-connector-react-package) – React package simplifying the integration of the EIP-12 dApp Connector. [`JS/TS`, `React`] *(Community)*
- [Ergo SDK JS (ErgoLabs)](https://github.com/ergolabs/ergo-sdk-js) – Community JavaScript SDK utilizing the WASM bindings (`ergo-lib-wasm`). [`JS/TS`, `Wasm`] *(Community)*
- [ergo-ts](https://github.com/coinbarn/ergo-ts) – Early TypeScript library developed by CoinBarn. [`TS`] *(Community, Inactive?)*
- [Boxer](https://github.com/ericksonwinter/boxer) - Library/tool potentially for working with Ergo boxes. [`Scala`?] *(Community)*
- [WASM Fail (c8e4d2a)](https://github.com/c8e4d2a/wasm-fail) - Debugging or testing tool related to WASM. [`Rust`?] *(Community, Debugging)*

---

## 🛠️ Development Tooling <a id="development-tooling"></a>

> See also: [Developer Getting Started Guide on ErgoDocs](https://docs.ergoplatform.com/dev/get-started/)

### 📜 Smart Contracts & ErgoScript <a id="smart-contracts--ergoscript"></a>

- 🥇 **[Sigmastate Interpreter](https://github.com/ScorexFoundation/sigmastate-interpreter)** – The core engine that interprets and validates ErgoScript contracts. [`Scala`, `ErgoScript`] *(Active)*
- 🥇 **[escript.online](https://escript.online/)** – Online editor, compiler, and playground for developing and testing ErgoScript contracts *(Live)*. [GitHub](https://github.com/SavonarolaLabs/escript-online) [`JS/TS`] *(Active)*
- 🥇 **[Ergo Playgrounds](https://github.com/ergoplatform/ergo-playgrounds)** – Scala-based framework for writing and testing Ergo contracts and off-chain logic in a simulated environment. [`Scala`] *(Active)* | [jaysee260 Fork](https://github.com/jaysee260/ergo-playground)
- [Ergoscript Compiler (Rust)](https://github.com/ergoplatform/sigma-rust/tree/develop/ergoscript-compiler) – Rust implementation of the ErgoScript compiler, part of `sigma-rust`. [`Rust`] *(Active)*
- [Ergoscript Compiler (Scala)](https://github.com/ergoplatform/ergoscript-compiler) – Original Scala command-line tool for compiling ErgoScript source files. [`Scala`] *(Active)* | [Scalahub Fork](https://github.com/scalahub/ErgoScriptCompiler)
- [ErgoScala Compiler](https://github.com/ergoplatform/ergoscala-compiler) – Experimental compiler that translates a subset of Scala code into ErgoScript. [`Scala`] *(Experimental, Needs link update if available)*
- [ErgoScript CLI Compiler](https://github.com/ergoplatform/ergoscript-compiler) – Command-line tool to compile ErgoScript source code into a P2S address. [`Scala`] *(Same as Scala compiler above)*
- [VSCode ErgoScript Language Support](https://marketplace.visualstudio.com/items?itemName=ergoscript.ergoscript-language-support) – Visual Studio Code extension providing syntax highlighting for ErgoScript. [Source](https://github.com/GuapSwap/vscode-ergoscript-language-support) *(Community)*
- [FlowcardLib](https://github.com/lucagdangelo/flowcardLib) – Library containing various ErgoScript contract templates. [`ErgoScript`] *(Community)*
- [FlowCards Framework](https://github.com/ergoplatform/ergo-jde/tree/main/flowcards) – Declarative framework for building dApps using JSON configurations, part of the Ergo JDE. [`JSON`, `Scala`] *(Experimental)*
- [ergo-script-re](https://github.com/ross-weir/ergo-script-re) – Tools for reverse engineering and analyzing compiled ErgoScript bytecode. [`Rust`] *(Community)*
- [ergo-castanet](https://github.com/iandebeer/ergo-castanet) – Development tooling based on the Dhall configuration language for managing Ergo contracts. [`Dhall`, `Scala`] *(Community, Experimental, ErgoHack)*
- [Plutomonkey](https://wallet.plutomonkey.com/) – Web-based compiler supporting ErgoScript and Plutus (Cardano). *(Live)*
- [Ergo Playground (Scastie)](https://scastie.scala-lang.org/ergoplatform) – Online Scala/ErgoScript playground environment using Scastie. *(Live)*
- [KioskWeb](https://github.com/scalahub/KioskWeb) – Web interface for the Kiosk framework (now archived). [`Scala`, `JS/TS`?] *(Archived)*
- [Ergoscript Language Tools (nirvanush)](https://github.com/nirvanush/ergoscript) - Tools related to the ErgoScript language. *(Community)*
- [Ergoscript NodeJS bindings (nirvanush)](https://github.com/nirvanush/ergoscript-nodejs) - NodeJS bindings for ErgoScript tooling. [`JS`] *(Community)*
- [ErgoDiff](https://github.com/Luivatra/ergo_diff) - Tool for comparing or diffing ErgoScript? [`Go`?] *(Community)*
- [Just Ergo Things](https://github.com/ross-weir/just-ergo-things) - Miscellaneous ErgoScript examples or utilities. [`Scala`?] *(Community)*

### 🧱 Frameworks <a id="frameworks-dev"></a>

- 🥇 **[Mosaik](https://github.com/MrStahlfelge/mosaik)** – Framework for building mobile dApp frontends with a native look and feel, interacting via ErgoPay *(Paused Development)*. [`Java`] *(Paused)*
- [Kiosk](https://github.com/scalahub/Kiosk) – Framework designed for building secure Ergo dApps, focusing on composability (Project Archived). [`Scala`] *(Archived)*
- [Ergo JSON Development Environment (JDE)](https://github.com/ergoplatform/ergo-jde) – Framework for developing dApps using JSON configuration files to define contracts and interactions. [`JSON`, `Scala`] *(Experimental)* | [Scalahub Fork](https://github.com/scalahub/jde)
- [Edge](https://github.com/Ergo-Lend/edge) – Ergo Development Generics Elements: A library of reusable Scala components for dApp development, created by ErgoLend. [`Scala`] *(Community)*
- [Mosaik Web Executor](https://github.com/MrStahlfelge/mosaik-kt-js) – Browser-based executor for Mosaik applications, allowing them to run in web environments. [`Kotlin`, `JS`] *(Paused)*
- [Headless dApp Framework](https://github.com/ergoplatform/ergo-headless-dapp-framework) – Rust framework enabling the creation of portable off-chain logic for dApps, adhering to EIP-6. [`Rust`] *(Experimental)*
- [Terahertz Starter](https://github.com/nn-dmt/terahertz-starter) – Framework and template designed to accelerate the development of Ergo dApps. [`JS/TS`?] *(Community)*
- [Mosaik4S](https://github.com/aslesarenko/mosaik4s) – Scala bindings/utilities for Mosaik framework? [`Scala`] *(Community)*
- [DAppStep Framework (ilyaLibin)](https://github.com/ilyaLibin/dAppStep) - Framework or platform for dApp development. [Docs](https://github.com/nirvanush/dappstep-docs) *(Community)*

### 📄 Templates <a id="templates"></a>

- [ergo-scala-skeleton-app](https://github.com/dav009/ergo-scala-skeleton-app) – Basic skeleton template for starting a Scala-based Ergo application using AppKit. [`Scala`] *(Community)*
- [ergo-web-template](https://github.com/SavonarolaLabs/ergo-web-template) – Template for building web-based Ergo dApps using JavaScript/TypeScript and Fleet SDK. [`JS/TS`] *(Community)*
- [ergo-js-template](https://github.com/anon-real/ergo-js-template) – Minimalist JavaScript template for simple Ergo interactions. [`JS/TS`] *(Community)*
- [Ergo Off-Chain Bot Template](https://github.com/mgpai22/Ergo-OffChain-Bot-Template) – Template for creating off-chain bots in Scala using AppKit. [`Scala`] *(Community)*
- [scala-play-next-ergo](https://github.com/kii-dot/scala-play-next-ergo) – Full-stack template combining Scala Play (backend), AppKit, and Next.js (frontend). [`Scala`, `JS/TS`] *(Community)*
- [ergo-play-boilerplate](https://github.com/kii-dot/ergo-play-boilerplate) – Scala Play boilerplate project for building Ergo backends. [`Scala`] *(Community)*
- [ergo-basic-template](https://github.com/ERGnomes/ergo-basic-template) – Basic React template for frontend dApp development. [`JS/TS`, `React`] *(Community)*
- [Terahertz Starter](https://github.com/nn-dmt/terahertz-starter) – Framework and template designed to accelerate the development of Ergo dApps. [`JS/TS`?] *(Community)*

### 🔧 Utilities <a id="utilities"></a>

- [Ergo Utils (JS)](https://github.com/anon-real/ErgoUtils) – Utility library in JavaScript/TypeScript providing common functions for Ergo development. [`JS/TS`] *(Community)*
- [TokenJay](https://tokenjay.app/) – Mobile-friendly web application for minting, managing, and sending Ergo tokens and NFTs *(Live)*. *(Community)*
- [Yet Another Airdrop Tool (YAAT)](https://github.com/FlyingPig69/YAAT/) – Python script for performing batch transfers and airdrops of Ergo tokens. [`Python`] *(Community)*
- [Ergo Node Interface (Rust)](https://github.com/ergoplatform/ergo-node-interface-rust) – Rust library for interacting with the Ergo node's REST API. [`Rust`] *(Official)* | [aliamsk Fork](https://github.com/aliamsk/ergo-node-interface)
- [ergo-assembler](https://github.com/anon-real/ergo-assembler) – Off-chain service for assembling and signing transactions, potentially simplifying dApp logic. [`Scala`] *(Community)*
- [Transaction Builder UI](https://thierrym1212.github.io/txbuilder/) – Web-based UI for constructing, inspecting, manipulating, and signing transaction JSON *(Live)*. [GitHub](https://github.com/ThierryM1212/transaction-builder/) [`JS/TS`] *(Community)*
- [ErgoSimpleAddresses](https://github.com/kushti/ergo-simple-addresses) – Java library for basic address manipulation and validation. [`Java`] *(Official)*
- [ErgoUtilsUploadService](https://github.com/arobsn/ErgoUtilsUploadService) – Backend service designed to handle NFT image uploads for the ErgoUtils library. [`C#`] *(Community)* | [anon-br fork](https://github.com/anon-br/ErgoUtilsUploadService)
- [Ergo Vanity Address Generator](https://github.com/jellymlg/ergo-vanitygen) – Tool for generating custom Ergo addresses with specific prefixes. [`Scala`] *(Community)*
- [Ergo Monitoring](https://github.com/SabaunT/ergo-monitoring) – Debugging service providing insights into node status and blockchain state. [`Rust`] *(Community)*
- [Ergo Faucet](https://github.com/zargarzadehm/ergo-faucet) – Simple implementation of a faucet for distributing testnet ERG or tokens. [`Scala`] *(Community)* | [mgpai22 fork](https://github.com/mgpai22/ergo_faucet)
- [Chain Name Service (Experimental)](https://github.com/ross-weir/chain-name-service) – Experimental implementation of a decentralized naming service on Ergo. [`Scala`] *(Community, Experimental)*
- [Transaction Group Framework](https://github.com/GetBlok-io/Subpooling#frameworks--abstractions) – Framework for managing large groups of interrelated transactions, developed by GetBlok for subpooling. *(Community)*
- [Ergo Utilities (Rust)](https://github.com/ergoplatform/ergo-utilities-rust) – Official Rust library containing various utilities useful for off-chain code development. [`Rust`] *(Official)* | [aliamsk Fork](https://github.com/aliamsk/ergo-utilities-rust)
- [Token Reward Dispenser](https://github.com/FlyingPig69/TokenRewardDispenser) – Utility script for distributing token rewards based on specified criteria. [`Python`] *(Community)*
- [Ergo Setup](https://github.com/abchrisxyz/ergo-setup) – Docker Compose setup for easily running an Ergo node, explorer, and GraphQL interface. [`Docker`] *(Community)* | [reqlez Fork](https://github.com/reqlez/ergo-setup)
- [Ergo Handshake (Reference)](https://github.com/SabaunT/ergo-handshake) – Reference implementation of the Ergo P2P network handshake protocol. [`Rust`] *(Official)*
- [MobilERG](https://github.com/ladopixel/mobilERG) – Experimental project to interact with the Ergo blockchain via phone calls and SMS messages. [`Python`] *(Community, Experimental)*
- [tERGminal](https://github.com/ladopixel/tERGminal) – Terminal-based interface for interacting with the Ergo blockchain. [`Python`] *(Community, ErgoHack)*
- [On-Chain Notifications Service](https://github.com/ergopad/onchain-notifications-service) – Service for monitoring transactions and tracking on-chain events, developed by ErgoPad. [`Scala`] *(Community)*
- [Ergo-node-TUI-installer](https://github.com/Itaggergaard/Ergo-node-TUI-installer) – Text-based User Interface (TUI) installer for simplifying Ergo node setup. [`Shell`] *(Community)*
- [Ergo Synced Node Helper](https://github.com/mgpai22/ergo-synced-node) – Helper scripts for managing and ensuring an Ergo node is fully synchronized. [`Python`, `Shell`] *(Community)*
- [Ergo Portable Node](https://github.com/ross-weir/ergo-portable) – Scripts to create a portable Ergo node setup, useful for running on different machines. [`Shell`] *(Community)*
- [Ergo Nix Toolkit](https://github.com/ergoplatform/ergo-nix) – Nix toolkit for building and managing Ergo-related software packages reproducibly. [`Nix`] *(Official)*
- [Ergo Bootstrap](https://github.com/ergoplatform/ergo-bootstrap) – Nix-based tool for deploying Ergo clusters and infrastructure. [`Nix`, `Shell`] *(Official)*
- [Ergo RPI Scripts](https://github.com/Eeysirhc/ergo-rpi) – Scripts and guides for setting up and running an Ergo full node on a Raspberry Pi. [`Shell`?] *(Community)* | [Logs Repo](https://github.com/Eeysirhc/ergo-rpi-node-logs)
- [ErgoScripts (Misc)](https://github.com/glasgowm148/ergoscripts) – Collection of miscellaneous community-contributed scripts (e.g., nginx configurations). [`Shell`, `Other`] *(Community)*
- [ErgoNodeAndroid (Termux)](https://github.com/rustinmyeye/ErgoNodeAndroid) – One-click installer app for setting up an Ergo node on Android devices using Termux. [`Shell`, `Android`] *(Community)* | [Related Scripts](https://github.com/rustinmyeye/phonenodescriptsnshit)
- [ErgoTool](https://github.com/aslesarenko/ergo-tool) – Command-line interface tool built with AppKit for various blockchain interactions. [`Scala`] *(Community)* | [ergoplatform mirror](https://github.com/ergoplatform/ergo-tool)
- [ErgoSphere](https://github.com/jellymlg/ErgoSphere) – Collection of tools and utilities for Ergo developers and users. [`Scala`?] *(Community)*
- [Ergo Meta](https://github.com/nautls/ergo-meta) – Metadata service used by the Nautilus wallet to provide information about tokens and dApps. [`JS/TS`] *(Community)*
- [Ergo UIKit](https://github.com/aslesarenko/ergo-uikit) – UI component library for Ergo apps. [`JS/TS`?] *(Community)*
- [Bitdomains Plasma](https://github.com/bitdomains/plasma) – Plasma L2 implementation by Bitdomains. [`Scala`?] *(Community)*
- [Airdrop Address Recorder](https://github.com/Luivatra/airdropaddressrecorder) - Tool to record addresses for airdrops. [`Python`] *(Community)*
- [Ergo Test Utilities (Sininen Taivas)](https://github.com/sininen-taivas/ergo-test) - Testing utilities. [`Go`?] *(Community)*
- [Ergo Utils (Sininen Taivas)](https://github.com/sininen-taivas/ergoutils) - General utilities in Go. [`Go`] *(Community)*
- [Ergo Tx Verify (ergopool.io)](https://github.com/ergopool-io/ergotxverify) - Tool for verifying transactions, likely for pool payouts. [`Go`] *(Community)*

### ⌨️ CLI Tools <a id="cli-tools"></a>
*(Note: Many utilities in the section above also have CLI interfaces. This section highlights tools primarily used via command line.)*

- [Yet Another Airdrop Tool (YAAT)](https://github.com/FlyingPig69/YAAT/) – Python CLI tool for batch transfers/airdrops. [`Python`] *(Community)*
- [Ergo Vanity Address Generator](https://github.com/jellymlg/ergo-vanitygen) – CLI tool to generate custom Ergo addresses. [`Scala`] *(Community)*
- [MobilERG](https://github.com/ladopixel/mobilERG) – CLI interface for interacting with Ergo via phone/SMS (experimental). [`Python`] *(Community, Experimental)*
- [tERGminal](https://github.com/ladopixel/tERGminal) – CLI wallet and interaction tool. [`Python`] *(Community, ErgoHack)*
- [Ergo-node-TUI-installer](https://github.com/Itaggergaard/Ergo-node-TUI-installer) – CLI (TUI) based installer for Ergo nodes. [`Shell`] *(Community)*
- [Ergo Synced Node Helper](https://github.com/mgpai22/ergo-synced-node) – CLI scripts for node management. [`Python`, `Shell`] *(Community)*
- [Ergo Portable Node](https://github.com/ross-weir/ergo-portable) – CLI scripts for creating portable node setups. [`Shell`] *(Community)*
- [Ergo Nix Toolkit](https://github.com/ergoplatform/ergo-nix) – CLI tools for managing Ergo packages via Nix. [`Nix`] *(Official)*
- [Ergo Bootstrap](https://github.com/ergoplatform/ergo-bootstrap) – CLI tool for deploying Ergo clusters via Nix. [`Nix`, `Shell`] *(Official)*
- [Ergo RPI Scripts](https://github.com/Eeysirhc/ergo-rpi) – CLI scripts for RPi node setup. [`Shell`?] *(Community)*
- [ErgoScripts (Misc)](https://github.com/glasgowm148/ergoscripts) – Collection including CLI-usable scripts. [`Shell`, `Other`] *(Community)*
- [ErgoNodeAndroid (Termux)](https://github.com/rustinmyeye/ErgoNodeAndroid) – Underlying scripts are CLI-based for Termux. [`Shell`, `Android`] *(Community)*
- [ErgoTool](https://github.com/aslesarenko/ergo-tool) – AppKit-based general purpose CLI tool. [`Scala`] *(Community)* | [ergoplatform mirror](https://github.com/ergoplatform/ergo-tool)

### 🔌 Node Interaction & APIs <a id="node-interaction--apis"></a>

- 🥇 **[Danaides](https://github.com/ergopad/danaides)** – High-performance blockchain indexing toolkit developed by ErgoPad, useful for dApp backends. [`Python`] *(Community)*
- 🥇 **[Ergo Node API Swagger UI](http://127.0.0.1:9053/swagger)** – Interactive documentation for the local Ergo node's REST API (access via your running node). [OpenAPI Spec](https://github.com/ergoplatform/ergo/blob/master/src/main/resources/api/openapi.yaml) *(Official)*
- [Ergo GraphQL](https://github.com/capt-nemo429/ergo-graphql) – GraphQL interface providing an alternative way to query Ergo blockchain data. [`JS/TS`] *(Community)* | [Nautls Fork](https://github.com/nautls/ergo-graphql)
- [Rosetta API for Ergo](https://github.com/ross-weir/rosetta-ergo) – Implementation of the Rosetta API standard for Ergo, facilitating integration with exchanges and wallets. [`Go`] *(Community)*
- [Ergo Scanner](https://github.com/ergoplatform/scanner) – Official framework for scanning the blockchain for specific events or patterns. [`Scala`] *(Official)*
- [ergo-indexer-rust](https://github.com/darkdrag00nv2/ergo-indexer-rust) – Blockchain indexer implementation written in Rust. [`Rust`] *(Community)*
- [Strainer](https://github.com/dav009/strainer) – Tool to listen for transactions/UTXOs from a node and pipe them for processing. [`Rust`] *(Community)*
- [ergo-node-zmqpub](https://github.com/cruxfinance/ergo-node-zmqpub) – Plugin for the Ergo node to publish events (like new blocks/transactions) via ZeroMQ. [`Scala`] *(Community)*
- [Pragmaxim Chain Indexer (Ergo)](https://github.com/pragmaxim-com/chain-indexer/tree/ergo-boxes) – Custom chain indexer implementation with support for Ergo. [`Scala`] *(Community)*
- [Ergonnection](https://github.com/Satergo/Ergonnection) – Java library focusing on P2P networking aspects of the Ergo protocol (used by Satergo). [`Java`] *(Community)*
- [General API Docs](https://api.ergoplatform.com/api/v1/docs/) – Overview documentation for the Node and main Explorer APIs. *(Official)*
  - [Node API Specification (OpenAPI)](https://github.com/ergoplatform/ergo/blob/master/src/main/resources/api/openapi.yaml) – OpenAPI (Swagger) definition file for the Node API.
  - [Explorer API v1 Specification (OpenAPI)](https://github.com/ergoplatform/explorer-backend/blob/master/modules/explorer-api/src/main/resources/openapi.yaml) – OpenAPI definition file for the official Explorer API v1.
- [Ergonode Spyder](https://github.com/chriswill/ergonode-spyder) – Network spider tool for discovering and analyzing Ergo nodes on the network. [`C#`] *(Community)*
- [Ergo Blockchain Scanner (Aragogi)](https://github.com/aragogi/scanner) – Alternative scanner implementation. [`Scala`] *(Community)*
  - [Aragogi Scanner Frontend](https://github.com/aragogi/scanner-front) – Frontend interface for the Aragogi scanner. *(Community)*
- [Ergo Node API SDKs (ross-weir)](https://github.com/ross-weir/ergo-node-api-sdks) - Generated SDKs for interacting with the node API. *(Community)*
- [Ergo API (ergopool.io)](https://github.com/ergopool-io/ergoapi) - API component for the ergopool.io mining pool infrastructure. [`Go`] *(Community)*
- [TxBuilder Service (nirvanush)](https://github.com/nirvanush/txbuilder-service) - Service for building transactions, potentially off-chain. [`TS`?] *(Community)*
- [Ergo Explorer Websockets Demo](https://github.com/noob77777/ergoexplorer-websockets-demo) - Demonstration of using websockets with an explorer backend. *(Community, Example)*

### 🧪 Testing & Debugging <a id="testing--debugging"></a>

- 🥇 **[Contract Testing Framework](https://github.com/anon-real/contract-testing)** – Framework for off-chain testing of ErgoScript contracts using simulated contexts. [`Scala`] *(Community)* | [Code-for-uss Fork](https://github.com/code-for-uss/contract-testing)
- [Ergoscript Simulator](https://github.com/spectrum-finance/ergoscript-simulator) – Community tool developed by Spectrum Finance for simulating ErgoScript execution. [`Scala`?] *(Community)*
- [Ergo Puppet](https://github.com/dav009/ergo-puppet) – Tool for off-chain experimentation and unit testing of Ergo interactions. [`Scala`] *(Community)*
- [Ergo Test Vectors](https://github.com/ergoplatform/ergo-test-vectors) – Standardized test vectors for cryptographic operations and serialization formats used in Ergo. *(Official)*
- [ScalaTest](https://github.com/scalatest/scalatest) - General Scala testing framework, widely used in Ergo Scala projects. [`Scala`] *(External Tool)*
- [Appkit Issue Repo (scalahub)](https://github.com/scalahub/AppkitIssue) - Repository likely used for reporting/tracking AppKit issues. *(Infrastructure)*
- [WASM Fail (c8e4d2a)](https://github.com/c8e4d2a/wasm-fail) - Debugging or testing tool related to WASM. [`Rust`?] *(Community, Debugging)*

### 💳 Payments <a id="payments"></a>

- [ErgoPay (EIP-20)](https://github.com/ergoplatform/eips/blob/master/eip-0020.md) – URI scheme standard enabling interaction between wallets and dApps, especially useful for mobile (QR code scanning). [Docs](https://docs.ergoplatform.com/dev/stack/ergo-pay/) *(Standard)*
- [dApp Connector (EIP-12)](https://github.com/ergoplatform/eips/pull/23/files) – Standard interface defining how web-based dApps communicate with browser extension wallets. [Docs](https://docs.ergoplatform.com/dev/stack/dApp-connector/) *(Standard)*
- [Proxy Contracts (EIP-17)](https://github.com/ergoplatform/eips/blob/master/eip-0017.md) – Standard for using intermediate proxy contracts to enhance security and user experience in dApp interactions. [Docs](https://docs.ergoplatform.com/dev/stack/proxy-contracts/) *(Standard)*
- [ErgoPay Utilities (ThierryM1212)](https://github.com/ThierryM1212/ergo-pay) - Utilities or libraries related to implementing ErgoPay. [`JS`/`TS`?] *(Community)*
- [ErgoPay Payment Portal (MrStahlfelge)](https://github.com/MrStahlfelge/ergopay-payment-portal) - Example payment portal using ErgoPay. [`Java`?] *(Community, Example)*

### ✨ Examples & Snippets <a id="examples--snippets"></a>

- 🥇 **[ErgoScript by Example](https://github.com/ergoplatform/ergoscript-by-example)** – Collection of simple ErgoScript contracts demonstrating various language features and common patterns. [`ErgoScript`] *(Official)*
- 🥇 **[AppKit Examples](https://github.com/aslesarenko/ergo-appkit-examples)** – Repository showcasing AppKit usage in multiple supported languages (Java, Scala, JS, Python, Ruby, C). [`Java`, `Scala`, `JS`, `Python`, `Ruby`, `C`] *(Official)* | [Talgat Fork](https://github.com/Talgat-qypshaq/Appkit-By-Example)
- 🥇 **[Fleet Examples](https://github.com/fleet-sdk/fleet-by-example)** – Repository demonstrating various use cases and features of the Fleet SDK for web dApp development. [`TS`] *(Official)*
- [Ergo Contracts](https://github.com/ergoplatform/ergo-contracts) – Early examples of Ergo contracts along with their verification logic. [`Scala`] *(Official, Legacy)*
- [SigmaState Interpreter Examples](https://github.com/ScorexFoundation/sigmastate-interpreter/tree/develop/sc/src/test/scala/sigmastate/utxo/examples) – Contract examples found within the test suite of the core interpreter. [`Scala`] *(Official)*
- [Kiosk Offchain Examples](https://github.com/scalahub/Kiosk/tree/master/src/test/scala/kiosk/offchain) – Examples using the Kiosk framework's off-chain transaction assembler (JSON based). [`JSON`] *(Archived)*
- [Headless dApp Framework Tutorials](https://github.com/ergoplatform/ergo-headless-dapp-framework/tree/main/tutorials) – Tutorial demonstrating the framework with a "Math Bounty" dApp example. [`Rust`] *(Experimental)*
- [Mosaik Examples](https://github.com/MrStahlfelge?tab=repositories&q=mosaik&type=source) – Various examples showcasing the Mosaik UI framework for mobile dApps. [`Kotlin`, `Java`] *(Paused)*
- [Atomic Swap Example (secp256k1)](https://github.com/dzyphr/atomicswapexample) – Example of a 2-party atomic swap using secp256k1 signatures. [`Scala`?] *(Community)* | [2p version?](https://github.com/dzyphr/2pAtomicSwapExample)
- [ErgoRaffle Bot (JS)](https://github.com/zkastn/ergo-raffle-bot) – Example JavaScript bot interacting with the ErgoRaffle dApp. [`JS`] *(Community)*
- [Quid Games (ErgoHack)](https://github.com/hypo10use/quid-games) – Gaming dApp prototype developed during an ErgoHack event. [`Angular`, `TS`] *(Community, ErgoHack)*
- [NFT Minting for Dummies](https://github.com/lucagdangelo/minting-for-dummies) – Basic Scala script demonstrating NFT minting. [`Scala`] *(Community)*
- [Profit Sharing dApp](https://github.com/mhssamadani/ErgoProfitSharingDapp) – Example contract and logic for a simple profit-sharing dApp. [`Scala`?] *(Community)*
- [Trade-In Protocol](https://github.com/lucagdangelo/trade-in) – Example protocol demonstrating token burning and trading mechanics. [`Scala`, `JS/TS`] *(Community)*
- [SigmaFi UI Plugins](https://github.com/capt-nemo429/sigmafi-ui/blob/main/src/offchain/plugins.ts) – Example off-chain logic plugins used in the SigmaFi dApp frontend. [`TS`] *(Community)*
- [Ergo Payroll (ErgoHack)](https://github.com/andrehafner/ergo-payroll) – Payroll system prototype from an ErgoHack event. *(Community, ErgoHack)*
- [LETS Backend (ErgoHack)](https://github.com/arkan294/LETS-backend) – Local Exchange Trading System (LETS) backend prototype from an ErgoHack. *(Community, ErgoHack)*
- [Inergitance (ErgoHack)](https://github.com/inergitance) – Proof-of-concept for an inheritance dApp from an ErgoHack. *(Community, ErgoHack)*
- [dAppStep Play (ErgoPay Example)](https://github.com/nirvanush/dappstep-play) – Example backend application demonstrating ErgoPay integration. [`TS`] *(Community)*
- [Ergo Android (AppKit Demo)](https://github.com/aslesarenko/ergo-android) – Example Android application showcasing the use of AppKit. [`Java`, `Kotlin`] *(Community)*
- [Node Wallet Address Generation Demo (Java)](https://github.com/ergoplatform/ergo/blob/master/ergo-wallet/src/test/java/org/ergoplatform/wallet/AddressGenerationDemo.java) – Example Java code using the node's internal wallet logic for address generation. [`Java`] *(Official)*
- [Node Wallet Create Transaction Demo (Java)](https://github.com/ergoplatform/ergo/blob/master/ergo-wallet/src/test/java/org/ergoplatform/wallet/CreateTransactionDemo.java) – Example Java code using the node's internal wallet logic for transaction creation. [`Java`] *(Official)*
- [Ergo Asset Locker Demo](https://github.com/mowreez/ergo-asset-locker) – Demonstration dApp for locking assets in a contract. [`JS/TS`] *(Community)*
- [Ergo Audit Backend Demo](https://github.com/jlsachse/ergo-audit-backend) – Demo backend application for auditing purposes. [`Java`] *(Community)* | [Frontend](https://github.com/jlsachse/ergo-audit-frontend)
- [SchedulERG Demo](https://github.com/ladopixel/schedulERG) – Demo project utilizing encrypted descriptions. [`Python`] *(Community)* | [Web UI](https://github.com/ladopixel/schedulERGweb)
- [Ergo Offchain Demo](https://github.com/MrStahlfelge/ergo-offchain) – Examples demonstrating various off-chain interaction patterns. [`Kotlin`] *(Community)*
- [Fleet SDK Send NFT Demo](https://github.com/ladopixel/fleet-sdk-sendnft) – Simple demo script for sending NFTs using the Fleet SDK. [`JS/TS`] *(Community)*
- [Fleet SDK Create Token Demo](https://github.com/ladopixel/fleet-sdk-createtoken) – Simple demo script for creating new tokens using the Fleet SDK. [`JS/TS`] *(Community)*
- [Fleet SDK Burn Tokens Demo](https://github.com/ladopixel/fleet-sdk-burntokens) – Simple demo script for burning tokens using the Fleet SDK. [`JS/TS`] *(Community)*
- [MultiSig Input Demo (WASM)](https://github.com/SavonarolaLabs/multisig-input) – Example tests demonstrating multi-signature input handling with `ergo-lib-wasm`. [`JS`] *(Community)*
- [Fleet Chained Token Sender](https://github.com/mgpai22/fleet-ergo-chained-token-sender) – Demo script showing how to send tokens using chained transactions with Fleet SDK. [`JS/TS`] *(Community)*
- [AppKit by Example (ApexTheory)](https://github.com/ApexTheory/appkit-by-example) – Community collection of AppKit usage examples in Scala. [`Scala`] *(Community)*
- [Go Ergo Example](https://github.com/ross-weir/go-ergo-example) – Example project demonstrating how to use the Go bindings (`ergo-lib-go`) for Ergo. [`Go`, `C`] *(Community)*
- [Ergo Stealth Address Example](https://github.com/ross-weir/ergo-stealth-address-example) – Example implementation of EIP-41 stealth addresses. [`JS/TS`] *(Community, ErgoHack)*
- [Ergo Playground Scenarios](https://github.com/jaysee260/ergo-playground) – Collection of miscellaneous contract scenarios developed using Ergo Playground. [`Scala`?] *(Community)*
- [ErgoPay Server Example](https://github.com/MrStahlfelge/ergopay-server-example) – Example backend server implementation for handling ErgoPay requests. [`Java`, `Spring`] *(Community)*
- [Ergo Android Example App](https://github.com/aslesarenko/ergo-android) – Standalone Android app demonstrating Ergo integration using AppKit. [`Java`, `Kotlin`] *(Community)*
- [Mosaik AgeUSD Demo](https://github.com/MrStahlfelge/mosaik-ageusddemo) – Mosaik UI example interacting with the SigmaUSD (AgeUSD) protocol. [`Kotlin`?] *(Paused)*
- [Mosaik Tutorial Series App](https://github.com/MrStahlfelge/mosaik-tutorial-series) – Example application accompanying the Mosaik framework tutorial series. [`Kotlin`] *(Paused)*
- [Mosaik Token Burn Demo](https://github.com/MrStahlfelge/mosaik-demo-tokenburn) – Mosaik demo UI for a simple token burning application. [`Kotlin`] *(Paused)*
- [Mosaik NFT Marketplace Example](https://github.com/MrStahlfelge/mosaiknftmarketplace) – Example Mosaik UI demonstrating interaction with an NFT marketplace concept. [`Kotlin`?] *(Paused)*
- [Mosaik Box Consolidation Demo](https://github.com/MrStahlfelge/mosaikboxconsolidation) - Mosaik demo UI for consolidating UTXOs. [`Kotlin`?] *(Paused)*
- [ErgoPay Frontend Example](https://github.com/MrStahlfelge/ergopay-frontend-example) – Example frontend UI demonstrating how to generate and display ErgoPay QR codes. [`JS/TS`?] *(Community)*
- [Scalahub AgeUSD Example](https://github.com/scalahub/AgeUSD) – Example implementation of the AgeUSD stablecoin protocol (basis for SigmaUSD). [`Scala`] *(Archived)*
- [Scalahub Oracle Pool Example](https://github.com/scalahub/OraclePool) – Example implementation of Oracle Pools V1. [`Scala`] *(Archived)*
- [Reduced Transactions Example](https://github.com/zkastn/reduced-transactions) - Implementation example for EIP-43 Reduced Transactions. *(Community)*
- [Ergo Wooden Nickels](https://github.com/cafebedouin/ergo-wooden-nickels) - Example project, perhaps related to tokens or simple contracts. [`Python`?] *(Community)*

---

## 💸 DeFi & dApps <a id="defi--dapps"></a>

> See also: [Ecosystem Overview on ErgoDocs](https://docs.ergoplatform.com/uses/use-cases-overview/)

### 💹 DEXs & Swaps <a id="dexs--swaps"></a>

- 🥇 **[Spectrum Finance](https://spectrum.fi/)** – Cross-chain Decentralized Exchange (DEX) offering both AMM and Order Book trading models *(Live)*. [Contracts](https://github.com/spectrum-finance/ergo-dex/tree/master/contracts) | [Backend](https://github.com/spectrum-finance/spectrum-offchain-ergo) *(Active)* | [Stats](https://github.com/error1100/ergodex-stats)
- [DexyGold](https://dexygold.com/) – Decentralized exchange platform focusing on Gold-backed tokens and other assets *(Live)*. [Telegram](https://t.me/dexygold) | [Contracts/Spec](https://github.com/ergoplatform/ergo-jde/tree/main/kiosk/src/test/scala/kiosk/dexy) *(Active)*
- [GuapSwap](https://github.com/GuapSwap) – Decentralized profit-swapping service allowing miners to automatically swap mined tokens *(Live)*. [Contracts](https://github.com/GuapSwap/guapswap-ronin/tree/main/src/main/scala/contracts) *(Active)*
- [Single Transaction Swap](https://www.single-tx-swap.com/) – UI facilitating atomic swaps between two parties within a single transaction *(Live)*. [GitHub](https://github.com/danieloravec/ergo-token-swap) *(Active, ErgoHack)*
- [Arbit](https://github.com/ConnecMent/arbit) – Simple arbitrage platform aiming to capture price differences across Ergo DEXs. [`JS`] *(Active?)*
- [Analog Ergo](https://github.com/dzyphr/ScalaSigmaParticle) – P2P atomic swap protocol implementation. [Contract](https://github.com/dzyphr/ScalaSigmaParticle/blob/main/ScalarLock/src/main/scala/ScalarLock.scala) | [UI PoC](https://github.com/dzyphr/AtomicAnalogSwapWebsite) *(Experimental)*
- [Mew Finance](https://mewfinance.com/) – DeFi suite including a DEX, NFT marketplace, and other financial tools *(Live)*. [Docs](docs/eco/mew-finance.md) | [Telegram](https://t.me/MewFinance) *(Active)*

### 🏦 Stablecoins & Lending <a id="stablecoins--lending"></a>

- 🥇 **[SigmaUSD](https://sigmausd.io/)** – Decentralized algorithmic stablecoin based on the AgeUSD protocol *(Live)*. [EIP-15](https://github.com/ergoplatform/eips/blob/master/eip-0015.md) | [Bot](https://github.com/anon-real/sigma-usd) | [Spec](https://github.com/Emurgo/age-usd) | [Telegram](https://t.me/SigmaUSD) *(Active)* | [Platypus45 Fork](https://github.com/platypus45/sigma-usd) | [SIPs](https://github.com/ergoplatform/sips)
- [Duckpools](https://duckpools.io/) – Decentralized P2P lending platform *(Live)*. [GitHub Org](https://github.com/duckpools) | [Contracts](https://github.com/duckpools/lend-protocol-contracts/tree/main/contracts) | [Option Pools](https://github.com/duckpools/off-chain-bot/tree/optionPools/optionPools) | [Telegram](https://t.me/duckpools_chat) *(Active)*
- [EXLE (ErgoLend)](https://ergolend.org/) – Decentralized P2P lending platform *(Live)*. [Contracts/Edge Lib](https://github.com/Ergo-Lend/edge) | [Telegram](https://t.me/ErgoLend) *(Active)*
- [SigmaFi](https://sigmafi.org/) – DeFi platform offering various yield generation strategies *(Live)*. [UI](https://github.com/capt-nemo429/sigmafi-ui) | [Contracts](https://github.com/K-Singh/Sigma-Finance) | [Telegram](https://t.me/sigmafi) *(Active)* | [Docs](https://github.com/NoahErgo/SigmaFi-Docs)
- [Phoenix Finance](https://github.com/PhoenixErgo/phoenix-hodlcoin-contracts) – DeFi platform centered around the Hodlcoin concept *(Live)*. *(Active)*
- [Hodlcoin Contracts](https://github.com/lucagdangelo/hodlcoin-contracts) – Smart contracts implementing the core Hodlcoin mechanics (proof-of-hodl). *(Active)*
- [Gluon](https://github.com/DjedAlliance) – Infrastructure project aiming to bring Djed-style cross-chain stablecoins to Ergo. [Twitter](https://twitter.com/DjedAlliance) *(In Development)*
- [Scalahub AgeUSD Example](https://github.com/scalahub/AgeUSD) – Example implementation of the AgeUSD stablecoin protocol (basis for SigmaUSD). [`Scala`] *(Archived)*



### 🆔 Identity & DNS <a id="identity--dns"></a>

- [ErgoNames](https://ergonames.com/) – Decentralized domain name service (DNS) mapping human-readable names to Ergo addresses *(Live)*. [API Repo](https://github.com/ergonames/ErgoNames.Api) *(Active)*
- [Ergo Reputation System](https://reputation-systems.github.io/) – On-chain reputation system allowing users to build and verify trust *(Beta)*. [GitHub Org](https://github.com/sigma-rps) | [Library](https://github.com/reputation-systems/reputation-system-lib) | [Forum](https://www.ergoforum.org/t/reputation-system/4782) *(Active)*
- [ErgoDNS Frontend (jaythiya)](https://github.com/jaythiya/ergodns-frontend) - Frontend for an Ergo DNS project (ErgoHack?). [`JS`?] *(Community, ErgoHack)*

### 🤫 Privacy <a id="privacy"></a>

- 🥇 **[ErgoMixer](https://ergomixer.com/)** – Non-custodial, non-interactive transaction mixer enhancing privacy on the Ergo blockchain *(Live)*. [GitHub Org](https://github.com/ergoMixer/) | [Backend](https://github.com/ergoMixer/ergoMixBack) | [Releases](https://github.com/ergoMixer/ergoMixBack/releases) *(Active)* | [Web UI (Community)](https://github.com/anon92048/ergo-mixer-web)
- [Sigmajoin](https://github.com/ergoplatform/ergo-jde/blob/main/kiosk/src/test/scala/kiosk/mixer/doc/main.pdf) – Specification for a CoinJoin-like protocol utilizing Sigma protocols for enhanced privacy. [Tests](https://github.com/ergoplatform/ergo-jde/tree/main/kiosk/src/test/scala/kiosk/mixer) *(Concept/Spec)*
- [Stealth Address Docs (Aragogi)](https://github.com/aragogi/Stealth-doc) - Documentation related to a stealth address scanner/mixer concept. *(Community Concept, ErgoHack)*

### 🎮 Gaming & Metaverse <a id="gaming--metaverse"></a>

- [BlitzTCG](https://blitz-tcg.com/) – Collectible Trading Card Game utilizing Ergo NFTs *(Beta)*. *(Active)*
- [CyberVerse](https://cyberverseteam.itch.io/cyberverse) – Metaverse and gaming project built on Ergo *(Live)*. [Telegram](https://t.me/CyberVersegame) *(Active)*
- [NightOwl Casino](https://nightowlcasino.io/) – Decentralized casino platform offering various games of chance *(Live)*. [GitHub Org](https://github.com/nightowlcasino) | [Telegram](https://t.me/nightowlcasino) *(Active)*
- [Comet Community](https://github.com/Koutelier/CometCommunity) – Community project featuring various small dApps and games. [Website](https://github.com/Koutelier/CometGag-Webiste) *(Active?)*
- [ObolFlip](https://github.com/ObolFlip) – Decentralized CoinFlip betting game example. [Client](https://github.com/ObolFlip/obolflip-client) *(Example)*
- [Comet Lottery](https://github.com/mgpai22/comet-lottery) – Smart contracts and off-chain bot for running a lottery dApp. [`Scala`] *(Active?)*
- [Quid Games (ErgoHack)](https://github.com/hypo10use/quid-games) – Gaming dApp prototype developed during an ErgoHack event. [`Angular`, `TS`] *(Community, ErgoHack)*

### 🏛️ DAO Frameworks <a id="dao-frameworks"></a>

- 🥇 **[Paideia](https://paideia.im/)** – Comprehensive platform for creating and managing Decentralized Autonomous Organizations (DAOs) on Ergo *(Beta)*. [Contracts](https://github.com/paideiadao/paideia-contracts) | [Telegram](https://t.me/paideiaDAO) *(Active)*
- [Ergo Team](https://github.com/anon-real/ergo-team) – Simple example contract demonstrating a basic team treasury or DAO structure. [`ErgoScript`] *(Example)*
- [ErgoDAO (K-9Nine)](https://github.com/K-9Nine/ergodao) - DAO related project. *(Community)*
- [DAO dApp (nirvanush)](https://github.com/nirvanush/dao-dapp) - DAO dApp prototype. *(Community)*

### 🧩 Other dApps & Services <a id="other-dapps--services"></a>

- [CruxFinance](https://github.com/cruxfinance) – Project focused on building cross-chain liquidity solutions involving Ergo *(Live)*. [`Scala`, `Rust`, `JS/TS`] *(Active)*
- [Machina Finance](https://github.com/nautls/machina-finance) – Off-chain execution bot platform (formerly Ergomatic) enabling automated interactions with dApps. [`JS/TS`] *(Active)*
- [Hodlbox](https://hodlbox.xyz/) – Service allowing users to lock tokens in time-locked smart contracts *(Live)*. [GitHub](https://github.com/SavonarolaLabs/hodlbox-xyz) | [Contracts](https://github.com/SavonarolaLabs/hodlbox-xyz/tree/main/src/lib/contract) *(Active)*
- [SigmaO](https://sigmao.cc/) – Decentralized options trading platform built on Ergo *(Beta)*. [GitHub](https://github.com/ThierryM1212/SigmaO) | [Telegram](https://t.me/SigmaOpts) *(Active)*
- [Netnotes](https://github.com/networkspore/Netnotes-Linux/releases) – Secure peer-to-peer messaging and note-taking application utilizing the Ergo blockchain *(Beta)*. [`Java`] *(Active)* | [GitHub Org](https://github.com/networkspore/)
- [TabbyPOS](https://tabbypos.com/) – Point-of-Sale (POS) system allowing merchants to accept ERG and native tokens *(Live)*. [GitHub](https://github.com/Kolmen-Tech/ErgoPOS) | [Telegram](https://t.me/tabbypos) *(Active)*
- [Benefaction Platform](https://github.com/StabilityNexus/BenefactionPlatform-Ergo) – Prototype platform for facilitating charitable donations on Ergo. *(Development)*
- [Moria Finance](https://github.com/Moria-Finance) – Project exploring ERG derivatives and other financial instruments. *(Development)*
- [ChainCash](https://github.com/ChainCashLabs) – Framework for creating decentralized, note-based monetary systems on UTXO blockchains like Ergo. [Whitepaper](https://github.com/kushti/chaincash/blob/master/paper/chaincash.pdf) | [Server](https://github.com/ChainCashLabs/chaincash-rs) | [Contracts](https://github.com/ChainCashLabs/chaincash/tree/master/contracts) *(Active)*
- [Sigma Subscriptions](https://github.com/cornbelt-dev/sigma-subscriptions) – Framework for implementing on-chain subscription services. [Manager UI](https://github.com/cornbelt-dev/sigma-subscriptions-manager) *(Paused?, ErgoHack)*
- [ErgoWell](https://github.com/mhssamadani/ErgoWell) – Concept for a crowdfunding/investment platform on Ergo. [`JS/TS`] *(Inactive/Concept)*
- [Lithos Protocol](https://lithosprotocol.org/) – DeFi protocol aiming to enhance ERG liquidity and utility. [GitHub Org](https://github.com/Lithos-Protocol) | [LitePaper](https://github.com/Lithos-Protocol/LitePaper) *(Active)*
- [Off The Grid](https://github.com/Telefragged/off-the-grid) – Decentralized grid trading bot designed to operate on Ergo DEXs. [`Rust`] *(Development)*
- [Sigmarand](https://github.com/noob77777/ergo-randgen) – Commit-reveal scheme for generating pseudo-random numbers on-chain. [`Scala`] *(Experimental)*
- [Community Liquidity Bootstrap](https://github.com/AcoSmrkas/community-liquidity-bootstrap) – Platform concept from ErgoHack VII focused on bootstrapping liquidity. [`JS/TS`?] *(ErgoHack)*
- [Perma Ergo](https://github.com/firashebili/permergo-microfinancing-dao) – RealFi (Real World Finance) micro-finance project prototype from ErgoHack VI. *(ErgoHack)*
- [DumDumDum](https://github.com/kii-dot/dumdumdum) – Concept for an on-chain Twitter alternative from ErgoHack V. [`Scala`?] *(ErgoHack)*
- [Ergo Index](https://github.com/ergo-index) – Decentralized indexing service prototype developed during ErgoHack VII. [Backend](https://github.com/ergo-index/ergo-index-backend) | [Python Backend](https://github.com/ergo-index/ergo-index-backend-python) | [Contracts](https://github.com/ergo-index/ergo-index-contracts) | [Frontend](https://github.com/ergo-index/ergo-index-frontend) *(Development, ErgoHack)*
- [SigmaStamp](https://sigmastamp.com/) – Document timestamping service utilizing the Ergo blockchain for verifiable proof-of-existence (ErgoHack VII). [GitHub Org](https://github.com/sigmastamp) | [Docs](https://github.com/sigmastamp/docs) | [Frontend](https://github.com/sigmastamp/sigmastamp-frontend) *(Development, ErgoHack)*
- [Profit Sharing dApp (Org)](https://github.com/profit-sharing) - Backend/Frontend for a profit sharing dApp. [`Scala`, `JS`?] *(Community)*
- [Kalita Platform](https://github.com/Kalita-Platform/kalita) - Decentralized physical item marketplace. [`JS`?] *(Community)*
- [Ergo LETS (Local Exchange Trading System)](https://github.com/sininen-taivas/ergo-lets) - LETS implementation on Ergo. [`Go`?] *(Community)*
- [Ergo Notary](https://github.com/sininen-taivas/ergo-notary) - Notarization service on Ergo. [`Go`?] *(Community)*
- [Ergo Numerals](https://github.com/sininen-taivas/ergo-numerals) - Service dealing with numerals/numbers on-chain? [`Go`?] *(Community)*
- [Ergo WBO (Write Back Once?)](https://github.com/sininen-taivas/ergo-wbo) - Immutable data storage service? [`Go`?] *(Community)*
- [Proof of Commitment Protocol](https://github.com/koukarin/Proof-of-Commitment-Protocol) - Implementation of a commitment scheme. *(Community)*
- [Ergone V2 Frontend](https://github.com/koukarin/ErgoneV2-front-end) - Frontend for Ergone project (related to Local Economy Wallet?). *(Community)*
- [Local Economy Wallet](https://github.com/koukarin/Local-Economy-Wallet) - Wallet focused on local economies. *(Community)*
- [EHR Chain](https://github.com/greenhat/ehrchain) - Electronic Health Record project on Ergo? *(Community)*

---

## 🖼️ NFT Ecosystem <a id="nft-ecosystem"></a>

> See also: [NFTs Overview on ErgoDocs](https://docs.ergoplatform.com/uses/nft/)

### 🛒 Marketplaces & Auctions <a id="marketplaces--auctions"></a>

- 🥇 **[SkyHarbor](https://skyharbor.io/)** – Leading NFT marketplace on Ergo, supporting various sale types and standards *(Live)*. [Contracts](https://github.com/skyharbor-market/contracts) *(Active)*
- [AuctionHouse](https://ergoauctions.org/) – Platform implementing the EIP-22 standard for decentralized auctions *(Live)*. [GitHub](https://github.com/anon-real/ErgoAuctionHouse) | [Frontend](https://github.com/ergo-auction-house/frontend) | [EIP-22](https://github.com/ergoplatform/eips/blob/master/eip-0022.md) | [Telegram](https://t.me/ergoauctionhouse) *(Active)*
- [ENFT](https://github.com/enft-so/enft-dapp) - NFT marketplace project. [`JS`/`TS`?] *(Community)*

### 🎨 Minting & Utilities <a id="minting--utilities"></a>

- 🥇 **[Lilium](https://lilium.digital/)** – Suite of NFT tools including minting, collection management, and API services *(Live)*. [GitHub Org](https://github.com/LiliumErgo) | [Contracts](https://github.com/LiliumErgo/scala-api/blob/main/app/contracts/LiliumContracts.scala) [`Scala`, `JS/TS`, `Python`] *(Active)*
- [ErgoRaffle](https://ergoraffle.com/) – Decentralized platform for running raffles using NFTs as tickets or prizes *(Live)*. [GitHub](https://github.com/ErgoRaffle) | [Contracts](https://github.com/ErgoRaffle/raffle-backend/blob/master/app/raffle/RaffleContract.scala) | [Docs](https://github.com/NazeriMahdi2001/Raffle-Doc) *(Active)*
- [Ergo NFT Bulk Minter](https://github.com/mgpai22/ergo-nft-bulk-minter) – Python bulk minting script (with royalties). [`Python`] *(Community)*
- [Ergo Fleet Bulk Minter](https://github.com/mgpai22/ergo-fleet-bulk-minter) - Bulk minting script using Fleet SDK. [`JS/TS`?] *(Community)*
- [Ergo Token Minter](https://thierrym1212.github.io/tokenminter/) – Simple web UI for minting fungible tokens and basic NFTs *(Live)*. [GitHub](https://github.com/ThierryM1212/ergo-token-minter) [`JS/TS`] *(Community)*
- [CYTI](https://thierrym1212.github.io/cyti/) – "Choose Your Token ID": An experimental, mineable NFT minting contract allowing users to influence the resulting token ID *(Live)*. [GitHub](https://github.com/ThierryM1212/cyti) [`JS/TS`] *(Community, Experimental, ErgoHack)*
- [Sigma Mint](https://github.com/thedlop/sigma_mint) – Ruby NFT minting library (ErgoHack IV). [`Ruby`] *(Community, ErgoHack)*
- [NFT Image Generator](https://github.com/benyaminahmed/nft-image-generator) – Basic NFT image generation script. *(Community)*
- [Ergo NFT Viewer](https://github.com/johannesstrueber/ergo-nft-viewer) - Simple tool to view NFTs. [`JS`?] *(Community)*
- [Breed Server / Utils (c8e4d2a)](https://github.com/c8e4d2a/breedserver) - Backend/Utilities potentially for generative NFT breeding mechanics. [`TS`?, `Rust`?] | [Utils](https://github.com/c8e4d2a/breedutils) *(Community)*
- [GEN1SEARCH (gammahazard)](https://github.com/gammahazard/GEN1SEARCH) - Tool likely for searching specific generation 1 NFTs (e.g., ErgoSapiens?). [`Python`] *(Community Tool)*

### 🗿 NFT Projects <a id="nft-projects"></a>
*(Note: This is not an exhaustive list, but highlights some projects with available code or infrastructure.)*

- [ErgoSapiens](https://ergosapiens.com/) – NFT collection and community project with associated tools *(Live)*. [GitHub](https://github.com/mgpai22/ergosapiens) | [Payment Portal](https://github.com/mgpai22/ergosapiens-payment-portal) *(Active)*
- [Auction Coin](https://auctioncoin.app/) – Platform utilizing NFTs within its auction mechanics *(Live)*. [GitHub Org](https://github.com/orgs/Auction-Coin/repositories) | [Contracts](https://github.com/Auction-Coin/contracts) *(Active)*
- [Blobstopia](https://github.com/ThierryM1212/blobs-topia/) – Completed generative NFT project with an associated simple game mechanic. [Release](https://github.com/ThierryM1212/blobs-topia/releases/tag/v1.1.0) *(Done)*
- [ErgoNATION](https://github.com/nirojan95/ergonation) - NFT project website/community hub (ErgoHack?). *(Community, ErgoHack)*
- [Twotens](https://github.com/thedlop/twotens) - NFT or token project from ErgoHack. [`Ruby`?] *(Community, ErgoHack)*
- [ErgoTokens.org](https://github.com/ladopixel/ErgoTokens.org) - Website listing/showcasing Ergo tokens/NFTs. [`JS`] *(Community)*
- [ErgoNFTs.org](https://github.com/ladopixel/ErgoNFTs.org) - Website listing/showcasing Ergo NFTs. [`JS`] *(Community)*
- [Ergold](https://github.com/supERGeometry/Ergold) - NFT project, potentially related to gold tokens or themes. *(Community)*

---

## ⛏️ Mining <a id="mining"></a>

> See also: [Mining Overview on ErgoDocs](https://docs.ergoplatform.com/mining/mining-overview/)

### 🏊 Pools <a id="pools"></a>

- 🥇 **[Sigmanauts Mining Pool](https://sigmanauts.com/mining/)** – Prominent community-run mining pool. | [UI Code](https://github.com/marctheshark3/sigmanaut-mining-pool-ui)
- [MiningCore](https://github.com/oliverw/miningcore) – Popular open-source software for building mining pools, supports Ergo. [Config Wiki](https://github.com/oliverw/miningcore/wiki/Configuration) *(Software)*
- [NOMP (ergo-nomp)](https://github.com/btclinux/ergo-nomp) – Fork of the Node Open Mining Portal software adapted for Ergo mining. *(Software)*
- [Node Stratum Pool](https://github.com/vorujack/node-stratum-pool) – Stratum pool server implementation written in Node.js. [`JS`] *(Software)*
- [ergo-mining-pool (MGpai)](https://github.com/mgpai22/ergo-mining-pool) – Open source Ergo mining pool implementation. [`Go`?] *(Software)*
- [Ergopool.io Software](https://github.com/ergopool-io) – Collection of open-source components (Accounting, API, Frontend, Proxy) for running an Ergo mining pool. [`Go`, `JS/TS`] *(Software)*
  - [Accounting](https://github.com/ergopool-io/ergoaccounting) | [API](https://github.com/ergopool-io/ergoapi) | [Frontend](https://github.com/ergopool-io/ergofront) | [Proxy](https://github.com/ergopool-io/proxy) | [Tx Verify](https://github.com/ergopool-io/ergotxverify)

### 💻 Software <a id="software"></a>

- 🥇 **[Autolykos2 Nvidia Miner](https://github.com/mhssamadani/Autolykos2_NV_Miner)** – Open-source GPU miner optimized for Nvidia cards mining Autolykos v2. *(Open Source)*
- 🥇 **[Autolykos2 AMD Miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner)** – Open-source GPU miner optimized for AMD cards mining Autolykos v2. *(Open Source)*
- [Autolykos2 CPU Miner](https://github.com/mhssamadani/Autolykos2-CPUMiner) – Open-source CPU miner for Autolykos v2 (less efficient than GPU mining). *(Open Source)*
- [Autolykos GPU Miner (v1)](https://github.com/ergoplatform/Autolykos-GPU-miner) – Original open-source GPU miner for the previous Autolykos v1 algorithm. *(Open Source, Legacy)* | [mhssamadani Fork](https://github.com/mhssamadani/Autolykos-GPU-miner)
- [Ergo AMD Miner (v1)](https://github.com/mhssamadani/ergoAMDminer) – Open-source AMD miner for Autolykos v1. *(Open Source, Legacy)*
- *Note: Several closed-source miners exist (lolMiner, Nanominer, SRBMiner, NBMiner, TeamRedMiner, T-Rex). Refer to external resources like [Mining Software Comparison on ErgoDocs](https://docs.ergoplatform.com/mining/software/) for links and fee information.*

### 🔧 Utilities & Tooling <a id="utilities--tooling"></a>

- [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer) – Stratum server implementation compatible with Ergo miners. [`Scala`] | [Reqlez Fork](https://github.com/reqlez/ErgoStratumServer) *(Software Component)*
- [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy) – Stratum proxy designed for use with open-source Ergo miners. [`Scala`] *(Software Component)*
- [Stratum4Ergo](https://github.com/Satergo/stratum4ergo) – Java library for building Ergo Stratum servers. [`Java`] *(Library)*
- [Ergo Profit Calculator](https://babygrenade.github.io/ergo-profit-calc/) – Web-based calculator for estimating Ergo mining profitability *(Live Tool)*.
- [ErgoTools (Mining Rewards)](https://github.com/lorien/ergotools) – Command-line tool to find and withdraw mining rewards associated with an address. *(CLI Tool)*
- [Miner Rewarder](https://github.com/mgpai22/miner-rewarder) – Bot script designed to automate the distribution of rewards to miners (e.g., for pool operators). [`JS/TS`] *(Bot)*
- [Miner Reward Consolidator](https://github.com/mgpai22/ergo-miner-reward-consolidator) – Tool to consolidate many small mining reward UTXOs into fewer, larger ones. [`JS/TS`?] *(Tool)*
- [Miner Rights Protocol](https://github.com/The-Last-Byte-Bar/Miner-Rights-Protocol) – Concept and potential implementation for distributing tokens based on mining rights. *(Concept)*
  - [Token Flight](https://github.com/The-Last-Byte-Bar/Token-Flight) – Related implementation project.
  - [Token Flight Bot](https://github.com/The-Last-Byte-Bar/Token-Flight-Bot) – Bot associated with the Token Flight protocol.
- [Sigmanaut Mining Pool UI](https://github.com/marctheshark3/sigmanaut-mining-pool-ui) – Community-developed user interface for the Sigmanauts mining pool. [`JS/TS`] *(Community UI)*
- [Ergo CYTI Miner](https://github.com/Telefragged/ergo-cyti-miner) – Specialized miner designed to mine NFTs using the CYTI (Choose Your Token ID) contract. [`Rust`] *(Tool, ErgoHack)*
- [RustChain](https://github.com/Scottcjn/Rustchain) – Proof-of-Antiquity blockchain that anchors miner attestation data to Ergo via register-based transactions. Uses 6-point hardware fingerprinting (clock drift, cache timing, SIMD identity, thermal drift, instruction jitter, anti-emulation) to reward vintage hardware miners. [`Python`] *(Community)*

### 🧠 Smart Pooling <a id="smart-pooling"></a>

- [ErgoSmartPools](https://github.com/WilfordGrimley/ErgoSmartPools) – Research and implementation of decentralized mining pools using smart contracts. *(Research/Experimental, ErgoHack)*
- [GetBlok Subpooling Contracts](https://github.com/GetBlok-io/ergo-smartpooling-contracts) – Smart contracts developed by GetBlok for their smart subpooling system. [`Scala`] *(Community)*
- [GetBlok Subpooling Plasma Configs](https://github.com/GetBlok-io/Subpooling/tree/mainnet_plasma/conf/scripts) – Configuration scripts related to GetBlok's Plasma-based subpooling implementation. *(Community)*

### 🔐 Hardware Wallet Support <a id="hardware-wallet-support"></a>
*(Note: While listed under Mining in the ToC, this logically relates more to Wallets/Security.)*

- 🥇 **[Ledger App for Ergo (Official)](https://github.com/LedgerHQ/app-ergo)** – Official Ledger hardware wallet application for Ergo *(Live)*. [`C`] *(Active)*
- [Ledger App for Ergo (Tesseract Fork)](https://github.com/tesseract-one/ledger-app-ergo) – Community-maintained fork of the Ledger app, often incorporating newer features or fixes. [`C`] *(Active)*
  - [LedgerJS Bindings](https://github.com/anon-br/ledgerjs-hw-app-ergo) – JavaScript library for interacting with the Ledger Ergo app from web applications. [`JS`] | [Old? anon-br/ledger-ergo-js](https://github.com/anon-br/ledger-ergo-js)
  - [Ledger4j Bindings](https://github.com/aionnetwork/ledger4j) – Java library for interacting with Ledger devices (may support Ergo app via generic HID). [`Java`]
  - [Ledger Core Lib](https://github.com/LedgerHQ/lib-ledger-core) – Ledger's core library used internally for device communication. [`C++`]

---

## 📜 Standards (EIPs) <a id="standards-eips"></a>

- 🥇 **[EIP Repository](https://github.com/ergoplatform/eips)** – Official repository for Ergo Improvement Proposals, detailing standards and protocol changes. | [anon-real fork](https://github.com/anon-real/eips) | [nitram147 fork](https://github.com/nitram147/eips)
- [EIP-1: Ergo Address Types](https://github.com/ergoplatform/eips/blob/master/eip-0001.md) – Defines the different address types used on the Ergo blockchain.
- [EIP-3: HD Wallet Derivation Paths](https://github.com/ergoplatform/eips/blob/master/eip-0003.md) – Specifies standard derivation paths for Hierarchical Deterministic (HD) wallets.
- [EIP-4: Asset Standard (Tokens & NFTs)](https://github.com/ergoplatform/eips/blob/master/eip-0004.md) – Defines the standard for issuing and identifying native assets (fungible tokens and NFTs).
- [EIP-5: ErgoScript Templates (Deprecated)](https://github.com/ergoplatform/eips/blob/master/eip-0005.md) – Older, deprecated proposal for script templating.
- [EIP-6: Headless dApp Protocol](https://github.com/ergoplatform/eips/blob/master/eip-0006.md) – Defines a protocol for stateless, off-chain execution bots ("headless dApps").
- [EIP-11: Asset Issuance Box Standard](https://github.com/ergoplatform/eips/pull/11) – Standardizes the structure of the box used to issue new assets (refines EIP-4).
- [EIP-12: dApp Connector Interface](https://github.com/ergoplatform/eips/pull/23/files) – Standard interface for communication between web dApps and browser wallets.
- [EIP-15: SigmaUSD Protocol](https://github.com/ergoplatform/eips/blob/master/eip-0015.md) – Describes the core mechanics of the SigmaUSD algorithmic stablecoin protocol.
- [EIP-16: Oracle Pool V2 (Draft)](https://github.com/ergoplatform/eips/blob/eip16/eip-0016.md) – Draft proposal outlining the design for the second iteration of oracle pools.
- [EIP-17: Proxy Contracts Standard](https://github.com/ergoplatform/eips/blob/master/eip-0017.md) – Standardizes the use of proxy contracts for safer dApp interactions.
- [EIP-19: Cold Wallet Standard](https://github.com/ergoplatform/eips/blob/master/eip-0019.md) – Defines standards for air-gapped cold wallet interactions.
- [EIP-20: ErgoPay URI Scheme](https://github.com/ergoplatform/eips/blob/master/eip-0020.md) – Standard URI scheme for QR code-based wallet/dApp communication.
- [EIP-21: URI Scheme for Token Payments](https://raw.githubusercontent.com/ergoplatform/eips/master/eip-0021.md) – (Draft) Extends payment URIs to include native token information.
- [EIP-22: Auction Contract Standard](https://github.com/ergoplatform/eips/blob/master/eip-0022.md) – Defines a standard interface for on-chain auction contracts.
- [EIP-23: Oracle Pool V2 Bootstrap Standard](https://github.com/ergoplatform/eips/tree/cae50b722d6929c794847d21668500acb01f3c8c/eip-0023/contracts) – Defines the contracts and process for bootstrapping Oracle Pools V2.
- [EIP-24: Digital Artwork / NFT Standard](https://github.com/ergoplatform/eips/blob/master/eip-0024.md) – Standardizes metadata for digital artwork NFTs, including royalties.
- [EIP-25: Payment Request URI Scheme](https://github.com/ergoplatform/eips/blob/master/eip-0025.md) – General standard for creating payment request URIs (BIP-21 style).
- [EIP-27: Miner Voting Parameters](https://github.com/ergoplatform/eips/blob/master/eip-0027.md) – Defines how miners can vote on adjustable blockchain parameters.
- [EIP-31: Babel Fees Standard](https://github.com/ergoplatform/eips/blob/master/eip-0031.md) – Defines a mechanism allowing transaction fees to be paid using native tokens instead of ERG.
- [EIP-33: Crowdfunding Contract Standard](https://github.com/ergoplatform/eips/pull/33) – Proposes a standard interface for on-chain crowdfunding campaigns.
- [EIP-37: Autolykos v2 Update](https://github.com/ergoplatform/eips/blob/ddbca24fef5e91e0c80c6881fc31d8831ae69768/eip-0037.md) – Specification for the Autolykos v2 Proof-of-Work algorithm update.
- [EIP-38: Partial Voting for Miners (Draft)](https://github.com/WilfordGrimley/eip38PartialVoting) – Draft proposal exploring partial or weighted voting mechanisms for miners. *(ErgoHack)*
- [EIP-39: Just-In-Time Costing (JITC)](https://github.com/ergoplatform/eips/blob/master/eip-0039.md) – Describes the Just-In-Time Costing mechanism for ErgoScript execution.
- [EIP-41: Stealth Addresses (Draft)](https://raw.githubusercontent.com/ergoplatform/eips/d21280977f2c21dc733632c48c98d0f614bc6123/eip-0041.md) – Draft proposal for implementing privacy-enhancing stealth addresses.
- [EIP-43: Reduced Transaction](https://github.com/ergoplatform/eips/pull/91) – Proposal for a compact transaction format suitable for lightweight clients. [Implementation Example](https://github.com/zkastn/reduced-transactions)
- [EIP-44: Arbitrary Data Signing](https://github.com/ergoplatform/eips/pull/92) – Proposal for a standard method for wallets to sign arbitrary data messages.
- [EIP-45: Storage Rent Redistribution (Draft)](https://github.com/ergoplatform/eips/pull/93) – Draft exploring alternative mechanisms for storage rent redistribution.
- [EIP-46: Authentication Message Signing (Draft)](https://github.com/ergoplatform/eips/blob/2de4ea0deff12a276f74df57ef3a14dab2c5dfb8/eip-0046.md) – Draft standard for signing authentication messages, distinct from transactions.
- [EIP-47: Re-emission Contract Standard (Draft)](https://github.com/ergoplatform/eips/blob/0836dd1eca323c6b5fd6b5172c27a465bd4449cd/eip-0047.md) – Draft proposing a standard contract for managing token re-emission schedules.
- [EIP-50: Context Extension Clarification (Draft)](https://github.com/ergoplatform/eips/blob/a24fc414abbc10e6ee59f878b280d9ecc725e10c/eip-0050.md) – Draft clarifying the usage and properties of the `ContextExtension` field in transactions.
- [SigmaUSD Improvement Proposals (SIPs)](https://github.com/ergoplatform/sips) – Separate repository for proposals specifically related to improving the SigmaUSD protocol.

---

## 🔍 Explorers & Dashboards <a id="explorers--dashboards"></a>

> See also: [Explorer Overview on ErgoDocs](https://docs.ergoplatform.com/dev/stack/explorer/)

### 🔭 Explorers <a id="explorers"></a>

- 🥇 **[Ergo Explorer (Official)](https://explorer.ergoplatform.com/)** – The canonical blockchain explorer for viewing transactions, blocks, addresses, and tokens *(Live)*. [Frontend](https://github.com/ergoplatform/explorer-frontend) | [Backend](https://github.com/ergoplatform/explorer-backend) *(Active)*
- [Sigmaspace](https://sigmaspace.io/) – Alternative explorer offering additional tools, charts, and network statistics *(Live)*. [GitHub](https://github.com/pulsarz/sigmaexplorer) *(Active)* | [Testnet Version](https://github.com/pulsarz/sigmaexplorer-testnet)
- [erg-explorer](https://github.com/AcoSmrkas/ErgExplorer) – Community-built blockchain explorer. [`JS/TS`] [Telegram](https://t.me/ErgExplorer) *(Community)*
- [uexplorer](https://github.com/pragmaxim/ergo-uexplorer) – Minimalist explorer focused specifically on exploring the UTXO set. [`Scala`] *(Community)*
- [Indexed Node Explorer](https://github.com/Luivatra/indexed-node-explorer) – Simple UI designed to work with a locally indexed Ergo node. [`JS/TS`] *(Community)*
- [Testnet Explorer](https://testnet.ergoplatform.com/) – Official blockchain explorer specifically for the Ergo test network *(Live)*.
  - [Using Ergo Testnet (Wiki)](https://github.com/ergoplatform/ergo/wiki/Ergo-Testnet) – Guide on how to use the Ergo testnet.
- [ErgoAppKit Spent Box Explorer](https://github.com/mgpai22/ergoappkit-spent-box-explorer) - Tool to explore spent boxes using AppKit. [`Scala`] *(Community)*

### 📈 Dashboards & Network Stats <a id="dashboards--network-stats"></a>

- [ErgoWatch](https://ergo.watch/) – Dashboard providing comprehensive network statistics, tokenomics data, and various analytics *(Live)*. [GitHub (Backend)](https://github.com/abchrisxyz/ergowatch) *(Active)*
- [Ergo Nodes Dashboard](http://ergonodes.net/) – Network map visualizing active Ergo nodes and providing node statistics *(Live)*. [GitHub](https://github.com/Satergo/Ergonnection) *(Active)*
- [Paizo Mining Vote Simulator](https://deadit.github.io/paizo/) – Simulator tool for visualizing the potential outcomes of EIP-27 miner voting *(Live Tool)*. [GitHub](https://github.com/deadit/paizo) *(Community, ErgoHack)*
- [ErgCube](https://ergcube.com/) – Community-run dashboard and information site for the Ergo ecosystem *(Live)*. *(Community)*
- [Testnet Faucet](https://testnet.ergofaucet.org/) – Faucet for obtaining free ERG on the test network for development and testing purposes *(Live Tool)*.
- [ErgoStats Android](https://github.com/sachindayl/ErgoStatsAndroid) – Native Android application for viewing Ergo network statistics. [`Kotlin`/`Java`] *(Community)*
- [ErgoStats iOS](https://github.com/ach2swift/ErgoStats) – Native iOS application for viewing Ergo network statistics. [`Swift`] *(Community, ErgoHack)*
- [ergo-status](https://github.com/bdkent/ergo-status) – Community-run dashboard displaying the status of various Ergo network services and endpoints *(Live Tool)*. [`JS/TS`?] *(Community)*
- [ErgoDex Stats](https://github.com/error1100/ergodex-stats) - Statistics specific to the ErgoDex (Spectrum Finance) platform. [`JS`?] *(Community)*

---

## 📊 Analytics <a id="analytics"></a>

- 🥇 **[ErgoVision](https://github.com/CryptoCream/ErgoVision)** – Python-based tool for visualizing wallet activity and investigating transaction histories *(Tool)*. [`Python`] *(Community)*
  - [Colab Notebook](https://colab.research.google.com/drive/13O_6XEHi7xbjuhzby0s7YGX0rshrClXK?usp=sharing) – Google Colaboratory notebook version of ErgoVision.
- [SigmaUSD Bank Analysis Notebook](https://colab.research.google.com/drive/1iA_PPvWrJGjdpOFYME7W_lQrU4BemaE4?usp=sharing) – Colab notebook providing tools for analyzing the SigmaUSD bank contract state. [`Python`] *(Community)*
- [ergo-intelligence](https://github.com/Eeysirhc/ergo-intelligence) – Collection of tools and resources aimed at blockchain analysts studying the Ergo network. *(Community)*
- [tidyergo](https://github.com/Eeysirhc/tidyergo) – R package using the Tidyverse framework for analyzing Ergo blockchain statistics. [`R`] *(Community)*
- [ergo-analytics](https://github.com/gsblabsio/ergo-analytics) – Docker setup providing a suite of tools for gaining insights into the Ergo network. [`Docker`] *(Community)*
- [Ergo Tokenautics](https://github.com/babygrenade/ergo-tokenautics) – Tool for analyzing the distribution and holdings of Ergo native tokens. [`Python`] *(Community)*
- [Ergo Token Analysis (Freebyo)](https://github.com/freeboy0/ergo-token-analysis) – Collection of Python tools for analyzing Ergo tokens. [`Python`?] *(Community)*
- [Developer Activity (Artemis)](https://app.artemis.xyz/developer-activity?ecosystemValue=Ergo) – Platform tracking developer activity across various blockchains, including Ergo (based on GitHub commits) *(External Service)*.
- [Developer Activity (DeveloperReport)](https://www.developerreport.com/ecosystems/ergo) – Alternative platform providing insights into Ergo's developer activity *(External Service)*.
- [Ergo Node Metrics Report Notebook](https://github.com/ergoplatform/ergo/blob/master/metrics/Report.ipynb) – Jupyter notebook for analyzing performance metrics collected from an Ergo node. [`Python`] *(Official)*
- [Ergo Notebooks (Glasgowm)](https://github.com/glasgowm148/ergo-notebooks) – Collection of Jupyter notebooks for various Ergo data analysis tasks. [`Python`] *(Community)*
- [Ergo Explorer Queries (FlyingPig)](https://github.com/FlyingPig69/Ergo_Explorer_Queries) – Collection of SQL queries designed for analyzing data extracted from the official Ergo Explorer database. [`SQL`] *(Community)*
- [DefiLlama Adapters (NoahErgo)](https://github.com/NoahErgo/DefiLlama-Adapters) - Adapters for integrating Ergo DeFi data into DefiLlama. [`JS`?] *(Community Contribution)*

---

## 🤝 Community & Resources <a id="community--resources"></a>

### 📰 Information Hubs <a id="information-hubs"></a>

- 🥇 **[Ergo Platform Website](https://ergoplatform.org/)** – Official main website for the Ergo blockchain, news, and overview. [GitHub](https://github.com/ergoplatform/website) *(Official)* | [RJErik Fork](https://github.com/RJErik/ergoweb)
- 🥇 **[Ergo Documentation](https://docs.ergoplatform.com/)** – Official documentation portal covering all aspects of Ergo for users, developers, and miners. [GitHub](https://github.com/ergoplatform/ergodocs) *(Official)* | Forks: [dzyphr](https://github.com/dzyphr/ergodocs), [NetWalker108](https://github.com/NetWalker108/ergodocs), [omahs](https://github.com/omahs/ergodocs), [rustinmyeye](https://github.com/rustinmyeye/ergodocs), [satsen](https://github.com/satsen/ergodocs), [TanBeige](https://github.com/TanBeige/ergodocs) | [German Translation](https://github.com/mapp0/Ergo_DE)
- [Ergonaut Handbook](https://ergonaut.space/) – Community-driven wiki and handbook covering various Ergo topics and guides. [GitHub](https://github.com/glasgowm148/ergonaut-handbook) *(Community)*
- [Sigmaverse](https://sigmaverse.io/) – Directory showcasing dApps, tools, and projects within the Ergo ecosystem. [GitHub](https://github.com/ergoplatform/sigmaverse) *(Official)*
- [ErgoForum](https://www.ergoforum.org/) – Official community discussion forum for longer-form discussions and proposals. *(Official)*
- [Ergo Discord](https://discord.gg/ergo-platform-668903786361651200) – Main real-time community chat server on Discord. *(Official)*
- [Ergo Telegram](https://t.me/ergoplatform) – Main Telegram group for community discussion. *(Official)*
- [Ergo Reddit](https://www.reddit.com/r/ergonauts/) – Subreddit for Ergo news, discussion, and community interaction. *(Community)*
- [Awesome Ergo](https://github.com/ergoplatform/awesome-ergo) – This curated list of resources. *(Official)* | [Glasgowm Fork](https://github.com/glasgowm148/awesome-ergo) | [Scalahub Fork](https://github.com/scalahub/awesome-ergo)
- [Ergo Sites](https://ergosites.github.io/) – Community-maintained list of various Ergo-related websites. *(Community)*
- [Ergo Platform Wiki](https://github.com/ergoplatform/ergo/wiki) – Official wiki associated with the reference node software repository, often containing technical details. *(Official)*
- [Ergo Foundation Website](https://ergofoundation.org/) – Website providing information about the Ergo Foundation entity. *(Official)*
- [Ergo Platform GitHub Discussions](https://github.com/ergoplatform/ergo/discussions) – Forum within GitHub for discussions related to node development and technical protocol topics. *(Official)*
- [ergohack.io](https://ergohack.io/resources) – Resource hub for past and present ErgoHack hackathon events. *(Official)*
- [PaiNet](https://github.com/mgpai22/paiNet) / [SigmaNet](https://github.com/mgpai22/sigmanet) - Personal project/network sites. *(Community)*

### 💰 Contribution Platforms <a id="contribution-platforms"></a>

- 🥇 **[Ergo Bounties](https://github.com/ErgoDevs/Ergo-Bounties)** – Platform for proposing, finding, and funding development bounties within the Ergo ecosystem. *(Community)*
- [Grow Ergo Issues](https://github.com/ergoplatform/grow-ergo/issues) – GitHub repository issue tracker used for coordinating ecosystem growth initiatives and tasks. *(Official)*
- [Ergo Node Issues](https://github.com/ergoplatform/ergo/issues) – Main issue tracker for reporting bugs and suggesting features for the official Ergo reference node implementation. *(Official)*
- [Analytics Ecosystem Data](https://github.com/electric-capital/crypto-ecosystems/blob/master/data/ecosystems/e/ergo.toml) – Add your project here to be tracked by developer activity analytics platforms like Electric Capital. *(External)*

### 🎓 Education & Tutorials <a id="education--tutorials"></a>

- 🥇 **[DeCo Education](https://deco-education.github.io/deco-docs/docs/intro)** – Educational platform offering structured courses on Ergo and related technologies. *(Community)* | [Docs Repo](https://github.com/DeCo-Education/deco-docs) | [Homeworks](https://github.com/DeCo-Education/DeCo-Homeworks) | [Ergo School](https://github.com/DeCo-Education/Ergo-School)
  - [Into the Woods Course](https://deco-education.github.io/deco-docs/docs/category/into-the-woods) – Introductory course on Ergo concepts.
  - [ErgoScript Developer Course](https://github.com/DeCo-Education/ErgoScript-Developer-Course) – Course focused on learning ErgoScript development.
- [Learn Ergo](https://github.com/learn-ergo) - Educational resource organization. [Developer Tutorials](https://github.com/learn-ergo/DeveloperTutorials) *(Community)*
- [ErgoScript 101 Crash Course (Slides)](https://docs.google.com/presentation/d/10gYO82z_7qloRrFOcCxTFuzpP40IImPyIKMV2ZFd9M4/edit#slide=id.p) – Presentation slides providing a quick overview of ErgoScript fundamentals. *(Community)*
- [Zack Balbin's Ergo Tutorials](https://github.com/zackbalbin/ErgoTutorials) – Collection of Scala tutorials focused on Ergo development patterns. [`Scala`] *(Community)*
- [Ergo Community YouTube](https://www.youtube.com/@ErgoPlatform) – Official YouTube channel featuring AMAs, interviews, tutorials, and presentations. *(Official)*
- [ErgoFoundation YouTube](https://www.youtube.com/@ErgoFoundation) – YouTube channel specifically for content related to the Ergo Foundation. *(Official)*
- [Starting with Appkit on Gradle projects](https://github.com/ergoplatform/ergo-appkit/wiki/Tutorial-starting-with-Appkit-on-Gradle-projects) – Wiki tutorial on setting up AppKit within a Gradle-based Java/Scala project. *(Official)*
- [AppKit by Example (Video)](https://www.youtube.com/watch?v=Md5s-XV6-Hs) – Video tutorial demonstrating practical examples of using AppKit. *(Community)*
- [Learn ErgoScript By Example Via The Ergo Playground (Video)](https://www.youtube.com/watch?v=8l2v1asHgyA) – Video tutorial guiding users through ErgoScript concepts using the Ergo Playground. *(Community)*
- [Multi-Stage Contracts in the UTXO Model (Video)](https://www.youtube.com/watch?v=g3FlM_WOwBU) – Presentation explaining how to implement multi-stage logic in eUTXO systems like Ergo. *(Official)*
- [ErgoScript Design patterns (Forum)](https://www.ergoforum.org/t/ergoscript-design-patterns/222) – Forum thread discussing common design patterns in ErgoScript development. *(Community)*
- [Advanced ErgoScript Tutorial (PDF)](https://ergoplatform.org/docs/AdvancedErgoScriptTutorial.pdf) – In-depth PDF document covering more advanced ErgoScript topics. *(Official)*
- [Ergo with C# 101 (Video Playlist)](https://www.youtube.com/watch?v=aUuki-fAxwc&list=PLUWruihtE-HtL-JZk8Vb4Yn_H18aE3rb6) – YouTube playlist teaching Ergo development using C# and the FleetSharp library. *(Community)*
- [A Quick Primer on ErgoScript (Wiki)](https://github.com/ergoplatform/ergo/wiki/ErgoScript-Overview) – Overview of ErgoScript concepts on the node repository wiki. *(Official)*
- [Building Ergo: ErgoScript (Blog)](https://ergoplatform.org/en/blog/2021-06-09-building-ergo-ergoscript/) – Blog post discussing the design and features of ErgoScript. *(Official)*
- [Using Appkit from Python (Wiki)](https://github.com/ergoplatform/ergo-appkit/wiki/Using-Appkit-from-Python) – Guide demonstrating how to use AppKit from Python via the JPype bridge (Note: `ergo-lib-python` is now generally recommended). *(Official, Legacy Approach)*
- [Ergo Full Node on Raspberry Pi Guide](https://github.com/ccgarant/ergo-full-node-raspi) – Community guide detailing the process of setting up an Ergo full node on a Raspberry Pi. *(Community)*
- [Fleet SDK Documentation](https://fleet-sdk.github.io/docs/) – Official documentation for the Fleet SDK (JS/TS). *(Official)*
  - [Fleet Compiler Docs](https://fleet-sdk.github.io/docs/compiler) – Documentation for Fleet's built-in ErgoScript compiler.
  - [Fleet Serializer Overview](https://fleet-sdk.github.io/docs/serializer-overview) – Explanation of serialization methods used in Fleet.
  - [Fleet Babel Fees Plugin Docs](https://fleet-sdk.github.io/docs/plugins/babel-fees) – Documentation for the Fleet SDK plugin implementing EIP-31 Babel Fees.
- [ErgoTutorials.com (ladopixel)](https://github.com/ladopixel/ErgoTutorials.com) - Website for Ergo tutorials. [`JS`] *(Community)*
- [Ergo Learning App vERGinia](https://github.com/ErGonario/Ergo_learning_app_vERGinia) - Learning application project. *(Community)*
- *Note: The main [Ergo Documentation](https://docs.ergoplatform.com/dev/tutorials/) contains many specific guides (e.g., debugging, message signing, running off-chain bots).*

### 📄 Papers & Specifications <a id="papers--specifications"></a>

- 🥇 **[Ergo Whitepaper](https://ergoplatform.org/en/documents/)** – The foundational document outlining the core design, principles, and goals of the Ergo platform. *(Official)*
- [ErgoScript Whitepaper](https://ergoplatform.org/docs/ErgoScript.pdf) – Detailed paper describing the ErgoScript smart contract language. *(Official)*
- [Autolykos PoW Algorithm](https://ergoplatform.org/docs/ErgoPow.pdf) – Paper detailing the original Autolykos (v1) Proof-of-Work algorithm. *(Official)*
- [NiPoPoWs Paper](https://eprint.iacr.org/2016/994.pdf) – Academic paper on Non-Interactive Proofs of Proof-of-Work, a core technology used by Ergo for light clients. *(Research)*
- [Storage Rent Paper](https://ergoplatform.org/docs/StorageRent.pdf) – Paper explaining the storage rent mechanism implemented in Ergo. *(Official)*
- [Sigma Protocols Paper](https://ergoplatform.org/docs/ergoscript.pdf) – Sigma protocols and their application in ErgoScript are covered within the ErgoScript Whitepaper. *(Official)*
- [ErgoTree Specification](https://raw.githubusercontent.com/ScorexFoundation/sigmastate-interpreter/master/docs/spec/ergotree.pdf) – Formal specification of the ErgoTree binary format used for compiled scripts. *(Official)*
- [ErgoScript Language Specification](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md) – Specification defining the syntax and semantics of the ErgoScript language. *(Official)*
- [Sigma Language DSL Documentation](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/sigma-dsl.md) – Documentation on the Sigma-protocol Domain Specific Language features within ErgoScript. *(Official)*
- [Know Your Assumptions (KYA)](https://github.com/kushti/kya) – Framework and methodology for analyzing the security assumptions of blockchain protocols. [PDF](https://github.com/kushti/kya/blob/master/kya.pdf) *(Research)*
- [ChainCash Whitepaper](https://github.com/kushti/chaincash/blob/master/paper/chaincash.pdf) – Whitepaper describing the ChainCash protocol for decentralized note-based monetary systems. *(Research)*
  - [ChainCash Server Docs](https://github.com/ChainCashLabs/chaincash/blob/master/docs/server.md) – Documentation for the ChainCash server implementation.
- [High Level Design Patterns In Extended UTXO Systems](https://github.com/Emurgo/Emurgo-Research/blob/master/smart-contracts/High%20Level%20Design%20Patterns%20In%20Extended%20UTXO%20Systems.md) – Research exploring common dApp design patterns in the eUTXO model. *(Research)*
- [Ergo Scala Style Guide](https://github.com/ergoplatform/ergo-scala-style-guide) – Official style guide for contributing Scala code to Ergo projects. *(Official)*
- [Ergo Social Contract](https://ergoplatform.org/en/blog/2022-04-26-the-ergo-manifesto-revised-edition/) – Document outlining the guiding principles, values, and long-term vision of the Ergo platform (Manifesto). *(Official)*
- [On Contractual Money](https://ergoplatform.org/docs/AdvancedErgoFeatures.pdf) – Paper discussing advanced financial primitives and features possible on Ergo. *(Official)*
- [ErgoScript Compiler Documentation](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/ergoscript-compiler.md) – Documentation detailing the internals of the ErgoScript compiler. *(Official)*
- [ErgoScript Performance & Style Guide](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/perf-style-guide.md) – Guide with tips for writing efficient and idiomatic ErgoScript code. *(Official)*
- [Ergo Platform Improvement Proposals (EIPs)](https://github.com/ergoplatform/eips) – Link to the main EIPs repository (see [Standards](#standards-eips) section for individual EIPs). *(Official)*
- [SLIP-0044 : Registered coin types for BIP-0044](https://github.com/satoshilabs/slips/blob/master/slip-0044.md) – Ergo's registered coin type (`429`) for use in BIP-44 derivation paths. *(Standard)* | [Related IOHK Address Lib](https://github.com/input-output-hk/cardano-addresses) (May contain relevant logic)
- [Ergo Subblocks Paper](https://raw.githubusercontent.com/ergoplatform/ergo/e15dcd0b4ca0a72d32d97228f010d813540de39d/papers/subblocks/subblocks.md) – Paper exploring the concept of sub-blocks for potential future protocol enhancements. *(Research)*
- [Ergohack Sidechain Whitepaper](https://github.com/ross-weir/ergohack-sidechain/blob/main/docs/whitepaper/sidechain.pdf) – Whitepaper describing a sidechain proof-of-concept developed during an ErgoHack. *(ErgoHack)*
- [Ergohack Sidechain Repo](https://github.com/ross-weir/ergohack-sidechain) – Repository containing the code for the Ergohack sidechain PoC. [`Rust`?] *(ErgoHack)* | [Pragmaxim Spikechain PoC](https://github.com/pragmaxim/ergo-spikechain)
- [Stealth Address Docs (Aragogi)](https://github.com/aragogi/Stealth-doc) – Documentation related to a stealth address scanner/mixer concept. *(Community Concept, ErgoHack)*
- [Test Vectors - Transaction Serialization](https://github.com/ergoplatform/ergo-test-vectors/blob/master/src/test/resources/vector/tx_ser.json) – JSON file containing test vectors for Ergo transaction serialization. *(Official)*
- [Test Vectors - Signature Scheme](https://github.com/ergoplatform/ergo-test-vectors/blob/master/src/test/resources/vector/sig.json) – JSON file containing test vectors for Ergo's signature scheme. *(Official)*
- [Difficulty Algorithms (Zawy)](https://github.com/zawy12/difficulty-algorithms) – Research and analysis related to blockchain difficulty adjustment algorithms (relevant context for Ergo's algorithm). *(External Research)*
- **[Scorex](https://github.com/scorexfoundation/scorex)** – The modular blockchain framework upon which Ergo's core node implementation is built. [`Scala`] *(Foundation)* | [Hyperledger Labs Mirror](https://github.com/hyperledger-labs/Scorex)
- [P2S Address Conversion Tool](https://github.com/nitram147/ergo_mainnet_p2s_to_testnet_p2s) - Utility to convert P2S addresses between mainnet and testnet. [`Scala`?] *(Community Tool)*

### 🔩 Utilities <a id="utilities"></a>
*(Miscellaneous community tools & resources)*

- [ErgoTipper Token List](https://github.com/Luivatra/ergotipper-tokens) – Tokens recognized by the ErgoTipper Telegram bot. *(Community)*
- [Spectrum Token List](https://github.com/spectrum-finance/ergo-token-list) – Token list curated and used by the Spectrum Finance DEX. *(Community)*
- [ErgoToolsBot (Telegram)](https://t.me/ergotoolsbot) – Telegram bot with various utilities and information related to Ergo. [GitHub](https://github.com/ladopixel/ErgoToolsBot) [`Python`] *(Community)*
- [Matterbridge](https://github.com/42wim/matterbridge) – Software used for bridging various Ergo community chat platforms (Discord, Telegram). *(Tool)*
- [SharkNet](https://github.com/The-Last-Byte-Bar/SharkNet) – Community project creating a dataset of ErgoScript examples for potential AI/ML training. *(Community, Experimental)*
- [ErgoLLM](https://github.com/glasgowm148/ErgoLLM) – Experimental tooling exploring the use of Large Language Models (LLMs) with Ergo data and concepts. [`Python`] *(Community, Experimental)*
- [General Ergo Chatbot](https://www.chatbase.co/chatbot-iframe/zxB2uzZfYoHIpA98eTzgM) – AI assistant trained on general Ergo documentation *(External Tool)*.
- [ErgoScript Chatbot](https://www.chatbase.co/chatbot-iframe/INAIfQ2ts4E6ykf4rseVu) – AI assistant specifically focused on answering questions about ErgoScript *(External Tool)*.
- [Sigma Bot](https://github.com/cafebedouin/sigmabot) - Telegram bot for the Sigmanauts community? [`Python`] *(Community)* | [Eeysirhc Fork](https://github.com/Eeysirhc/sigmabot)
- [Ergo Champions Bot](https://github.com/Eeysirhc/ergo-champions-bot) - Telegram bot related to the Ergo Champions program. [`Python`] *(Community)*
- [Whale Alerts Twitter Bot](https://github.com/nirvanush/whale-alerts-twitter-bot) - Bot for monitoring and reporting large Ergo transactions on Twitter. [`TS`?] *(Community)*
- [Sigmanauts Community Site Code](https://github.com/cafebedouin/sigmanauts) - Code for the Sigmanauts community website. *(Community)* | [Rustinmyeye Fork](https://github.com/rustinmyeye/sigmanauts)
- [Sigmanauts List](https://github.com/rustinmyeye/list/) - Community maintained list, purpose unclear. *(Community)*

---

> **Tip:** bookmark this page and ⭐ star it on GitHub to stay in the loop. New tools appear every week!
