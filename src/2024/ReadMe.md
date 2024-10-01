
# DeFi Reentrancy Hacks 2024 - Foundry

**Reproduce DeFi reentrancy hack incidents using Foundry.**

Join [Discord](https://discord.gg/Fjyngakf3h) to help make Web3 secure!

**Disclaimer:**  
This content serves solely as a proof of concept showcasing past DeFi hacking incidents. It is strictly intended for educational purposes and should not be interpreted as encouraging or endorsing any form of illegal activities or actual hacking attempts. The provided information is for informational and learning purposes only, and any actions taken based on this content are solely the responsibility of the individual. The usage of this information should adhere to applicable laws, regulations, and ethical standards.

---

## List of Reentrancy Attacks in 2024

1. [20240903 - Penpiexyz_io - Reentrancy and Reward Manipulation](#20240903---penpiexyz_io---reentrancy-and-reward-manipulation)
2. [20240714 - Minterest - Reentrancy](#20240714---minterest---reentrancy)
3. [20240702 - MRP - Reentrancy](#20240702---mrp---reentrancy)
4. [20240529 - PredyFinance - Reentrancy](#20240529---predyfinance---reentrancy)
5. [20240514 - PredyFinance - Reentrancy](#20240514---predyfinance---reentrancy)
6. [20240228 - SMOOFSStaking - Reentrancy](#20240228---smoofsstaking---reentrancy)
7. [20240125 - NBLGAME - Reentrancy](#20240125---nblgame---reentrancy)
8. [20240128 - BarleyFinance - Reentrancy](#20240128---barleyfinance---reentrancy)

---

### 20240903 - Penpiexyz_io - Reentrancy and Reward Manipulation

#### Lost: 11,113.6 ETH (~$27,348,259 USD)

**Testing**

```sh
forge test --contracts ./src/2024/test/Penpiexyzio_exp.sol -vvv --evm-version shanghai
```

#### Contract

[Penpiexyzio_exp.sol](../../src/2024/test/Penpiexyzio_exp.sol)

#### Link References

- [PeckShield Report](https://x.com/peckshield/status/1831072098669953388)
- [AnciliaInc Report](https://x.com/AnciliaInc/status/1831080555292856476)
- [HackenClub Report](https://x.com/hackenclub/status/1831383106554573099)
- [Post-Mortem](https://x.com/Penpiexyz_io/status/1831462760787452240)

---

### 20240714 - Minterest - Reentrancy

#### Lost: ~427 ETH

**Testing**

```sh
forge test --contracts ./src/2024/test/Minterest_exp.sol -vvv
```

#### Contract

[Minterest_exp.sol](../../src/2024/test/Minterest_exp.sol)

#### Link References

- [0xNickLFranklin Tweet](https://x.com/0xNickLFranklin/status/1813122959219040323)

---

### 20240702 - MRP - Reentrancy

#### Lost: 17 BNB

**Testing**

```sh
forge test --contracts ./src/2024/test/MRP_exp.sol -vvv
```

#### Contract

[MRP_exp.sol](../../src/2024/test/MRP_exp.sol)

#### Link References

- [0xNickLFranklin Tweet](https://x.com/0xNickLFranklin/status/1808309614443733005)

---

### 20240529 - PredyFinance - Reentrancy

#### Lost: $464K

**Testing**

```sh
forge test --contracts ./src/2024/test/PredyFinance_exp.sol -vvv
```

#### Contract

[PredyFinance_exp.sol](../../src/2024/test/PredyFinance_exp.sol)

#### Link References

- [Phalcon_xyz Tweet](https://twitter.com/Phalcon_xyz/status/1790307019590680851)

---

### 20240514 - PredyFinance - Reentrancy

#### Lost: $464K

**Testing**

```sh
forge test --contracts ./src/2024/test/PredyFinance_exp.sol -vvv
```

#### Contract

[PredyFinance_exp.sol](../../src/2024/test/PredyFinance_exp.sol)

#### Link References

- [Phalcon_xyz Tweet](https://twitter.com/Phalcon_xyz/status/1790307019590680851)

---

### 20240228 - SMOOFSStaking - Reentrancy

#### Lost: Unclear

**Testing**

```sh
forge test --contracts ./src/2024/test/SMOOFSStaking_exp.sol -vvv
```

#### Contract

[SMOOFSStaking_exp.sol](../../src/2024/test/SMOOFSStaking_exp.sol)

#### Link References

- [AnciliaInc Tweet](https://twitter.com/AnciliaInc/status/1762893563103428783)
- [0xNickLFranklin Tweet](https://twitter.com/0xNickLFranklin/status/1762895774311178251)

---

### 20240125 - NBLGAME - Reentrancy

#### Lost: ~180K

**Testing**

```sh
forge test --contracts ./src/2024/test/NBLGAME_exp.sol -vvv
```

#### Contract

[NBLGAME_exp.sol](../../src/2024/test/NBLGAME_exp.sol)

#### Link References

- [SlowMist_Team Tweet](https://twitter.com/SlowMist_Team/status/1750526097106915453)
- [AnciliaInc Tweet](https://twitter.com/AnciliaInc/status/1750558426382635036)

---

### 20240128 - BarleyFinance - Reentrancy

#### Lost: ~130K

**Testing**

```sh
forge test --contracts ./src/2024/test/BarleyFinance_exp.sol -vvv
```

#### Contract

[BarleyFinance_exp.sol](../../src/2024/test/BarleyFinance_exp.sol)

#### Link References

- [Phalcon_xyz Tweet](https://twitter.com/Phalcon_xyz/status/1751788389139992824)
- [PeckShieldAlert Tweet](https://twitter.com/PeckShieldAlert/status/1752279373779194011)

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

## View Gas Reports

Foundry also has the ability to [report](https://book.getfoundry.sh/forge/gas-reports) the `gas` used per function call, which mimics the behavior of [hardhat-gas-reporter](https://github.com/cgewecke/hardhat-gas-reporter). Generally speaking, if gas costs per function call are very high, then the likelihood of its success is reduced. Gas optimization is an important activity done by smart contract developers.

Every PoC in this repository can produce a gas report like this:

```bash
forge test --gas-report --contracts <contract> -vvv
```

**For Example:**

Let us find out the gas used in the [Penpiexyz_io PoC](../../src/2024/test/Penpiexyzio_exp.sol)

**Execution**

```bash
forge test --gas-report --contracts ./src/2024/test/Penpiexyzio_exp.sol -vvv
```

_**Demo**_

![Penpiexyz_io PoC Gas Report](./PenpiexyzioPocGasReport.gif)

---

## Bug Reproduce

Moved to [DeFiVulnLabs](https://github.com/SunWeb3Sec/DeFiVulnLabs)

## FlashLoan Testing

Moved to [DeFiLabs](https://github.com/SunWeb3Sec/DeFiLabs)

---

## Summary

The above README focuses on DeFi incidents involving **reentrancy attacks** in **2024**. Each incident provides details including the date, project name, loss amount, testing commands, contract links, and relevant references for further information. This targeted approach helps in understanding the common vulnerabilities exploited in the DeFi space and aids in developing strategies to prevent similar attacks in the future.
