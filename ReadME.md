# DeFi Reentrancy Hacks Repository - Foundry

Welcome to the **DeFi Reentrancy Hacks Repository**, a comprehensive collection of decentralized finance (DeFi) reentrancy attack incidents reproduced using [Foundry](https://getfoundry.sh/), a blazing-fast Ethereum development toolkit. This repository serves as an educational resource to understand common vulnerabilities exploited in the DeFi ecosystem and provides proof-of-concept (PoC) implementations to aid in learning and prevention strategies.

This repository filters out reentrancy attacks from the repository [DeFiHacksReproduce](https://github.com/SunWeb3Sec/DeFiHackLabs.git) to focus on reentrancy attacks only. The incidents are categorized by year, with each year containing a dedicated folder for all related attack incidents. Each attack incident is represented by a Solidity (`.sol`) file containing the exploit's proof of concept.

## Table of Contents

- [About This Repository](#about-this-repository)
- [File Structure](#file-structure)
- [Contents Overview](#contents-overview)
  - [Reentrancy Attacks in 2024](#1-reentrancy-attacks-in-2024)
  - [Reentrancy Attacks in 2023](#2-reentrancy-attacks-in-2023)
  - [Reentrancy Attacks Before 2021 (2020 and Older)](#3-reentrancy-attacks-before-2021-2020-and-older)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running Tests](#running-tests)
- [Additional Resources](#additional-resources)
- [Contribution](#contribution)
- [Disclaimer](#disclaimer)
- [License](#license)

---

## About This Repository

This repository aims to:

- **Educate:** Provide detailed examples of reentrancy attacks to help developers understand how vulnerabilities are exploited.
- **Reproduce:** Offer reproducible PoCs using Foundry to simulate real-world attack scenarios.
- **Prevent:** Aid in developing strategies and best practices to prevent similar attacks in the future.

By studying these incidents, developers can gain insights into the common pitfalls in smart contract development and enhance the security of their own projects.

---

## File Structure

The repository is organized by year, with each year containing a dedicated folder for all related attack incidents. Each attack incident is represented by a Solidity (`.sol`) file containing the exploit's proof of concept.

```
root/
├── src/      
│   ├── 2020-Older/
│   │   └── test/
│   │       ├── LendfMe_exp.sol
│   │       └── UniSwapV1_exp.sol
|   |       └── SpankChain_exp.sol
│   │       └── Parity_exp.sol
│   ├── 2021/
│   │   └── test/
│   │       ├── SpankChain_exp.sol
│   │       ├── LendfMe_exp.sol
│   │       ├── UniSwapV1_exp.sol
│   │       └── Parity_exp.sol
│   ├── 2022/
│   │   └── test/
│   │       ├── JAY_exp.sol
│   │       ├── Defrost_exp.sol
│   │       ├── DFX_exp.sol
│   │       ├── N00d_exp.sol
│   │       ├── Market_exp.sol
│   │       ├── THB_exp.sol
│   │       ├── Omni_exp.sol
│   │       ├── Rari_exp.sol
│   │       ├── Revest_exp.sol
│   │       ├── Agave_exp.sol
│   │       ├── HundredFinance_exp.sol
│   │       ├── Paraluni_exp.sol
│   │       └── Bacon_exp.sol
│   ├── 2023/
│   │   └── test/
│   │       ├── NFTTrader_exp.sol
│   │       ├── GoodDollar_exp.sol
│   │       ├── CAROLProtocol_exp.sol
│   │       ├── StarsArena_exp.sol
│   │       ├── XSDWETHpool_exp.sol
│   │       ├── uniclyNFT_exp.sol
│   │       ├── Paribus_exp.sol
│   │       ├── Sentiment_exp.sol
│   │       ├── Euler_exp.sol
│   │       ├── Conic_exp.sol
│   │       ├── Conic_exp2.sol
│   │       ├── Libertify_exp.sol
│   │       ├── ArcadiaFi_exp.sol
│   │       ├── Sturdy_exp.sol
│   │       ├── dForce_exp.sol
│   │       ├── Midas_exp.sol
│   │       └── Orion_exp.sol
│   └── 2024/
│       └── test/
│           ├── Penpiexyzio_exp.sol
│           ├── Minterest_exp.sol
│           ├── MRP_exp.sol
│           ├── PredyFinance_exp.sol
│           ├── SMOOFSStaking_exp.sol
│           ├── NBLGAME_exp.sol
│           ├── BarleyFinance_exp.sol
│           └── ...
├── README.md
└── ... (other files and folders)
```

---

## Contents Overview

### 1. Reentrancy Attacks in 2024

**[Reentrancy Attacks 2024 README](./README_2024.md)**

This section includes detailed accounts of reentrancy-related DeFi incidents that occurred in 2024. Each incident provides information on the loss incurred, testing commands using Foundry, contract references, and relevant links for further information.

**Key Incidents:**

- **20240903 - Penpiexyz_io - Reentrancy and Reward Manipulation**
- **20240714 - Minterest - Reentrancy**
- **20240702 - MRP - Reentrancy**
- **20240529 - PredyFinance - Reentrancy**
- **...and more**

### 2. Reentrancy Attacks in 2023

**[Reentrancy Attacks 2023 README](./README_2023.md)**

This section documents reentrancy-related DeFi incidents from 2023. Similar to the 2024 section, each entry includes the date, project name, loss amount, testing commands, contract links, and relevant references.

**Key Incidents:**

- **20231216 - NFTTrader - Reentrancy**
- **20231216 - GoodDollar - Lack of Input Validation & Reentrancy**
- **20231213 - CAROLProtocol - Price Manipulation Via Reentrancy**
- **...and more**

### 3. Reentrancy Attacks Before 2021 (2020 and Older)

**[Reentrancy Attacks Before 2021 README](./README_Before2021.md)**

This section covers reentrancy-related DeFi incidents that occurred before 2021, including the years 2017, 2018, and 2020. Each incident provides comprehensive details similar to the other sections.

**Key Incidents:**

- **20181007 - SpankChain - Reentrancy**
- **20200419 - LendfMe - ERC777 Reentrancy**
- **20200418 - UniSwapV1 - ERC777 Reentrancy**
- **20171106 - Parity - 'Accidentally Killed It'**

---

## Getting Started

### Prerequisites

Ensure you have the following installed on your system:

- **[Foundry](https://getfoundry.sh/)**: Ethereum development toolkit.
- **[Git](https://git-scm.com/)**: Version control system.
- **[Node.js](https://nodejs.org/)** (optional): For running scripts or additional tools.

### Installation

1. **Clone the Repository:**

   ```sh
   git clone https://github.com/SunWeb3Sec/DeFiHacksReproduce.git
   cd DeFiHacksReproduce
   ```

2. **Install Foundry:**

   Follow the [Foundry installation guide](https://book.getfoundry.sh/getting-started/installation) to set up Foundry on your machine.

### Running Tests

Each attack incident includes a Solidity file (`.sol`) with a proof of concept. To run the tests using Foundry:

1. **Navigate to the Attack Directory:**

   ```sh
   cd src/[year]/test/
   ```

2. **Run the Test:**

   ```sh
   forge test --contracts ./AttackName_exp.sol -vvv
   ```

   Replace `AttackName_exp.sol` with the specific contract file you wish to test.

**Example:**

To test the **Penpiexyz_io** attack from 2024:

```sh
forge test --contracts ./src/2024/test/Penpiexyzio_exp.sol -vvv --evm-version shanghai
```

---

## Additional Resources

### Transaction Debugging Tools

- [Phalcon](https://explorer.phalcon.xyz/)
- [Tx Tracer](https://openchain.xyz/trace)
- [Cruise](https://cruise.supremacy.team/)
- [EthTx](https://ethtx.info/)
- [Tenderly](https://dashboard.tenderly.co/explorer)
- [EigenPhi](https://tx.eigenphi.io/analyseTransaction)

### Ethereum Signature Database

- [4byte](https://www.4byte.directory/)
- [Sig DB](https://openchain.xyz/signatures)
- [EtherFace](https://www.etherface.io/hash)

### Useful Tools

- [ABI to Interface](https://gnidan.github.io/abi-to-sol/)
- [Get ABI for Unverified Contracts](https://abi.w1nt3r.xyz/)
- [ETH Calldata Decoder](https://apoorvlathey.com/eth-calldata-decoder/)
- [ETHCMD - Guess ABI](https://www.ethcmd.com/tools/decode-calldata/)
- [Abi Tools](https://openchain.xyz/tools/abi)

### Hacks Dashboard

- [Slowmist](https://hacked.slowmist.io/)
- [Defillama](https://defillama.com/hacks)
- [De.Fi](https://de.fi/rekt-database)
- [Rekt](https://rekt.news/)
- [Cryptosec](https://cryptosec.info/defi-hacks/)

---

## Contribution

Contributions are welcome! If you have any improvements, additional incidents, or fixes, please follow these steps:

1. **Fork the Repository.**
2. **Create a Feature Branch:**

   ```sh
   git checkout -b feature/YourFeatureName
   ```

3. **Commit Your Changes:**

   ```sh
   git commit -m "Add your message here"
   ```

4. **Push to the Branch:**

   ```sh
   git push origin feature/YourFeatureName
   ```

5. **Open a Pull Request.**

Please ensure your contributions adhere to the repository's guidelines and maintain the existing structure and formatting.

---

## Disclaimer

**Disclaimer:**  
This content serves solely as a proof of concept showcasing past DeFi hacking incidents. It is strictly intended for educational purposes and should not be interpreted as encouraging or endorsing any form of illegal activities or actual hacking attempts. The provided information is for informational and learning purposes only, and any actions taken based on this content are solely the responsibility of the individual. The usage of this information should adhere to applicable laws, regulations, and ethical standards.

---

## License

This project is licensed under the [MIT License](./LICENSE).

