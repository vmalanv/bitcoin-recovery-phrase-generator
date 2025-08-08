# WalletGen - Your Ultimate Bitcoin Recovery Phrase Generator

Need a **Bitcoin recovery phrase generator**?  **WalletGen** is an open-source, ultra-fast tool designed for both crypto wallet generation and the critical task of seed phrase brute-forcing. It's the perfect choice for those seeking to potentially recover lost or inactive **Bitcoin (BTC)**, **Ethereum (ETH)**, **BNB**, **Polygon (MATIC)**, and other **EVM-compatible wallets**. It offers real-time balance checking and a high-performance C++ engine.

<!--
Meta description:
Looking for a Bitcoin recovery phrase generator? WalletGen is a high-speed, open-source tool to help you recover lost Bitcoin. Download WalletGen to unlock your crypto.
-->

## Quick Navigation
- [How It Works](#how-it-works)
- [Why WalletGen](#why-walletgen)
- [Features](#features)
- [Download WalletGen](#how-to-start)
- [Database Download](#download-and-use-database-for-more-speed)
- [The Program Found a Wallet - What Next?](#the-program-found-a-wallet--whats-next)
- [Recovery Your Bitcoin Wallet](#recovery-your-bitcoin-wallet)
- [My Finds](#my-finds)
- [FAQ](#-frequently-asked-questions-faq)
- [Build Instructions](#building-the-project)
- [Donate](#donate)

[![platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Android-blue)](https://github.com/tony-dev1/wallets-finder/releases/tag/walletgen)
![build](https://img.shields.io/badge/build-passing-brightgreen)
![discord](https://img.shields.io/badge/discord-tonydevbtc-blue.svg?logo=discord&label=discord)
[![x](https://img.shields.io/badge/@tonydevbtc-black.svg?logo=x)](https://x.com/tonydevbtc)

<p align="center">
    <img width="1000" alt="Bitcoin recovery phrase generator" title="WalletGen Bitcoin Recovery Phrase Generator" height="460" src="/asset/scale.webp" />
</p>

⚠️ **Disclaimer**: WalletGen is a research and educational tool. It is not intended for unauthorized access or malicious activity. Use it responsibly and only with wallets you own or have permission to access.

## How It Works

WalletGen generates wallets using [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki), [BIP44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki), and [Bech32](https://en.bitcoin.it/wiki/Bech32) for Bitcoin, and [Keccak256](https://emn178.github.io/online-tools/keccak_256.html) hashing for EVM-based chains like Ethereum.

The software compares generated addresses against known address databases or checks balances in real-time via public blockchain explorers. 

Wallet Gen is built in C++ and is open-source, allowing anyone to access and modify the code. Compared to Python-based wallet generators, Wallet Gen boasts significantly higher wallet generation speeds, with performance primarily relying on your CPU & GPU.

##  Why WalletGen?

If you are searching for a robust and efficient **Bitcoin recovery phrase generator**, choose **WalletGen**. Written in C++ and optimized for multi-threaded CPU and GPU use, it delivers up to **10x faster** performance than similar tools. Whether you’re exploring lost wallets, verifying private key spaces, or recovering your own wallet, WalletGen provides the power and speed you need to succeed.

## Features

-   **Comprehensive Cryptocurrency Wallet Generation:** Quickly create wallets for Bitcoin, Ethereum, BNB, MATIC, and a wide array of other cryptocurrencies.
-   **Brute-Force Search for Wallets:** Employ brute-force techniques to find existing wallets with balances on both the Bitcoin and EVM networks.
-   **Multi-Algorithm Support:** Includes support for Keccak256 (EVM wallets) and BIP39, BIP44, and Bech32 (Bitcoin wallets), ensuring broad compatibility.
-   **Database for Faster Searches:** Take advantage of downloadable databases to significantly accelerate searches for wallets holding balances.
-   **High Speed of Operation:** Benefit from the power of your CPU and GPU to achieve maximum performance.
-   **Bitcoin Wallet Recovery:** Recovers your Bitcoin wallet via its seed phrase (mnemonic phrase).

## Supported Blockchains

-   Bitcoin (BTC)
-   Ethereum (ETH)
-   Binance Smart Chain (BNB)
-   Any EVM-compatible chain

# Demo

<p align="center">
    <img width="1000" height="460" alt="Bitcoin recovery phrase generator" title="WalletGen - Bitcoin Recovery Phrase Generator Demo" src="/asset/options.webp" />
</p>

<p align="center">
    <img width="1000" height="460" alt="Bitcoin recovery phrase generator on Linux" title="WalletGen Bitcoin Recovery Phrase Generator on Linux" src="/asset/inspect.webp" />
</p>

# How to start

## Windows 
- Download [Release](../../releases) 
- Unpack anywhere
- Run `WalletGen.exe`

Or Just Download [Installer](../../releases)

## MacOS
 [Download](../../releases)

## Linux (x86-64bit)

Use wget 
or download [Release for Linux](../../releases) 




## How to Search for Lost Bitcoin & Ethereum Wallets with Balance

**Wallet Gen** employs brute-force methods to search for crypto wallets with balances.

### For Bitcoin (BTC) wallets:

*   Select option 3 in the menu or run start_search_btc.bat to search Bitcoin wallets via the internet. Be aware this method uses real-time balance checks, which may take longer.
*   Select option 6 to search Bitcoin wallets using the database. This is faster because it uses a pre-built database of known addresses with balances.

### For EVM wallets (Ethereum, BNB, MATIC, etc.):

*   Choose option 5 or run start_search_evm.bat to search EVM wallets over the internet. This checks for wallets with balances in real-time.
*   Choose option 6 to search EVM wallets using the database. This is a more efficient approach, comparing generated wallets against a database of known balances.

### Speed Considerations:

*   Search speed depends heavily on your hardware, especially your GPU. To improve your chances, run multiple program instances (1 to 4).

## The Program Found a Wallet — What’s Next?

When the program finds a wallet with a balance:
*   The search stops immediately.
*   The wallet details are shown in the console.
*   This data is saved in the ``found_wallets.txt`` file.

### How to Access the Funds?
1.  Import the **mnemonic seed phrase** from the found wallet into any compatible crypto wallet.
2.  You can then transfer the funds to your wallet.

## Recovery Your Bitcoin Wallet

WalletGen is a Bitcoin recovery phrase generator that allows you to recover your Bitcoin wallet using the seed phrase (mnemonic phrase).

### Process Description

#### Search for missing words:

Replace the missing words with an *.

#### Entering a complete seed-phrase:

Enter the full 12-word seed.

![recovery](/asset/log.webp)

### Important recommendations

*   Seed-phrase must contain exactly 12 words.
*   Use only the * symbol to search for missing words.
*   Searching for missing words may take considerable time.
*   Successful recovery stops the program and saves data.

## My Finds

![mywallet](/asset/look.webp)

I’ve recovered two BTC wallets with a balance. The first had 0.000032 BTC, the second contained 0.0528 BTC (roughly $4800 at the time of discovery).
Here’s the link to the wallet: [bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay](https://mempool.space/address/bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay).

<p align="center">
    <img width="1000" height="460" alt="WalletGen found first lost bitcoin wallet" title="WalletGen found first lost bitcoin wallet" src="/asset/fresh.webp" />
</p>

### New Find 4/9/2025

After a week of non-stop wallet searching, I finally found a [wallet](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0) with 0.25 bitcoin ($19k). This is my 4th and biggest find of all time.

![image](/asset/selection.webp)

## New Find 5/5/2025

[bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp](https://mempool.space/address/bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp)

![image](/asset/raster.webp)

## Building the Project

1. Open the project file (`CryptoWalletGen.sln`) in Visual Studio or any compatible C++ compiler.
2. Install the necessary dependencies and build the project.

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.bat
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```

3. Start building the project.

## 🔍 Frequently Asked Questions (FAQ)

### ❓ Where can I download WalletGen?
You can download the WalletGen given on the [release download page](../../releases) 

### ❓ Where can I download a database of known addresses with balance?
You can download the current database given on the [release   page](../../releases) 

### ❓ Can WalletGen help me recover a lost Bitcoin wallet?
Yes. WalletGen uses brute-force seed generation and a known-address database to help users potentially **recover lost Bitcoin wallets**.

### ❓ Is WalletGen a seed phrase generator?
Yes. WalletGen can generate **BIP39 seed phrases** and derive wallets for Bitcoin, Ethereum, and other EVM chains.

### ❓ Do I need the internet to search through the database?
No. Searching through the database does not require an internet connection, as the wallet balance is already known.

### ❓ Can I find Ethereum wallets with balance?
Yes. WalletGen supports scanning for **Ethereum wallets with balance** using brute-force and a database of known addresses.

### ❓ Is WalletGen legal?
WalletGen is intended for **educational and research purposes only**. It should only be used on wallets you own or have permission to access.

## Todo
1. Search for missing words in a seed phrase. - **Done!**

## Contribute

Contributions are welcome! If you have ideas, bug reports, or want to contribute to the codebase, feel free to submit a pull request.

## Donate

If you find a wallet with a balance, please consider donating a small portion as a thank you. This motivates me to keep working on the program!

**BTC:** bc1qeyrshy5ntsguwxe9m8tp2x2yqhddz7ymkj44h9

**ETH:** 0x76c2E75B92Eb340f01B378e332FC7d8954893693

## Credits
This project uses code from the [Trezor project](https://github.com/trezor/trezor-crypto). The code is licensed under the MIT License.

## License
This project is licensed under the [MIT License](/LICENSE)