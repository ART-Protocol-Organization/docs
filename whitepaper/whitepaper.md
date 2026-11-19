# ART Protocol Whitepaper

*Version 2.0 · November 2026*

> **Summary.** Artcoin (ART) is the internal utility token of ART Protocol. It is used to access and pay for services inside the ART Protocol platform. It is not an investment, and does not represent any ownership, profit, or claim. ART may be traded on third-party exchanges that ART Protocol does not operate or control.

---

## 1. Overview

ART Protocol is a Web3.0 platform for artwork and other real-world assets (RWA). It brings together:

- **Art&Asset Market**: an on-chain market for digital assets linked to certified collections (currently on BNB Smart Chain Testnet). After the market launches on mainnet, fees will be paid in ART through the market's internal wallet, which connects to the Base network where ART is issued.
- **ART INDEX**: benchmark data for the art market (ART100, ENVISAGER INDEX), provided for information only.
- **RWA collections**: certified artwork collections, starting with ENVISAGER MUSEUM and ENVISAGER CLUB.
- **AI agents**: on-chain agents (TeleZon, AI Village) that help users with tasks inside the platform.

Artcoin (ART) is the single utility token that runs these services, in the same way a platform token is used to pay fees inside its own platform.

## 2. Artcoin (ART)

### 2.1 Token information

