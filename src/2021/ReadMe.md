
# DeFi Hacks Reproduce - Foundry

## 2021 - List of DeFi Incidents Involving Reentrancy

7 incidents included.

- [20211221 Visor Finance](#20211221-visor-finance---reentrancy)
- [20211218 Grim Finance](#20211218-grim-finance---flashloan--reentrancy)
- [20210830 Cream Finance](#20210830-cream-finance---flashloan-attack--reentrancy)
- [20210817 XSURGE](#20210817-xsurge---flashloan-attack--reentrancy)
- [20210527 BurgerSwap](#20210527-burgerswap---mathematical-flaw--reentrancy)
- [20210509 RariCapital](#20210509-raricapital---cross-contract-reentrancy)
- [20210508 Value Defi](#20210508-value-defi---cross-contract-reentrancy)

---

### 20211221 - Visor Finance - Reentrancy

#### Lost: $8.2 million

**Testing**

```sh
forge test --contracts ./src/2021/test/Visor_exp.sol -vv
```

#### Contract

[Visor_exp.sol](../../src/2021/test/Visor_exp.sol)

#### Link References

- [Beosin Analysis](https://beosin.medium.com/two-vulnerabilities-in-one-function-the-analysis-of-visor-finance-exploit-a15735e2492)
- [Gamma Strategies Tweet](https://twitter.com/GammaStrategies/status/1473306777131405314)
- [Etherscan Transaction](https://etherscan.io/tx/0x69272d8c84d67d1da2f6425b339192fa472898dce936f24818fda415c1c1ff3f)

---

### 20211218 - Grim Finance - Flashloan & Reentrancy

#### Lost: $30 million

**Testing**

```sh
forge test --contracts ./src/2021/test/Grim_exp.sol -vv
```

#### Contract

[Grim_exp.sol](../../src/2021/test/Grim_exp.sol)

#### Link References

- [Cointelegraph Article](https://cointelegraph.com/news/defi-protocol-grim-finance-lost-30m-in-5x-reentrancy-hack)
- [Rekt.News Report](https://rekt.news/grim-finance-rekt/)
- [Etherscan Transaction](https://ftmscan.com/tx/0x19315e5b150d0a83e797203bb9c957ec1fa8a6f404f4f761d970cb29a74a5dd6)

---

### 20210830 - Cream Finance - Flashloan Attack + Reentrancy

#### Lost: $18 million

**Testing**

```sh
forge test --contracts ./src/2021/test/Cream_exp.sol -vvv
```

#### Contract

[Cream_exp.sol](../../src/2021/test/Cream_exp.sol)

#### Link References

- [Immunefi Postmortem](https://medium.com/immunefi/hack-analysis-cream-finance-oct-2021-fc222d913fc5)
- [PeckShield Tweet](https://twitter.com/peckshield/status/1432249600002478081)
- [Cream Finance Tweet](https://twitter.com/creamdotfinance/status/1432249773575208964)
- [Etherscan Transaction](https://etherscan.io/tx/0xa9a1b8ea288eb9ad315088f17f7c7386b9989c95b4d13c81b69d5ddad7ffe61e)

---

### 20210817 - XSURGE - Flashloan Attack + Reentrancy

#### Lost: $5 million

**Testing**

```sh
forge test --contracts ./src/2021/test/XSURGE_exp.sol -vv
```

#### Contract

[XSURGE_exp.sol](../../src/2021/test/XSURGE_exp.sol)

#### Link References

- [Beosin Medium Analysis](https://beosin.medium.com/a-sweet-blow-fb0a5e08657d)
- [Knownsec Blockchain Lab Postmortem](https://medium.com/@Knownsec_Blockchain_Lab/knownsec-blockchain-lab-comprehensive-analysis-of-xsurge-attacks-c83d238fbc55)
- [BscScan Transaction](https://bscscan.com/tx/0x8c93d6e5d6b3ec7478b4195123a696dbc82a3441be090e048fe4b33a242ef09d)

---

### 20210527 - BurgerSwap - Mathematical Flaw + Reentrancy

#### Lost: [Amount Not Specified]

**Testing**

```sh
forge test --contracts ./src/2021/test/BurgerSwap_exp.sol -vv
```

#### Contract

[BurgerSwap_exp.sol](../../src/2021/test/BurgerSwap_exp.sol)

#### Link References

- [Mudit Gupta Tweet](https://twitter.com/Mudit__Gupta/status/1398156036574306304)

---

### 20210509 - RariCapital - Cross Contract Reentrancy

#### Lost: [Amount Not Specified]

**Testing**

```sh
forge test --contracts ./src/2021/test/RariCapital_exp.sol -vv
```

#### Contract

[RariCapital_exp.sol](../../src/2021/test/RariCapital_exp.sol)

#### Link References

- [Rekt.News Report](https://rekt.news/rari-capital-rekt/)
- [Etherscan Transaction](https://etherscan.com/tx/0x171072422efb5cd461546bfe986017d9b5aa427ff1c07ebe8acc064b13a7b7be)

---

### 20210508 - Value Defi - Cross Contract Reentrancy

#### Lost: [Amount Not Specified]

**Testing**

```sh
forge test --contracts ./src/2021/test/ValueDefi_exp.sol -vv
```

#### Contract

[ValueDefi_exp.sol](../../src/2021/test/ValueDefi_exp.sol)

#### Link References

- [Rekt.News Report](https://rekt.news/rari-capital-rekt/)
- [BscScan Transaction](https://bscscan.com/tx/0xa00def91954ba9f1a1320ef582420d41ca886d417d996362bf3ac3fe2bfb9006)

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

Let us find out the gas used in the [Visor Finance PoC](../../src/2021/test/Visor_exp.sol)

**Execution**

```bash
forge test --gas-report --contracts ./src/2021/test/Visor_exp.sol -vvv
```

_Demo_

![Visor Finance PoC Gas Report](./VisorFinancePocGasReport.gif)

### Bug Reproduce

Moved to [DeFiVulnLabs](https://github.com/SunWeb3Sec/DeFiVulnLabs)

### FlashLoan Testing

Moved to [DeFiLabs](https://github.com/SunWeb3Sec/DeFiLabs)

---

## Summary

The above README focuses on DeFi incidents involving **reentrancy attacks** in **2021**. Each incident provides details including the date, project name, loss amount, testing commands, contract links, and relevant references for further information. This targeted approach helps in understanding the common vulnerabilities exploited in the DeFi space and aids in developing strategies to prevent similar attacks in the future.
