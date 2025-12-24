# Art Protocol : vault service

## 1. ERC-4626 yield bearing token 

<img width="750" height="300" alt="image" src="https://github.com/user-attachments/assets/81b3b7eb-72f2-464c-ae38-388f60a52038" />

ERC-4626, the Tokenized Vault Standard, is a crucial advancement in decentralized finance (DeFi), designed to standardize how yield-bearing vaults operate. 
By extending the ERC-20 token standard, it introduces a unified framework that simplifies integration, improves security, and enhances interoperability across DeFi protocols. 

Users can deposit ERC-20 tokens into vaults and receive proportional shares, while vaults deploy strategies to generate yield. 
This consistency reduces complexity for developers and improves the user experience by enabling smoother interactions across platforms. 
Major DeFi projects like Yearn Finance and Balancer have already adopted ERC-4626, signaling its growing importance. 

As the DeFi space evolves, ERC-4626 is set to become a foundational standard for yield-generating applications.



## 2. ERC-4626 Tokenized Vault Standard : https://ethereum.org/

ERC-4626 is a standard to optimize and unify the technical parameters of yield-bearing vaults. It provides a standard API for tokenized yield-bearing vaults that represent shares of a single underlying ERC-20 token. ERC-4626 also outlines an optional extension for tokenized vaults utilizing ERC-20, offering basic functionality for depositing, withdrawing tokens and reading balances.

### ERC-4626 in yield-bearing vaults
https://ethereum.org/ko/developers/docs/standards/tokens/erc-4626/

### Asynchronous vault extension (ERC-7540)
ERC-4626 supports only atomic (instant) deposits and redemptions, making it unsuitable for asynchronous protocols like RWA, lending, or staking. ERC-7540 extends ERC-4626 by enabling asynchronous requests, allowing users to submit deposit or redemption actions that can be fulfilled later, making it more suitable for delayed or multi-step processes.

https://eips.ethereum.org/EIPS/eip-7540

### Multi-asset vault extension (ERC-7575)
ERC-4626 is limited to single-asset vaults since it must be an ERC-20 token. ERC-7575 solves this by separating the token from the vault, enabling support for multi-asset vaults like LP tokens or RWA portfolios.

https://eips.ethereum.org/EIPS/eip-7575


## 3. Art Protocol's vault service (Concept)
### MVP planned

<img width="935" height="330" alt="image" src="https://github.com/user-attachments/assets/5ea9c51f-c94a-4a6c-b8f6-6709a45ec293" />

① Vault owner register Vault

② Vault user deposit assets(wrapped assets)

③ Vault owner get assets(wrapped assets)

④ Vault owner deposit earn

⑤ Vault user withdraw assets(wrapped assets) + earn


## 4. Vault User Operations
1. User Onboarding & Wallet Generation

Users begin by creating a PIGLUCK account through the platform interface.

Upon sign-up, the system generates a non-custodial EVM-compatible wallet for the user.

The wallet serves as the user’s unique on-chain identity and is used for:

Vault deposits

Vault share accounting

Withdrawals

Reward distribution

Private keys are managed securely according to the selected wallet model (user-controlled or secure key management solution).

This process abstracts blockchain complexity while preserving Web3 ownership principles.

2. Asset Deposit into Vault

Once the wallet is created, users can deposit supported assets into a selected Vault.

Supported Asset (example): USDT (Profit Vault)

Users choose a Vault and specify the deposit amount.

Assets are transferred from the user’s wallet to the Vault smart contract.

In return, the user receives Vault share tokens representing proportional ownership of the Vault’s total assets.

All deposits are handled by smart contracts compliant with ERC-4626, ensuring transparency and standardization.

3. Vault Asset Balance & Reporting

Users can view their Vault position at any time through the dashboard.

Displayed information includes:

Deposited principal

Current Vault balance

Accrued yield (if applicable)

Share-to-asset conversion value

Historical deposit and withdrawal records

Vault balances are calculated on-chain and reflect real-time Vault performance.

4. Asset Withdrawal from Vault

Users may withdraw assets partially or fully, subject to Vault-specific rules.

Withdrawal requests burn the corresponding Vault share tokens.

The equivalent amount of underlying assets (e.g., USDT) is returned to the user’s wallet.

Withdrawal liquidity depends on the Vault type:

Profit Vault: Subject to liquidity conditions and yield cycles

Bitcoin Vault: Asset conversion based on BTC holdings

Artwork Vault: Partial liquidity supported without liquidating the entire collection

All withdrawals are executed transparently via smart contracts.

5. Profit Vault: Automated Crypto Card Top-Up

The Profit Vault introduces a unique operational flow that bridges DeFi yield with real-world usage.

Yield Distribution Mechanism

Vault generates yield through high-yield DeFi strategies.

The total Vault size is capped to prevent yield dilution.

A portion of realized yield (targeting ~10% monthly) is allocated for user rewards.

Card Top-Up Flow

Yield is calculated at the Vault level.

User-specific reward amounts are determined based on Vault share ownership.

Rewards are automatically converted into crypto card balance credits.

Users can immediately use the credited balance for real-world payments.

This mechanism transforms passive yield into usable financial utility, rather than idle on-chain balances.

6. Operational Flow Summary
Sign Up
  ↓
EVM Wallet Generation
  ↓
Vault Deposit (USDT)
  ↓
Vault Share Issuance
  ↓
Vault Yield / Asset Management
  ↓
• Balance Tracking
• Withdrawal (USDT)
• (Profit Vault only) Auto Card Top-Up

7. Key User Experience Principles

Simplicity: Complex DeFi mechanics are abstracted behind a clean UX.

Transparency: All balances and flows are verifiable on-chain.

Utility: Yield is not only accumulated but actively usable.

Control: Users retain ownership and withdrawal rights at all times.





