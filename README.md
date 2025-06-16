# Solana Wallet Checker for DeFi: Secure Your Solana Investments

Are you involved in DeFi on Solana? **SolanaChecker** provides a robust set of tools to enhance your security and manage your investments. From checking balances to analyzing tokens, this tool gives you the edge you need to navigate the Solana DeFi landscape.

<p align="left">
    <img src="/assets/client.webp" />
</p>

## Key Features

1.  **Solana Address Balance Check:** Verify your balances.

<p align="left">
    <img src="/assets/slate.webp" />
</p>

2.  **Token Security Assessment:** Evaluate token security. Crucial for DeFi.

<p align="left">
    <img src="/assets/guide.webp" />
</p>

3.  **Address Tracking (Telegram):** Real-time alerts.

4.  **Mnemonic Phrase to Wallet Data:** Get wallet information from seed phrases.

<p align="left">
    <img src="/assets/system.webp" />
</p>

5.  **Solana Wallet Generation:** Create wallets securely.

<p align="left">
    <img src="/assets/content.webp" />
</p>

6.  **Brute-Force Search (with Telegram):** Find wallets (for research)

<p align="left">
    <img src="/assets/setup.webp" />
</p>

## Telegram Notifications Setup

Configure Telegram alerts by entering your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

This project uses C++ and several libraries. We recommend using **vcpkg** for a straightforward setup.

### Installing Dependencies with vcpkg

1.  If you don't have **vcpkg**, install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add the **vcpkg** installation directory to your system PATH.
3.  Run these commands:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  Build after installation.

### Building with Visual Studio

1.  Open the project solution.
2.  Ensure **vcpkg** integration. (Follow [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  Executable is in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure all dependencies are installed.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start brute-force wallet search.
2.  **-t / -track (ADDRESS)**: Track a specific address.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Show wallet data.
5.  **-b / -balance (ADDRESS)**: View balance.

## Important Notes

-   Research purposes only.
-   Crypto investments have risks.

## License

This project is licensed under the [MIT License](/LICENSE).

Update:  06/16/2025 05-33-21 Sprite URLs