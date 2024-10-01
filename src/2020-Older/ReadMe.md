
# DeFi Reentrancy Hacks Before 2021 - Foundry

**Reproduce DeFi reentrancy hack incidents using Foundry.**

Join [Discord](https://discord.gg/Fjyngakf3h) to help make Web3 secure!

**Disclaimer:**  
This content serves solely as a proof of concept showcasing past DeFi hacking incidents. It is strictly intended for educational purposes and should not be interpreted as encouraging or endorsing any form of illegal activities or actual hacking attempts. The provided information is for informational and learning purposes only, and any actions taken based on this content are solely the responsibility of the individual. The usage of this information should adhere to applicable laws, regulations, and ethical standards.

---

## List of Reentrancy Attacks Before 2021 (2020 and Older)

1. [20181007 - SpankChain - Reentrancy](#20181007---spankchain---reentrancy)
2. [20200419 - LendfMe - ERC777 Reentrancy](#20200419---lendfme---erc777-reentrancy)
3. [20200418 - UniSwapV1 - ERC777 Reentrancy](#20200418---uniswaptv1---erc777-reentrancy)
4. [20171106 - Parity - 'Accidentally Killed It'](#20171106---parity---accidentally-killed-it)

---

### 20181007 - SpankChain - Reentrancy

#### Lost: Not Specified

**Testing**

```sh
forge test --contracts ./src/2018/test/SpankChain_exp.sol -vvv
```

#### Contract

[SpankChain_exp.sol](../../src/2018/test/SpankChain_exp.sol)

#### Link References

- [SpankChain Exploit Details](#) *(Please replace `#` with the actual URL if available)*

---

### 20200419 - LendfMe - ERC777 Reentrancy

#### Lost: Not Specified

**Testing**

```sh
forge test --contracts ./src/2020/test/LendfMe_exp.sol -vvv
```

#### Contract

[LendfMe_exp.sol](../../src/2020/test/LendfMe_exp.sol)

#### Link References

- [LendfMe Exploit Analysis](#) *(Please replace `#` with the actual URL if available)*

---

### 20200418 - UniSwapV1 - ERC777 Reentrancy

#### Lost: Not Specified

**Testing**

```sh
forge test --contracts ./src/2020/test/UniSwapV1_exp.sol -vvv
```

#### Contract

[UniSwapV1_exp.sol](../../src/2020/test/UniSwapV1_exp.sol)

#### Link References

- [UniSwapV1 Exploit Details](#) *(Please replace `#` with the actual URL if available)*

---

### 20171106 - Parity - 'Accidentally Killed It'

#### Lost: Not Specified

**Testing**

```sh
forge test --contracts ./src/2017/test/Parity_exp.sol -vvv
```

#### Contract

[Parity_exp.sol](../../src/2017/test/Parity_exp.sol)

#### Link References

- [Parity Multisig Wallet Hack](#) *(Please replace `#` with the actual URL if available)*

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

Let us find out the gas used in the [SpankChain PoC](../../src/2018/test/SpankChain_exp.sol)

**Execution**

```bash
forge test --gas-report --contracts ./src/2018/test/SpankChain_exp.sol -vvv
```

_**Demo**_

![SpankChain PoC Gas Report](./SpankChainPocGasReport.gif)

---

## Bug Reproduce

Moved to [DeFiVulnLabs](https://github.com/SunWeb3Sec/DeFiVulnLabs)

## FlashLoan Testing

Moved to [DeFiLabs](https://github.com/SunWeb3Sec/DeFiLabs)

---

## Summary

The above README focuses on DeFi incidents involving **reentrancy attacks** before **2021** (2020 and older). Each incident provides details including the date, project name, loss amount, testing commands, contract links, and relevant references for further information. This targeted approach helps in understanding the common vulnerabilities exploited in the DeFi space and aids in developing strategies to prevent similar attacks in the future.
