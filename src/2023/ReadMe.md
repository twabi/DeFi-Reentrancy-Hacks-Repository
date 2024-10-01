# DeFi Hacks Reproduce - Foundry (Reentrancy Attacks Only)

## 2023 - Reentrancy-Related Incidents

Below is a filtered list of DeFi incidents from 2023 where **reentrancy vulnerabilities** were exploited. Each entry includes details about the loss incurred, testing commands using Foundry, contract references, and relevant links for further information.

---

### 20231216 - NFTTrader - Reentrancy

#### Lost: ~$3M

**Testing**

```sh
forge test --contracts ./src/2023/test/NFTTrader_exp.sol -vvv
```

#### Contract

[NFTTrader_exp.sol](../../src/2023/test/NFTTrader_exp.sol)

#### Link References

- [Twitter - AnciliaInc](https://twitter.com/AnciliaInc/status/1736263884217139333)
- [Twitter - SlowMist Team](https://twitter.com/SlowMist_Team/status/1736005523550646535)
- [Twitter - 0xArhat](https://twitter.com/0xArhat/status/1736038250190651467)

---

### 20231216 - GoodDollar - Lack of Input Validation & Reentrancy

#### Lost: ~$2M

**Testing**

```sh
forge test --contracts ./src/2023/test/GoodDollar_exp.sol -vvv
```

#### Contract

[GoodDollar_exp.sol](../../src/2023/test/GoodDollar_exp.sol)

#### Link References

- [Twitter - MetaSec_xyz](https://twitter.com/MetaSec_xyz/status/1736428284756607386)

---

### 20231213 - CAROLProtocol - Price Manipulation Via Reentrancy

#### Lost: ~$53k

**Testing**

```sh
forge test --contracts ./src/2023/test/CAROLProtocol_exp.sol -vvv
```

#### Contract

[CAROLProtocol_exp.sol](../../src/2023/test/CAROLProtocol_exp.sol)

#### Link References

- [Twitter - MetaSec_xyz](https://x.com/MetaSec_xyz/status/1730496513359647167)

---

### 20231007 - StarsArena - Reentrancy

#### Lost: ~$3M

**Testing**

```sh
forge test --contracts ./src/2023/test/StarsArena_exp.sol -vvv
```

#### Contract

[StarsArena_exp.sol](../../src/2023/test/StarsArena_exp.sol)

#### Link References

- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1710556926986342911)
- [Twitter - Phalcon_xyz](https://twitter.com/Phalcon_xyz/status/1710554341466395065)
- [Twitter - PeckShield](https://twitter.com/peckshield/status/1710555944269292009)

---

### 20230926 - XSDWETHpool - Reentrancy

#### Lost: ~$56.9BNB

**Testing**

```sh
forge test --contracts ./src/2023/test/XSDWETHpool_exp.sol -vvv
```

#### Contract

[XSDWETHpool_exp.sol](../../src/2023/test/XSDWETHpool_exp.sol)

#### Link References

- [Twitter - CertiKAlert](https://twitter.com/CertiKAlert/status/1706765042916450781)

---

### 20230916 - uniclyNFT - Reentrancy

#### Lost: 1 NFT

**Testing**

```sh
forge test --contracts ./src/2023/test/uniclyNFT_exp.sol -vvv
```

#### Contract

[uniclyNFT_exp.sol](../../src/2023/test/uniclyNFT_exp.sol)

#### Link References

- [Twitter - DecurityHQ](https://twitter.com/DecurityHQ/status/1703096116047421863)

---

### 20230411 - Paribus - Reentrancy

#### Lost: $100k

**Testing**

```sh
forge test --contracts ./src/2023/test/Paribus_exp.sol -vvv
```

#### Contract

[Paribus_exp.sol](../../src/2023/test/Paribus_exp.sol)

#### Link References

- [Twitter - Phalcon_xyz](https://twitter.com/Phalcon_xyz/status/1645742620897955842)
- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1645744655357575170)
- [Twitter - PeckShield](https://twitter.com/peckshield/status/1645742296904929280)

---

### 20230405 - Sentiment - Read-Only-Reentrancy

#### Lost: $1M

**Testing**

```sh
forge test --contracts ./src/2023/test/Sentiment_exp.sol -vvv
```

#### Contract

[Sentiment_exp.sol](../../src/2023/test/Sentiment_exp.sol)

#### Link References

- [Twitter - PeckShield](https://twitter.com/peckshield/status/1643417467879059456)
- [Twitter - spreekaway](https://twitter.com/spreekaway/status/1643313471180644360)
- [Medium - CoinMonks](https://medium.com/coinmonks/theoretical-practical-balancer-and-read-only-reentrancy-part-1-d6a21792066c)

---

### 20230313 - EulerFinance - Reentrancy

#### Lost: ~$200M

**Testing**

```sh
forge test --contracts ./src/2023/test/Euler_exp.sol -vvv
```

#### Contract

[Euler_exp.sol](../../src/2023/test/Euler_exp.sol)

#### Link References

- [Twitter - FrankResearcher](https://twitter.com/FrankResearcher/status/1635241475989721089)
- [Twitter - nomorebear](https://twitter.com/nomorebear/status/1635230621856600064)
- [Twitter - PeckShield](https://twitter.com/peckshield/status/1635229594596036608)
- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1635262150624305153)

---

### 20230721 - Conic Finance - Read-Only-Reentrancy & MisConfiguration

#### Lost: ~$3.25M

**Testing**

```sh
forge test --contracts ./src/2023/test/Conic_exp.sol -vvv
```

#### Contract

[Conic_exp.sol](../../src/2023/test/Conic_exp.sol) | [Conic_exp2.sol](../../src/2023/test/Conic_exp2.sol)

#### Link References

- [Medium - ConicFinance](https://medium.com/@ConicFinance/post-mortem-eth-and-crvusd-omnipool-exploits-c9c7fa213a3d)
- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1682356244299010049)

---

### 20230711 - Libertify - Reentrancy

#### Lost: ~$452k

**Testing**

```sh
forge test --contracts ./src/2023/test/Libertify_exp.sol -vvv
```

#### Contract

[Libertify_exp.sol](../../src/2023/test/Libertify_exp.sol)

#### Link References

- [Twitter - PeckShield](https://twitter.com/peckshield/status/1678688731908411393)
- [Twitter - Phalcon_xyz](https://twitter.com/Phalcon_xyz/status/1678694679767031809)

---

### 20230710 - ArcadiaFi - Reentrancy

#### Lost: ~$400k

**Testing**

```sh
forge test --contracts ./src/2023/test/ArcadiaFi_exp.sol -vvv
```

#### Contract

[ArcadiaFi_exp.sol](../../src/2023/test/ArcadiaFi_exp.sol)

#### Link References

- [Twitter - Phalcon_xyz](https://twitter.com/Phalcon_xyz/status/1678250590709899264)
- [Twitter - PeckShield](https://twitter.com/peckshield/status/1678265212770693121)

---

### 20230612 - Sturdy Finance - Read-Only-Reentrancy

#### Lost: ~$800k

**Testing**

```sh
forge test --contracts ./src/2023/test/Sturdy_exp.sol -vvv
```

#### Contract

[Sturdy_exp.sol](../../src/2023/test/Sturdy_exp.sol)

#### Link References

- [Medium - SturdyFinance](https://sturdyfinance.medium.com/exploit-post-mortem-49261493307a)
- [Twitter - AnciliaInc](https://twitter.com/AnciliaInc/status/1668081008615325698)
- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1668084629654638592)

---

### 20230210 - dForce - Read-Only-Reentrancy

#### Lost: ~$3.65M

**Testing**

```sh
forge test --contracts ./src/2023/test/dForce_exp.sol -vvv
```

#### Contract

[dForce_exp.sol](../../src/2023/test/dForce_exp.sol)

#### Link References

- [Twitter - SlowMist_Team](https://twitter.com/SlowMist_Team/status/1623956763598000129)
- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1623901011680333824)
- [Twitter - PeckShield](https://twitter.com/peckshield/status/1623910257033617408)

---

### 20230116 - MidasCapital - Read-only Reentrancy

#### Lost: ~$650k

**Testing**

```sh
forge test --contracts ./src/2023/test/Midas_exp.sol -vvv
```

#### Contract

[Midas_exp.sol](../../src/2023/test/Midas_exp.sol)

#### Link References

- [Twitter - PeckShield](https://twitter.com/peckshield/status/1614774855999844352)
- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1614864084956254209)

---

### 20230203 - Orion Protocol - Reentrancy

#### Lost: $3M

**Testing**

```sh
forge test --contracts ./src/2023/test/Orion_exp.sol -vvv
```

#### Contract

[Orion_exp.sol](../../src/2023/test/Orion_exp.sol)

#### Link References

- [Twitter - PeckShield](https://twitter.com/peckshield/status/1621337925228306433)
- [Twitter - BlockSecTeam](https://twitter.com/BlockSecTeam/status/1621263393054420992)
- [NumenCyber Analysis](https://www.numencyber.com/analysis-of-orionprotocol-reentrancy-attack-with-poc/)

---

## Transaction Debugging Tools

- [Phalcon](https://explorer.phalcon.xyz/)
- [Tx Tracer](https://openchain.xyz/trace)
- [Cruise](https://cruise.supremacy.team/)
- [EthTx](https://ethtx.info/)
- [Tenderly](https://dashboard.tenderly.co/explorer)
- [EigenPhi](https://tx.eigenphi.io/analyseTransaction)

## Ethereum Signature Database

- [4byte](https://www.4byte.directory/)
- [Sig DB](https://openchain.xyz/signatures)
- [EtherFace](https://www.etherface.io/hash)

## Useful Tools

- [ABI to Interface](https://gnidan.github.io/abi-to-sol/)
- [Get ABI for Unverified Contracts](https://abi.w1nt3r.xyz/)
- [ETH Calldata Decoder](https://apoorvlathey.com/eth-calldata-decoder/)
- [ETHCMD - Guess ABI](https://www.ethcmd.com/tools/decode-calldata/)
- [Abi Tools](https://openchain.xyz/tools/abi)

## Hacks Dashboard

- [Slowmist](https://hacked.slowmist.io/)
- [Defillama](https://defillama.com/hacks)
- [De.Fi](https://de.fi/rekt-database)
- [Rekt](https://rekt.news/)
- [Cryptosec](https://cryptosec.info/defi-hacks/)

---

### View Gas Reports

Foundry also has the ability to [report](https://book.getfoundry.sh/forge/gas-reports) the `gas` used per function call, which mimics the behavior of [hardhat-gas-reporter](https://github.com/cgewecke/hardhat-gas-reporter). Generally speaking, if gas costs per function call are very high, then the likelihood of its success is reduced. Gas optimization is an important activity done by smart contract developers.

Every PoC in this repository can produce a gas report like this:

```bash
forge test --gas-report --contracts <contract> -vvv
```

**For Example:**

Let us find out the gas used in the [JAY PoC](../../src/2023/test/JAY_exp.sol)

**Execution**

```bash
forge test --gas-report --contracts ./src/2023/test/JAY_exp.sol -vvv
```

_**Demo**_

![JAY PoC Gas Report](./JAYPocGasReport.gif)

### Bug Reproduce

Moved to [DeFiVulnLabs](https://github.com/SunWeb3Sec/DeFiVulnLabs)

### FlashLoan Testing

Moved to [DeFiLabs](https://github.com/SunWeb3Sec/DeFiLabs)

---

## Summary

The above README focuses on DeFi incidents involving **reentrancy attacks** in **2023**. Each incident provides details including the date, project name, loss amount, testing commands, contract links, and relevant references for further information. This targeted approach helps in understanding the common vulnerabilities exploited in the DeFi space and aids in developing strategies to prevent similar attacks in the future.
