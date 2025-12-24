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






# Vault User Operations

## 1. User Onboarding & Wallet Generation

Users begin by creating a PIGLUCK account through the platform interface.

- Upon sign-up, the system generates a **non-custodial EVM-compatible wallet**.
- The wallet acts as the user’s on-chain identity and is used for:
  - Vault deposits
  - Vault share accounting
  - Withdrawals
  - Reward distribution
- Private keys are managed securely according to the selected wallet model.

This approach abstracts blockchain complexity while preserving Web3 ownership.

---

## 2. Asset Deposit into Vault

After wallet creation, users can deposit supported assets into a Vault.

- **Supported asset (example):** USDT (Profit Vault)
- Users select a Vault and enter the deposit amount.
- Assets are transferred to the Vault smart contract.
- Users receive **Vault share tokens** representing proportional ownership.

All deposits follow the **ERC-4626** standard.

---

## 3. Vault Asset Balance & Reporting

Users can monitor their Vault positions in real time.

Displayed information includes:
- Deposited principal
- Current Vault balance
- Accrued yield
- Share-to-asset conversion rate
- Historical transactions

All balances are calculated on-chain for full transparency.

---

## 4. Asset Withdrawal from Vault

Users may withdraw assets partially or fully, depending on Vault rules.

- Vault share tokens are burned upon withdrawal.
- Equivalent underlying assets (e.g., USDT) are returned to the user wallet.
- Liquidity depends on Vault type:
  - **Profit Vault:** Liquidity based on yield cycle
  - **Bitcoin Vault:** BTC conversion and availability
  - **Artwork Vault:** Partial liquidity without full asset liquidation

Withdrawals are executed via smart contracts.

---

## 5. Profit Vault: Automated Crypto Card Top-Up

The Profit Vault uniquely connects DeFi yield to real-world spending.

### Yield Distribution
- Yield is generated through high-yield DeFi strategies.
- Total Vault size is capped to prevent yield dilution.
- A portion of realized yield targets **~10% monthly rewards**.

### Card Top-Up Flow
1. Vault yield is calculated.
2. User rewards are allocated based on Vault share ownership.
3. Rewards are converted into crypto card balance.
4. Card balance becomes instantly usable for payments.

This enables **usable yield**, not just passive accumulation.

---

## 6. Operational Flow Summary

