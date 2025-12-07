# SafeSend

🌟 Status: Live

[SafeSend](https://safesend.to) is a secure token transfer platform that protects your DeFi transactions from costly mistakes through test transactions, approval-based security, and Telegram confirmations.

## Overview

SafeSend helps anyone transfer tokens safely from their wallet address to a receiver's wallet address. The platform addresses common DeFi risks—wrong addresses, gas failures, and malicious approvals—by implementing a verification-first transfer flow.

With SafeSend, you can:

- [Send tokens securely](#send-tokens-with-safesend) with test transaction verification
- [Receive transfer requests](#receive-and-approve-transfers-via-telegram) via Telegram for confirmation
- [Manage an Address Book](#manage-your-address-book) for frequent recipients
- [Add Custom Tokens](#add-custom-tokens) beyond default supported assets
- [Track transaction history](#view-transaction-history)
- [Connect Telegram](#connect-telegram-for-notifications) for transfer confirmations
- [Earn rewards](#leaderboard-and-rewards) through the SafeSend Leaderboard

> **tip** · Connect your Telegram account before making your first transfer to enable recipient confirmations and earn leaderboard rewards.

## Explain it like I'm five

Imagine you want to send your friend some tokens, but you're worried about typing their address wrong and losing your tokens forever. SafeSend is like a helpful assistant that:

1. **First sends a tiny test amount** (like sending $0.01 before sending $100) to make sure the address is correct
2. **Asks your friend on Telegram** "Hey, someone is trying to send you tokens—is this right?" before completing the transfer
3. **Only sends the full amount** after everything checks out

It's like double-checking the address on a package before the mailman takes it away—except for crypto!

## Why Use SafeSend?

| Without SafeSend | With SafeSend |
|------------------|---------------|
| One typo = funds lost forever | Test transaction catches errors first |
| No way to verify recipient | Telegram confirmation ensures correct recipient |
| Unlimited token approvals | Exact approval amounts only |
| No transaction records | Full history with explorer links |
| Just hoping for the best | Confidence with every transfer |

## The Problem SafeSend Solves

One tiny mistake in DeFi can cost you your entire wallet. The risks are real and unforgiving:

| Risk | What Happens |
|------|--------------|
| **Wrong Contract Address** | Send to a smart contract with bad approval logic → funds stolen instantly |
| **Infinite Allowances** | Auto-approval with unlimited allowance → exploited later through backdoors |
| **User Errors** | Typos, gas failures, or network issues → tokens lost forever |

SafeSend eliminates these risks through a multi-step verification process that includes test transactions and recipient confirmation via Telegram.

## How SafeSend Protects Your Transfers

| Protection | Description |
|------------|-------------|
| **Verify Before You Send** | Run a test transaction before moving large funds—no more costly mistakes |
| **Approval-Based Security** | Every transfer goes through a 2-step approval process—no surprises, no lost funds |
| **Telegram Confirmation** | Recipients confirm transfers via Telegram before execution, preventing sends to wrong addresses |
| **Built for Speed & Simplicity** | Integrated via Telegram bot and intuitive UI—no extra wallets or complex setups |

## Target Users

SafeSend is designed for:

- **DeFi users** who regularly transfer tokens and want protection against costly mistakes
- **Crypto newcomers** who need guardrails when sending their first transactions
- **High-volume traders** who want to verify addresses before large transfers
- **Teams and DAOs** managing treasury transfers with additional confirmation steps
- **Anyone** who has experienced or fears losing funds to a wrong address

## Prerequisites

- EVM-compatible wallet (MetaMask, WalletConnect, Trust Wallet, or other Web3-compatible wallets)
- Tokens on a [supported blockchain network](#supported-networks)
- Gas funds (ETH, BNB, etc.) on the network you're transferring from
- (Recommended) Telegram account for transfer confirmations

## Supported Networks

SafeSend supports the following blockchain networks:

| Network | Status |
|---------|--------|
| Ethereum | ✅ Live |
| Arbitrum | ✅ Live |
| BSC (Binance Smart Chain) | ✅ Live |
| Base | ✅ Live |

> **tip** · Base and Arbitrum typically have lower gas fees than Ethereum mainnet—consider using these networks for smaller transfers.

## Limitations

- Transfers are limited to ERC-20 tokens on supported networks
- Custom tokens must be manually added via contract address
- Telegram confirmation requires both sender and recipient to link their accounts
- Transactions expire after approximately 23 hours if not confirmed

---

## Get Started with SafeSend

Connect to SafeSend to start making secure transfers. You can connect using your Web3 wallet.

### Prerequisites

- EVM-compatible wallet (MetaMask, Trust Wallet, WalletConnect, etc.)
- The wallet must be unlocked and accessible

### Step 1: Navigate to SafeSend

- Go to [safesend.to](https://safesend.to) and click **Start Secure Transfer**.

<details>
<summary>Show me</summary>

The SafeSend landing page displays key platform statistics including total transactions and total volume processed. Click the green "Start Secure Transfer" button to begin.

![SafeSend landing page with Start Secure Transfer button](/img/safesend/landing-page.png)

</details>

### Step 2: Connect Your Wallet

- Click **Start Secure Transfer** to open the wallet verification modal.

<details>
<summary>Show me</summary>

A modal appears prompting you to verify your wallet. Your connected wallet address is displayed (e.g., `0xCD56...8b75`).

![Verify Your Wallet modal](/img/safesend/verify-wallet-modal.png)

</details>

### Step 3: Verify Wallet Ownership

- Click **Verify Wallet** and approve the signature request in your wallet.

<details>
<summary>Show me sign-in methods</summary>

Use the tabs to learn more about different wallet options:

**Trust Wallet**

1. Your Trust Wallet will prompt you to unlock with biometrics or password.
2. A signature request appears from `https://safesend.to` with the message: "Please verify your wallet to confirm ownership. You are responsible for submitting the correct address."
3. Click **Confirm** to complete verification.

![Trust Wallet signature request](/img/safesend/trust-wallet-signature.png)

**MetaMask**

1. MetaMask will popup requesting a signature.
2. Review the message and click **Sign** to verify ownership.
3. No gas fees are required for signature verification.

**WalletConnect**

1. Scan the QR code with your mobile wallet.
2. Approve the connection request in your wallet app.
3. Sign the verification message when prompted.

</details>

Congratulations: your wallet is now connected to SafeSend.

---

## Send Tokens with SafeSend

Use the walkthrough to understand how to send tokens securely with SafeSend's test transaction verification.

> **tip** · For the smoothest experience, [connect your Telegram](#connect-telegram-for-notifications) before initiating transfers. This enables recipient confirmations and keeps you updated on transaction status.

### Prerequisites

- [Connected wallet](#get-started-with-safesend)
- Tokens to send on a supported network
- Gas funds on the same network (ETH for Ethereum/Base/Arbitrum, BNB for BSC)

> ⚠️ **Gotcha** · Make sure you have enough gas funds *before* starting a transfer. Running out of gas mid-transaction can leave your transfer in a pending state.

### Step 1: Select Chain and Token

- From the **Send** tab, select your blockchain network and the token you want to transfer.

<details>
<summary>Show me</summary>

The Send interface shows dropdown selectors for chain and token. Select your chain first (Ethereum, Base, Arbitrum, or BSC), then choose your token from the available options.

![SafeSend main interface with chain and token selection](/img/safesend/send-interface.png)

</details>

If your wallet is on a different network, SafeSend will prompt you to switch.

<details>
<summary>Show me network switch</summary>

A prompt appears in your wallet: "Switch network to connect this site?" with a warning that switching networks will cancel all pending confirmations. Click **Switch** to proceed.

![Network switch prompt](/img/safesend/network-switch.png)

</details>

> ⚠️ **Gotcha** · Switching networks will cancel all pending wallet confirmations. Complete any pending transactions before switching.

### Step 2: Enter Transfer Details

- Enter the transfer amounts and recipient address.

| Field | Description |
|-------|-------------|
| **Amount** | The main transfer amount you want to send |
| **Test Amount** | Small verification amount (default: 0.001) sent first to verify the address |
| **Recipient Address** | The destination wallet address, or select from your Address Book |

<details>
<summary>Show me</summary>

Enter your amounts in the respective fields. The recipient address field also allows you to select from saved addresses in your Address Book.

![Transfer details entry](/img/safesend/transfer-details.png)

</details>

### Step 3: Initiate Transfer

- Click **Send Token** to begin the secure transfer process.

SafeSend creates a transaction record with a unique URL (e.g., `safesend.to/transaction/5212`) that tracks the transfer through all verification stages.

<details>
<summary>Show me transaction details</summary>

The Transaction Details page displays:
- **Sending on**: Network and amount (e.g., "Base • 1.00 USDC")
- **Expires in**: Time remaining (approximately 23 hours)
- **From/To**: Sender and recipient addresses
- **Test Amount**: The verification amount
- **Test Tx Hash**: Link to the test transaction on block explorer
- **Status**: Current state of the transfer

![Transaction details page](/img/safesend/transaction-details.png)

</details>

### Step 4: Approve Token Spending

- Your wallet will request permission to access your tokens. Set your spending limit and confirm.

<details>
<summary>Show me approval options</summary>

Trust Wallet (and similar wallets) displays an approval screen:
- **Amount**: Shows 0 (initial approval)
- **Spending Limit**: Choose from 25%, 50%, 100%, or Default
- **Estimated Time**: Approximately 15 seconds
- **Network fee**: Small gas fee (e.g., <$0.01)

For SafeSend, you can set a specific limit matching your transfer amount for maximum security.

![Wallet approval with spending limit options](/img/safesend/spending-limit-approval.png)

</details>

- Click **Confirm** to approve. You'll see a toast notification: "Approval transaction sent successfully!"

Ensure you have sufficient gas funds. If you see "Insufficient Base (ETH) - Base balance for gas fee", you'll need to add ETH to your wallet.

### Step 5: Execute Test Transaction

- Once approval is confirmed, click **Start Test TX** to send the verification amount.

<details>
<summary>Show me</summary>

The transaction status updates to show "Pending" for the Test Tx Hash. Click **Start Test TX** to initiate the small test transfer.

![Start Test TX button](/img/safesend/start-test-tx.png)

</details>

- A toast notification confirms: "Test transaction started successfully!"
- Wait for the test transaction to be confirmed on-chain.

### Step 6: Approve Main Transfer

- After the test transaction succeeds, the **Approve** button becomes available.

<details>
<summary>Show me</summary>

The status shows the test transaction as confirmed. The **Approve** button appears, allowing you to authorize the main transfer amount.

![Approve button after test TX](/img/safesend/approve-main-transfer.png)

</details>

- Click **Approve** to authorize the full transfer.
- Confirm the transaction in your wallet.

### Step 7: Transaction Complete

- Once confirmed, the status updates to show **Confirmed TX** with a link to the block explorer.

<details>
<summary>Show me</summary>

The Transaction Details page shows:
- **Status**: "Confirmed TX: 0x10fd...a74d" (clickable link to explorer)
- All transaction details are recorded for your records

![Confirmed transaction](/img/safesend/transaction-confirmed.png)

</details>

Congratulations: your tokens have been securely transferred!

---

## Receive and Approve Transfers via Telegram

SafeSend uses Telegram as a confirmation layer. When someone sends you tokens via SafeSend, you'll receive a notification to confirm the transfer before it executes.

### How Telegram Confirmation Works

1. **Sender initiates transfer** via SafeSend web app
2. **Recipient receives Telegram notification** with transfer details
3. **Recipient confirms or rejects** the transfer via Telegram bot
4. **Transfer executes** only after recipient confirmation

This flow prevents accidental transfers to wrong addresses by requiring the recipient to actively confirm they expect the funds.

### Prerequisites

- [Telegram account linked to SafeSend](#connect-telegram-for-notifications)
- SafeSend Telegram bot added to your contacts

### Confirming an Incoming Transfer

When you receive a transfer request:

- Open the notification from the SafeSend bot in Telegram.
- Review the transfer details (amount, token, sender address).
- Tap **Confirm** to approve or **Reject** to decline.

<details>
<summary>Show me</summary>

The Telegram bot message displays:
- Token and amount being sent
- Sender's wallet address
- Network/chain
- Confirmation and rejection buttons

![Telegram transfer confirmation](/img/safesend/telegram-confirmation.png)

</details>

Once confirmed, the sender can complete the transfer from their Transaction Details page.

---

## Connect Telegram for Notifications

Link your Telegram account to receive transfer confirmations and updates about your SafeSend activity.

### Prerequisites

- Telegram account
- [Connected wallet](#get-started-with-safesend) on SafeSend

### Step 1: Navigate to Profile

- From the SafeSend app, click the **Profile** tab in the navigation.

<details>
<summary>Show me</summary>

The Profile page displays the "Connect Your Telegram" section with instructions and an OTP code field.

![Profile page with Connect Telegram section](/img/safesend/profile-connect-telegram.png)

</details>

### Step 2: Copy Your OTP Code

- A 6-digit OTP code is automatically generated (e.g., `865964`).
- Click **Copy** to copy the code to your clipboard.

<details>
<summary>Show me</summary>

The Profile page shows:
- **OTP field**: Your 6-digit verification code
- **Copy button**: Click to copy the code
- **Check Status button**: Verify connection after completing the process
- **Open Bot link**: Direct link to the SafeSend Telegram bot

**How to connect:**
1. Click "Connect Telegram" button below
2. Copy the OTP code that appears
3. Open our Telegram bot and paste the OTP code

![OTP code generation](/img/safesend/otp-code.png)

</details>

### Step 3: Open the SafeSend Bot

- Click **Open Bot** to open the SafeSend Telegram bot (`@safesendbynodeopsbot`).

<details>
<summary>Show me</summary>

A dialog appears asking to open Telegram. Click **Open Telegram** or **START BOT** to proceed.

The bot page shows:
- **@safesendbynodeopsbot**
- "SafeSend by NodeOps"
- **START BOT** button to begin interaction

![SafeSend Telegram bot landing page](/img/safesend/telegram-bot-landing.png)

</details>

### Step 4: Verify in Telegram

- The bot sends a welcome message with verification instructions.
- Paste your 6-digit OTP code in the chat.

<details>
<summary>Show me</summary>

The SafeSend bot displays:

"🎉 Welcome to the verification process!

To link your Telegram account, please:
1. Go to https://safesend.to
2. Generate an OTP for Telegram verification
3. Come back here and send me the OTP code

Please enter your 6-digit OTP code:"

After entering your OTP, the bot confirms:

"✅ Successfully verified! Your account has been linked.
User ID: [your-id]
Telegram ID: [your-telegram-id]"

![Telegram bot verification success](/img/safesend/telegram-verified.png)

</details>

### Step 5: Confirm Connection

- Return to SafeSend and click **Check Status** to verify the connection.
- The Profile page now shows **"Telegram Connected"** with a green checkmark.

<details>
<summary>Show me</summary>

Once connected, the Profile page displays:
- ✅ **Telegram Connected**
- "Your Telegram account is successfully connected"
- **Open Bot** button to access the bot anytime

![Profile showing Telegram connected](/img/safesend/telegram-connected.png)

</details>

Congratulations: your Telegram is now connected for transfer confirmations and notifications.

---

## Manage Your Address Book

Save frequently used addresses for quick access during transfers.

### View Your Address Book

- Click the **Address Book** tab in the navigation.

<details>
<summary>Show me</summary>

The Address Book page displays:
- "Manage your addresses all in one place"
- Your saved addresses list
- If no addresses are saved: "No addresses saved - Add your first address to get started with the address book"

![Address Book - empty state](/img/safesend/address-book-empty.png)

</details>

### Add a New Address

- Click the green **+ Add New Address** button.
- Enter the wallet address (0x...).
- Add an optional label for easy identification (e.g., "My Ledger", "Team Treasury").
- Click **Save** to add the address to your book.

### Use a Saved Address

When sending tokens, click the **Recipient Address** field and select from your saved addresses instead of manually entering the address each time.

---

## Add Custom Tokens

SafeSend supports adding custom ERC-20 tokens beyond the default list.

### Step 1: Open Token Management

- From the **Send** tab, click **+ Add Custom Token** or **Manage Tokens**.

<details>
<summary>Show me</summary>

Below the Send Token button, you'll see options for "+ Add Custom Token" and "Manage Tokens".

The Token Management modal shows your custom tokens list. If you haven't added any yet, it displays:
- "No Custom Tokens"
- "Add your first custom token to get started"

![Token Management modal - empty state](/img/safesend/token-management-empty.png)

</details>

### Step 2: Add Custom Token

- Click **+ Add Custom Token** to open the add token form.
- Select the **Chain** from the dropdown (Ethereum, Base, Arbitrum, or BSC).
- Enter the **Token Contract Address** (0x...).
- The following fields auto-populate from the contract:
  - **Symbol** (e.g., "USDC")
  - **Decimals** (e.g., "18")
  - **Token Name** (e.g., "USD Coin")
- Click **Add Token** to save.

<details>
<summary>Show me</summary>

The Add Custom Token form shows:
- Chain selector dropdown
- Token Contract Address input field
- Auto-populated Symbol, Decimals, and Token Name fields
- Green "Add Token" button

![Add Custom Token form](/img/safesend/add-custom-token-form.png)

</details>

Your custom token will now appear in the token selector dropdown when sending on that chain.

---

## View Transaction History

Track all your SafeSend transactions from the **History** tab.

<details>
<summary>Show me</summary>

The Transaction History page displays your completed transfers with full details including test and confirmed transaction hashes.

![Transaction history showing completed transfer](/img/safesend/transaction-history.png)

</details>

Each transaction entry includes:

| Field | Description |
|-------|-------------|
| **Sent on** | Network and amount (e.g., "Base • 1.00 USDC") |
| **To** | Recipient wallet address |
| **Date** | Timestamp of the transaction |
| **Test Amount** | The verification amount sent (e.g., 0.01 USDC) |
| **Test TX** | Link to test transaction on block explorer |
| **Status** | Pending, Completed, or Failed |
| **Confirmed TX** | Link to main transaction on block explorer |

You can also **Share on X** (Twitter) to share your successful transfer.

Click **Refresh** to update the transaction list with the latest status.

---

## Leaderboard and Rewards

SafeSend features a leaderboard that ranks users by total transfer volume, with $NODE token rewards for top participants.

### View the Leaderboard

- Click **Leaderboard** in the top navigation to see rankings.

<details>
<summary>Show me</summary>

The Leaderboard page displays:

**My Profile section:**
- Your wallet address
- Your current rank (e.g., #434)
- Your total volume (e.g., $1.0000)

**Badges section:**
- Available badge tiers with their rewards

**Rankings table:**
- Rank, Address, and Total Volume for top users
- Pagination showing total participants (e.g., "Showing 1 to 10 of 660 results")

![Leaderboard showing rankings and badges](/img/safesend/leaderboard-full.png)

</details>

### Badge Tiers and Rewards

| Badge | Requirement | Reward |
|-------|-------------|--------|
| 🏆 **Champion of Rome** | Top 10 | 12,500 $NODE |
| 🥇 **Centurion** | Top 50 | 15,000 $NODE |
| 🥈 **Legionnaire** | Top 200 | 15,000 $NODE |
| 🎖️ **Citizen of the Arena** | All verified participants | 7,500 $NODE |

> **tip** · Even with small transfer amounts, you can earn the "Citizen of the Arena" badge and 7,500 $NODE just by participating!

Use SafeSend regularly to climb the rankings and earn badge rewards!

---

## Disconnect Your Wallet

To disconnect your wallet from SafeSend:

- Click the wallet address button in the top right corner of the app (e.g., `0x8ddd...9b49`).
- Click **Disconnect** to end your session.

This resets the app to its initial state. You'll need to reconnect and verify your wallet to use SafeSend again.

---

## Security

SafeSend prioritizes the security of your funds and data:

| Security Feature | Description |
|------------------|-------------|
| **Non-custodial** | SafeSend never holds your private keys—they remain in your wallet at all times |
| **Exact Approvals** | Token approvals are requested for exact amounts, not unlimited allowances |
| **On-chain Verification** | All transactions are recorded on the blockchain with full transparency |
| **Signature-only Authentication** | Wallet verification uses message signing, not transactions—no gas required |
| **Open Transaction Records** | Every transfer includes explorer links for independent verification |

SafeSend smart contracts facilitate the transfer flow while you maintain full custody of your assets.

---

## FAQ

<details>
<summary>What is SafeSend and how does it work?</summary>

SafeSend is a secure token transfer platform that protects your DeFi transactions through test transactions, approval-based security, and Telegram confirmations. You connect your wallet, select a token and amount, and SafeSend guides you through a verification process—including a small test transaction—before executing the full transfer.

</details>

<details>
<summary>Which blockchain networks does SafeSend support?</summary>

SafeSend currently supports Ethereum, Arbitrum, BSC (Binance Smart Chain), and Base. More networks may be added in the future.

</details>

<details>
<summary>How does the test transaction verification work?</summary>

Before your main transfer, SafeSend sends a small test amount (default 0.001 or as configured) to verify the recipient address is correct and reachable. This catches errors before you commit larger funds. You can see the test transaction hash and status in your Transaction Details page.

</details>

<details>
<summary>Why do I need to connect Telegram?</summary>

Telegram integration adds an extra security layer. Recipients receive notifications to confirm incoming transfers before they execute, preventing accidental sends to wrong addresses. It also keeps you updated on your transaction status.

</details>

<details>
<summary>Do I need to pay gas fees?</summary>

Yes, you need to pay gas fees on the network you're transferring from. Gas costs vary by network congestion. Base and Arbitrum typically have lower fees than Ethereum mainnet.

</details>

<details>
<summary>What happens if I don't have enough gas?</summary>

If you have insufficient gas funds, your wallet will display an error (e.g., "Insufficient Base (ETH) - Base balance for gas fee"). You'll need to add native tokens (ETH, BNB) to your wallet before proceeding.

</details>

<details>
<summary>How long do I have to complete a transfer?</summary>

Transactions expire after approximately 23 hours if not completed. You can see the remaining time in the Transaction Details page under "Expires in".

</details>

<details>
<summary>Is my wallet safe?</summary>

Yes. SafeSend never has access to your private keys—they remain in your wallet. You approve each transaction individually, and SafeSend requests specific approval amounts rather than unlimited allowances. The signature verification only proves wallet ownership without transferring any funds.

</details>

<details>
<summary>How do I earn $NODE rewards?</summary>

Use SafeSend to transfer tokens and climb the leaderboard. Higher transfer volumes earn higher rankings and badge tiers, each with associated $NODE rewards. All verified participants earn the "Citizen of the Arena" badge with 7,500 $NODE.

</details>

<details>
<summary>Can I add custom tokens?</summary>

Yes! Click "+ Add Custom Token" from the Send page and enter the token's contract address. The token details will auto-populate, and it will appear in your token selector for future transfers.

</details>

<details>
<summary>What if the recipient doesn't have Telegram connected?</summary>

If the recipient hasn't connected their Telegram to SafeSend, they won't receive the confirmation notification. The transfer will still proceed through the standard flow, but without the extra recipient verification step. For maximum security, encourage recipients to connect their Telegram accounts.

</details>

<details>
<summary>Can I cancel a pending transfer?</summary>

Pending transfers that haven't been confirmed will automatically expire after approximately 23 hours. If you need to cancel sooner, do not approve the main transfer transaction in your wallet.

</details>

<details>
<summary>Why is my test transaction different from my main transfer amount?</summary>

The test transaction is intentionally small (default 0.001) to minimize risk while verifying the recipient address. Once the test succeeds, you can confidently approve the full transfer amount.

</details>

---

## Troubleshooting

<details>
<summary>Transaction stuck on "Pending"</summary>

If your transaction remains pending:
1. Check that you have sufficient gas funds on the selected network
2. Ensure your wallet is connected to the correct network
3. Try refreshing the Transaction Details page
4. Check the block explorer to see if the transaction is processing on-chain

</details>

<details>
<summary>"Insufficient gas" error</summary>

You need native tokens (ETH, BNB) to pay for transaction gas:
- **Ethereum/Base/Arbitrum**: Add ETH to your wallet
- **BSC**: Add BNB to your wallet

Gas fees vary by network congestion. Base and Arbitrum typically have the lowest fees.

</details>

<details>
<summary>Telegram not receiving notifications</summary>

If you're not receiving Telegram notifications:
1. Verify your Telegram is connected in the [Profile](#connect-telegram-for-notifications) tab
2. Check that you haven't muted the SafeSend bot
3. Try disconnecting and reconnecting your Telegram account

</details>

<details>
<summary>Custom token not appearing</summary>

When adding a custom token:
1. Ensure you've selected the correct chain
2. Verify the token contract address is correct for that network
3. Check that the token follows the ERC-20 standard

</details>

---

## Get Help

If you need assistance with SafeSend:

- **Telegram**: Reach out to the [NodeOps Telegram](https://t.me/nodeops) community
- **Discord**: Join the [NodeOps Discord](https://discord.gg/nodeops) for support
- **SafeSend Bot**: Use the [@safesendbynodeopsbot](https://t.me/safesendbynodeopsbot) for transaction updates

---

## What Next?

- [Start using SafeSend](https://safesend.to) to make your first secure transfer
- [Connect your Telegram](#connect-telegram-for-notifications) for transfer confirmations
- Save frequent recipients in your [Address Book](#manage-your-address-book)
- Climb the [Leaderboard](#leaderboard-and-rewards) to earn $NODE rewards
- Learn more about [$NODE tokenomics](/Tokenomics/node)
- Explore other [NodeOps Core Services](/Core-Services)
- Discover [NodeOps Console](/Guides/Console) for Node-as-a-Service
- Browse the [NodeOps Cloud Marketplace](/Guides/Marketplace) for decentralized Compute
