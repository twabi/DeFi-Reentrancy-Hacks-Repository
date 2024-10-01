

# DeFi Hacks Reproduce - Foundry

## 2022 - List of Past DeFi Incidents

13 incidents included.

- [20221229 JAY](#20221229---jay---insufficient-validation--reentrancy)
- [20221223 Defrost](#20221223---defrost---reentrancy)
- [20221110 DFXFinance](#20221110---dfxfinance---reentrancy)
- [20221026 N00d Token](#20221026-n00d-token---reentrancy)
- [20221024 Market](#20221024-market---read-only-reentrancy)
- [20221001 Thunder Brawl](#20221001-thunder-brawl---reentrancy)
- [20220710 Omni NFT](#20220710-omni-nft---reentrancy)
- [20220430 Rari Capital/Fei Protocol](#20220430-rari-capitalfei-protocol---flashloan-attack--reentrancy)
- [20220327 Revest Finance](#20220327-revest-finance---reentrancy)
- [20220315 Agave Finance](#20220315-agave-finance---erc667-reentrancy)
- [20220315 Hundred Finance](#20220315-hundred-finance---erc667-reentrancy)
- [20220313 Paraluni](#20220313-paraluni---flashloan--reentrancy)
- [20220305 Bacon Protocol](#20220305-bacon-protocol---reentrancy)

---

### 20221229 - JAY - Insufficient Validation & Reentrancy

#### Lost: ~15.32 ETH

**Testing**

```sh
forge test --contracts ./src/2022/test/JAY_exp.sol -vvv
```

#### Contract

[JAY_exp.sol](../../src/2022/test/JAY_exp.sol)

#### Link References

- [BlockSec Team Tweet](https://twitter.com/BlockSecTeam/status/1608372475225866240)

---

### 20221223 - Defrost - Reentrancy

#### Lost: $170k

**Testing**

```sh
forge test --contracts ./src/2022/test/Defrost_exp.sol -vvv
```

#### Contract

[Defrost_exp.sol](../../src/2022/test/Defrost_exp.sol)

#### Link References

- [PeckShield Alert Tweet](https://twitter.com/PeckShieldAlert/status/1606276020276891650)

---

### 20221110 - DFXFinance - Reentrancy

#### Lost: $4M

**Testing**

```sh
forge test --contracts ./src/2022/test/DFX_exp.sol -vvv
```

#### Contract

[DFX_exp.sol](../../src/2022/test/DFX_exp.sol)

#### Link References

- [BlockSec Team Tweet](https://twitter.com/BlockSecTeam/status/1590960299246780417)
- [Beosin Alert Tweet](https://twitter.com/BeosinAlert/status/1591012525914861570)
- [AnciliaInc Tweet](https://twitter.com/AnciliaInc/status/1590839104731684865)
- [PeckShield Tweet](https://twitter.com/peckshield/status/1590831589004816384)

---

### 20221026 - N00d Token - Reentrancy

#### Lost: $29k

**Testing**

```sh
forge test --contracts ./src/2022/test/N00d_exp.sol -vvv
```

#### Contract

[N00d_exp.sol](../../src/2022/test/N00d_exp.sol)

#### Link References

- [BlockSec Team Tweet](https://twitter.com/BlockSecTeam/status/1584959295829180416)
- [AnciliaInc Tweet](https://twitter.com/AnciliaInc/status/1584955717877784576)

---

### 20221024 - Market - Read-only Reentrancy

#### Lost: $220k

**Testing**

```sh
forge test --contracts ./src/2022/test/Market_exp.sol -vv
```

#### Contract

[Market_exp.sol](../../src/2022/test/Market_exp.sol)

#### Link References

- [Quillaudits Medium Analysis](https://quillaudits.medium.com/decoding-220k-read-only-reentrancy-exploit-quillaudits-30871d728ad5)

---

### 20221001 - Thunder Brawl - Reentrancy

#### Lost: [Amount Not Specified]

**Testing**

```sh
forge test --contracts ./src/2022/test/THB_exp.sol -vv
```

#### Contract

[THB_exp.sol](../../src/2022/test/THB_exp.sol)

#### Link References

- [PeckShield Tweet](https://twitter.com/peckshield/status/1575890733373849601)
- [BscScan Transaction](https://bscscan.com/tx/0x57aa9c85e03eb25ac5d94f15f22b3ba3ab2ef60b603b97ae76f855072ea9e3a0)

---

### 20220710 - Omni NFT - Reentrancy

#### Lost: $1.4M

**Testing**

```sh
forge test --contracts ./src/2022/test/Omni_exp.sol -vv
```

#### Contract

[Omni_exp.sol](../../src/2022/test/Omni_exp.sol)

#### Link References

- [SlowMist Team Tweet](https://twitter.com/SlowMist_Team/status/1546379086792388609)
- [Etherscan Transaction](https://etherscan.io/tx/0x05d65e0adddc5d9ccfe6cd65be4a7899ebcb6e5ec7a39787971bcc3d6ba73996)

---

### 20220430 - Rari Capital/Fei Protocol - Flashloan Attack & Reentrancy

#### Lost: $80 million

**Testing**

```sh
forge test --contracts ./src/2022/test/Rari_exp.sol -vv
```

#### Contract

[Rari_exp.sol](../../src/2022/test/Rari_exp.sol)

#### Link References

- [CertiK Medium Analysis](https://certik.medium.com/fei-protocol-incident-analysis-8527440696cc)
- [PeckShield Tweet](https://twitter.com/peckshield/status/1520369315698016256)
- [Etherscan Transaction](https://etherscan.io/tx/0xab486012f21be741c9e674ffda227e30518e8a1e37a5f1d58d0b0d41f6e76530)

---

### 20220327 - Revest Finance - Reentrancy

#### Lost: $11.2 million

**Testing**

```sh
forge test --contracts ./src/2022/test/Revest_exp.sol -vv
```

#### Contract

[Revest_exp.sol](../../src/2022/test/Revest_exp.sol)

#### Link References

- [BlockSec Team Medium Article](https://blocksecteam.medium.com/revest-finance-vulnerabilities-more-than-re-entrancy-1609957b742f)
- [Etherscan Transaction](https://etherscan.io/tx/0xe0b0c2672b760bef4e2851e91c69c8c0ad135c6987bbf1f43f5846d89e691428)

---

### 20220315 - Agave Finance - ERC667 Reentrancy

#### Lost: $1.5 million

**Testing**

```sh
forge test --contracts ./src/2022/test/Agave_exp.sol -vv
```

#### Contract

[Agave_exp.sol](../../src/2022/test/Agave_exp.sol)

#### Link References

- [Agave Finance Exploit Analysis](https://medium.com/agavefinance/agave-exploit-reentrancy-in-liquidation-call-51ae407bc56)
- [GnosisScan Transaction](https://gnosisscan.io/tx/0xa262141abcf7c127b88b4042aee8bf601f4f3372c9471dbd75cb54e76524f18e)

---

### 20220315 - Hundred Finance - ERC667 Reentrancy

#### Lost: $1.7 million

**Testing**

```sh
forge test --contracts ./src/2022/test/HundredFinance_exp.sol -vvv
```

#### Contract

[HundredFinance_exp.sol](../../src/2022/test/HundredFinance_exp.sol)

#### Link References

- [Immunefi Medium Post](https://medium.com/immunefi/a-poc-of-the-hundred-finance-heist-4121f23a098)
- [GnosisScan Transaction](https://gnosisscan.io/tx/0x534b84f657883ddc1b66a314e8b392feb35024afdec61dfe8e7c510cfac1a098)

---

### 20220313 - Paraluni - Flashloan & Reentrancy

#### Lost: $1.7 million

**Testing**

```sh
forge test --contracts ./src/2022/test/Paraluni_exp.sol -vv
```

#### Contract

[Paraluni_exp.sol](../../src/2022/test/Paraluni_exp.sol)

#### Link References

- [Halborn Exploit Analysis](https://halborn.com/explained-the-paraluni-hack-march-2022/)
- [PeckShield Tweet](https://twitter.com/peckshield/status/1502815435498176514)
- [Paraluni Official Tweet](https://mobile.twitter.com/paraluni/status/1502951606202994694)
- [Zhihu Article](https://zhuanlan.zhihu.com/p/517535530)
- [BscScan Transaction](https://bscscan.com/tx/0x70f367b9420ac2654a5223cc311c7f9c361736a39fd4e7dff9ed1b85bab7ad54)

---

### 20220305 - Bacon Protocol - Reentrancy

#### Lost: $1 million

**Testing**

```sh
forge test --contracts ./src/2022/test/Bacon_exp.sol -vv
```

#### Contract

[Bacon_exp.sol](../../src/test/2022/test/Bacon_exp.sol)

#### Link References

- [PeckShield Tweet](https://twitter.com/peckshield/status/1500105933128495108)
- [Etherscan Transaction 1](https://etherscan.io/tx/0xacfcaa8e1c482148f9f2d592c78ca7a27934c7333dab31978ed0aef333a28ab6)
- [Etherscan Transaction 2](https://etherscan.io/tx/0x7d2296bcb936aa5e2397ddf8ccba59f54a178c3901666b49291d880369dbcf31)

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

Let us find out the gas used in the [JAY PoC](../../src/2022/test/JAY_exp.sol)

**Execution**

```bash
forge test --gas-report --contracts ./src/2022/test/JAY_exp.sol -vvv
```

_**Demo**_

![JAY PoC Gas Report](./JAYPocGasReport.gif)

### Bug Reproduce

Moved to [DeFiVulnLabs](https://github.com/SunWeb3Sec/DeFiVulnLabs)

### FlashLoan Testing

Moved to [DeFiLabs](https://github.com/SunWeb3Sec/DeFiLabs)

---

## Summary

The above README focuses on DeFi incidents involving **reentrancy attacks** in **2022**. Each incident provides details including the date, project name, loss amount, testing commands, contract links, and relevant references for further information. This targeted approach helps in understanding the common vulnerabilities exploited in the DeFi space and aids in developing strategies to prevent similar attacks in the future.
