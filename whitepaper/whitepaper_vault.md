# Art Protocol : vault service planned

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









