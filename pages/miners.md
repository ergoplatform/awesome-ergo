# Autolykos

Ergo has a strictly limited supply, an 8‐year emission schedule and a declining rate of emission over these 8 years. All tokens are mined through an original Asic and  Proof‐of‐Work (“PoW”) algorithm called [Autolykos](https://ergonaut.space/en/Autolykos), which employs a [non-linear difficulty algorithm](https://www.docdroid.net/mcoitvK/ergopow-pdf#page=2). Therefore, there are 0 Ergs in existence at launch of mainnet as there was no ICO nor pre‐mine. At the end of 8 years, the final Erg supply will be 97,739,925 Ergs. The Ergo block interval is 2 minutes and for the first 2 years, each block will release a total of 75 Ergs to be shared between the miners and the Treasury (Treasury discussed below). But starting at year 2, the rate of emission will fall by 3.0 Ergs and thereafter further decline every 3 months by an additional 3.0 Ergs, which will result in an end to emission 8 years after launch. There will be no additional inflation and the Erg monetary base will remain fixed. The [emission schedule chart](https://ergoplatform.org/en/blog/2019_05_20-curve/) illustrates this.

The [explorer](explorer.ergoplatform.com/) can give you various information & stats on mining and the network. 

## Hashrate

- [Mining Pool Stats](https://miningpoolstats.stream/ergo)
- [(Repsonses) Hashrates and GPU settings](https://docs.google.com/spreadsheets/d/1NsuoDB27EwCo_BlSjCP3GMLfTSJRPIWIBsL-wPTllUg/edit#gid=1675061291)
- [Mining Stats Submission Form](https://docs.google.com/forms/d/e/1FAIpQLSfvRg_I5QumCBmMCwOHzel6bt5OOAA0uvJl_PBdKEtlpbRnVQ/viewform)



## Difficulty 

Ergo uses a non-linear algorithm which smoothes over 8 epochs. This was designed to prevent coin-hopping and time warp attacks.

The [difficulty over time](https://explorer.ergoplatform.com/en/charts/difficulty) is visible here. If you want an estimate of what might be next you can observe the 
[Difficulty and epoch monitor.](http://cds.oette.info/ergo_diff.htm)


# Mining Requirements

To start mining you need an Ergo wallet, a compatible GPU, a miner program, and a pool.

A 6GB GPU is the suggested minimum as Ergo heavily relies on memory usage while the core processor sits idle.

Search your card here [Autolykos v2 hashrates](https://www.ergoforum.org/t/autolykos-v2-hashrates/580) to find the hashrate. 


For the [AMD miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner), the compatible Operating Systems are
- RedHat Enterprise Linux 7.2 (64-bit version)
- RedHat Enterprise Linux 6.8 (64-bit version)
- Ubuntu 16.04 (64-bit version)

Ergo can also be mined with [Nvidia miner](https://github.com/mhssamadani/Autolykos2_NV_Miner)


- Miners can fix value by minting [SigUSD](https://sigmausd.io/#/)


## Other Miners

- [CUDA-based GPU miner for Ergo](https://github.com/ergoplatform/Autolykos-GPU-miner) for NVidia cards
- [OpenCL miner for ERGO](https://github.com/mhssamadani/ergoAMDminer) for AMD cards 
- [ErgoPool - mining pool for self-sovereign Ergo miners!](https://ergopool.io/)
- [#smartpools](https://discord.gg/qdEpkRQZ4P) 

**Calculators**

- [ErgoPlatform - Mining Calculator](https://ergoplatform.org/en/mining/)
- [Plutomonkey Calculator](https://pool.plutomonkey.com/)
- [Miner Stats](https://minerstat.com/coin/erg)

# Guides

- [Mining $ERG: The Complete Guide](https://thecryptodrip.com/how-to-mine-erg-guide/)
- [ErgoForum: Mining Ergo for Fun and Profit](https://www.ergoforum.org/t/mining-ergo-for-fun-and-profit/154)
- [ErgoPlatform: Mining Ergo for Fun and Profit](https://ergoplatform.org/en/blog/2019_12_22_mining_for_fun/)
- [ErgoForum: Q&A on mining (for pool operators and solo miners)](https://www.ergoforum.org/t/q-a-on-mining-for-pool-operators-and-solo-miners/587)
- [How to set up and configure a full Ergo node on Windows (Youtube)](https://www.youtube.com/watch?v=fpEDJ1CM6ns)
- [Full node set-up](https://git.io/fjqwx)
- [Start mining](https://git.io/fjqwp)

# Pools


**WoolyPooly**
- [How to start mining Ergo (ERG) on Windows with AMD RX 4GB cards!!! Step by Step (Youtube)](https://www.youtube.com/watch?v=47eBVIjWYqY)

**HeroMiners**
- [Hero Miners: How to Mine Ergo (ERG)? Complete Beginner’s Guide](https://herominers.medium.com/how-to-mine-ergo-erg-complete-beginners-guide-608a87e89ed6)
- [HeroMiners: How to mine Erg](https://ergo.herominers.com/#how-to-mine-ergo-erg)
- [How to Mine Ergo? Step by Step (Youtube)](https://www.youtube.com/watch?v=4SnpCF67kyc)

**SRBminer**
- [SRBMiner-MULTI - How to mine Ergo coin (autolykos2)](https://www.youtube.com/watch?v=thBPstQJVWo)


> There are active miner communities for Ergo on [Discord](https://discord.gg/Q86PNMwRsu) and [Telegram](https://t.me/ergo_mining)

## Host A Pool

Currently the [#host-a-pool](https://discord.gg/kxbrHVwnm5) on Discord is the best place to get support configuring a pool. 

- [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy) | Miner Connection + Work Management
- [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer) |  Pool Server
- [ergo-nomp](https://github.com/btclinux/ergo-nomp) | Node open mining portal configufed for ergo

### Step by Step 

1. Setup a Node
2. Setup ErgoStratumServer
3. Point [ergo-nomp](https://github.com/btclinux/ergo-nomp) to (1) and (2).