| Item | Detail |
|---|---|
| Name / Symbol | Artcoin / ART |
| Type | Internal utility token (ERC-20) |
| Network | Base (Ethereum Layer 2) |
| Contract | [0xC33297B036aFbE0Da079B8Eba229a10964a30842](https://basescan.org/token/0xC33297B036aFbE0Da079B8Eba229a10964a30842) |
| Previous contracts | Ethereum and Polygon contracts are retired. All ART has been migrated to the Base contract above. |
| Total supply | 10,000,000,000 ART (current) → 1,000,000,000 ART after the planned burn |
| Circulating supply | ART held by external holders, included in the 1,000,000,000 ART (amount to be published with the planned burn) |
| Planned burn | 9,000,000,000 ART to be burned on-chain (burn transaction will be published when executed) |
| Issuer | Artcoin Foundation: issues and manages ART, including supply, reserves, and burns |
| Foundation location | Unknown |
| Operator | Art Protocol Inc.: operates the Art&Asset Market and other ART Protocol services. 3400 El Camino Real, Suite 9, Santa Clara, CA, USA |

### 2.2 What ART is used for

Inside ART Protocol, ART is used only for the following services:

1. **Service fees**: paying platform fees, such as market, market listing, and data-service fees.
2. **Fee discounts**: paying fees in ART instead of other assets can lower the fee.
3. **Feature access**: unlocking platform features, such as advanced ART INDEX data and partner tools offered within ART Protocol.
4. **AI agent tasks**: paying for tasks performed by ART Protocol AI agents.
5. **Community programs**: rewards for platform activity, such as testing, feedback, and content.

New uses are added only for services that ART Protocol itself operates.

### 2.3 What ART is not

- ART is **not** equity, debt, a profit share, a dividend, or interest, and gives no claim on ART Protocol, the Artcoin Foundation, or any asset.
- ART **cannot** be redeemed for money, artwork, or any physical asset.
- ART **cannot** be bought or sold on the Art&Asset Market or any other ART Protocol service.
- ART does **not** earn yield or rewards for simply holding it.
- ART Protocol does **not** sell ART as an investment or promote its price, and does **not** arrange, pay for, or support exchange listings, market making, or liquidity for ART.

### 2.4 How users obtain ART

- **Third-party exchanges**: ART is listed on third-party exchanges. These listings were not arranged, paid for, or supported by ART Protocol or the Artcoin Foundation, and ART Protocol does not operate, endorse, or control those exchanges. Prices there are set by their users, not by ART Protocol.
- **Community programs**: users can receive ART as rewards for platform activity (section 2.2).

Users are responsible for following the laws of their jurisdiction and the terms of any exchange they use.

## 3. Allocation

After the planned burn, the total supply of 1,000,000,000 ART (section 2.1) consists of:

- **Circulating supply**: ART already held by external holders. The amount will be published with the planned burn.
- **Internal reserves**: all remaining ART, held **for internal use within ART Protocol services only**.

The internal reserves are allocated as follows. Each allocation is spent only on the platform uses in section 2.2, or held as a reserve for the planned mainnet and platform security. Amounts in ART will be published together with the circulating supply.

| Allocation | Share of reserves | Internal use |
|---|---|---|
| Ecosystem Growth | 20% | Fee credits for users of new ART Protocol services and features |
| RWA Merchandising | 20% | Covering platform fees for artists and collections onboarding and certifying RWA |
| Protocol Development | 20% | Usage credits for testing platform features during protocol upgrades |
| Network Operations | 10% | Reserved for platform transaction fees on the planned ART Protocol mainnet |
| Community | 10% | Rewards for platform activity, such as testing, feedback, and content (section 2.2) |
| Strategic Partners | 10% | Access for partners that build or integrate services operated within ART Protocol |
| Foundation | 10% | Reserve held, not sold, for platform operations and security programs |
| **Total** | **100%** | |

**Internal-use rules**

- No allocation is sold, offered to investors, or distributed for trading.
- No allocation is used for exchange listings, market making, liquidity provision, or price support.
- ART given to users or partners is intended for use inside ART Protocol services. Because ART is a transferable ERC-20 token, this is an operating policy, not a technical restriction.
- Unused ART stays in reserve. ART spent on platform services may be burned (section 4).
- The schedule for moving ART from each allocation into platform use will be announced through the official channels (section 9).

## 4. Burn

ART spent on platform services (section 2.2) may be burned, which permanently removes it from the total supply. This includes ART paid by users and ART paid through fee credits and subsidies from the internal reserves (section 3).

- Burns are based on **service usage only**, not on company revenue or profit.
- Each burn is executed on-chain and announced with the transaction and the amount, shown separately for ART paid by users and ART paid from internal reserves.
- Burns are an operating policy for the platform, not a promise of any change in value.

## 5. Network

| Stage | Network | Status |
|---|---|---|
| 1 | Ethereum | Retired (migrated to Base) |
| 2 | Polygon | Retired (migrated to Base) |
| 3 | Base (Ethereum Layer 2) | **Current** |
| 4 | ART Protocol Mainnet (Proof-of-Stake) | Planned |

The planned mainnet is designed for platform transactions, RWA records, and AI agent activity. Its design, including validator requirements, is under development and will be published before launch. Validator and staking programs are **not offered** at this time.

## 6. AI agents

ART Protocol follows **ERC-8004 (Trustless Agents)**, currently a Draft standard, so that AI agents can be identified and trusted on-chain:

- **Identity Registry**: each agent has an on-chain identity (ERC-721) with metadata.
- **Reputation Registry**: feedback and scores build a reusable agent reputation.
- **Validation Registry**: task results are verified (validators, zero-knowledge proofs, TEEs) and recorded.

Users pay for agent tasks in ART (section 2.2).

## 7. RWA records

Certified artworks are linked to on-chain digital assets that record authentication, provenance, and transfer history. The rights of each holder are only those set out in that collection's documents. A digital asset does not by itself give legal title to, or a right to redeem, the physical work. Any collection that gives fractional, pooled, or profit-sharing interests is offered only in compliance with applicable securities laws.

## 8. Audit and governance

Smart contract audit results and the governance framework for ART will be published through the official channels (section 9).

## 9. Official channels

- Website: https://www.artprotocol.net
- Terms of Use: https://www.artprotocol.net/terms/
- Regulatory overview: https://www.artprotocol.net/regulations/
- Contact: artcoin64@gmail.com
- Address: Art Protocol Inc., 3400 El Camino Real, Suite 9, Santa Clara, CA, USA

## 10. Disclaimer

This whitepaper is for information only. It is not an offer to sell, or a solicitation to buy, any token, security, or financial product, and it is not investment, legal, or tax advice. ART is a utility token for use within ART Protocol services. ART Protocol makes no promise of profit, return, liquidity, or value. Plans described here, including the mainnet, burns, and new services, may change or may not happen, and some may be restricted by law in certain jurisdictions, including the United States and California. Digital assets and smart contracts carry risks, including loss of keys, software errors, and loss of value.
