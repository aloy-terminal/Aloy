# Aloy

**Unified Trading, Market Intelligence & Developer Infrastructure for LayerZero Zero**

*One terminal. Two execution rails. Unified market intelligence.*

![Status](https://img.shields.io/badge/Status-Implementation%20%26%20Research-yellow)
![Ecosystem](https://img.shields.io/badge/Ecosystem-LayerZero%20Zero-blue)
![Development](https://img.shields.io/badge/Development-Pre--Integration-orange)

## Overview

**Aloy** is a proposed non-custodial trading infrastructure and market intelligence platform designed for the **LayerZero Zero ecosystem**.

Aloy brings together two complementary trading environments within a single professional interface:

- **ATLAS Trading Rail:** Integration with LayerZero's ATLAS order-book infrastructure for perpetual derivatives, supported spot markets, order execution, market-depth analytics, position management, and professional trading workflows.

- **EVM/AMM Trading Rail:** Integration with permissionless Automated Market Makers (AMMs), token launchpads, bonding-curve markets, and other supported liquidity protocols deployed within Zero's EVM-compatible environment. This rail focuses on token discovery, memecoin trading, liquidity analytics, and decentralized swap execution.

Alongside the trading terminal, Aloy aims to make its underlying infrastructure available to other applications, protocols, trading venues, and developers within the Zero ecosystem.

The project is organized around two complementary products:

1. **Aloy Terminal** — A professional, unified trading interface providing access to ATLAS order-book markets and supported EVM/AMM liquidity through a consistent experience.

2. **Aloy Infrastructure** — A modular collection of indexing services, market-data APIs, analytics engines, execution adapters, developer SDKs, and embeddable components that power Aloy Terminal and can be integrated into third-party applications.

Both products share the same technical foundation.

The goal is not simply to build another trading interface. Aloy aims to provide the intelligence, execution capabilities, and developer infrastructure needed to make trading across Zero's distinct liquidity environments more accessible, transparent, and efficient.


### Core Product Thesis

Zero's architecture creates the opportunity for two complementary forms of onchain liquidity:

- **Order-book liquidity through ATLAS**, supporting perpetual derivatives, spot markets, and other markets enabled by its trading infrastructure.
- **Permissionless smart-contract liquidity through Zero's EVM environment**, potentially supporting AMMs, memecoins, token launchpads, and bonding-curve markets.

Aloy's thesis is that traders should be able to discover, analyze, execute, and manage their trading activity across both environments without navigating entirely separate applications.

At the same time, developers building products on Zero should be able to reuse common infrastructure rather than independently building market-data pipelines, execution integrations, and analytics systems.




---

## Vision

As blockchain networks develop specialized execution environments, liquidity can become distributed across different protocols, smart contracts, and trading venues.

Within Zero, ATLAS introduces order-book-based trading infrastructure, while its general-purpose EVM environment provides a potential foundation for smart-contract-based liquidity protocols.

These environments may serve different types of traders and markets.

ATLAS can support professional trading workflows, derivatives, order-book liquidity, and sophisticated market participants.

The EVM environment can potentially support permissionless token launches, memecoin trading, AMM liquidity, and emerging token ecosystems.

Although these environments operate differently, users may benefit from accessing them through a consistent interface.

Traders need more than the ability to submit transactions. They need reliable information about:

- Available spot and derivatives markets.
- Newly launched tokens.
- Order-book depth.
- AMM liquidity.
- Market prices and trading volume.
- Execution costs.
- Token and market risks.
- Open positions and portfolio exposure.
- Transaction and order status.
- Liquidity availability across supported venues.

Meanwhile, developers building trading applications repeatedly need similar underlying infrastructure:

- Blockchain and exchange-event indexing.
- Market and token discovery.
- Real-time market-data feeds.
- Historical price and volume data.
- Order-book and liquidity analytics.
- Transaction and order execution interfaces.
- Protocol-specific adapters.
- Portfolio and position data.
- Developer APIs and integration tools.

Aloy intends to provide these capabilities through a common infrastructure foundation.

**Our long-term vision is to unify the trading experience across ATLAS and permissionless EVM markets while making the underlying market intelligence and execution infrastructure reusable by other applications.**



---

## The Problem

### 1. Fragmented Trading Environments

Different execution environments require different interfaces, account models, market-data systems, and trading workflows.

Order-book trading and AMM trading have distinct mechanisms.

A derivatives trader may need order-book depth, position information, margin requirements, funding rates, and order management.

A memecoin trader may need token discovery, liquidity pool analytics, contract-risk indicators, and swap execution.

Without a unified interface, users may need multiple applications to understand and interact with the broader ecosystem.

Aloy aims to reduce this fragmentation while preserving the technical distinctions between these markets.


### 2. Limited Visibility Into Liquidity and Execution Quality

A displayed market price does not necessarily represent the price at which a meaningful trade can be executed.

For AMMs, execution quality may depend on:

- Pool reserves or active liquidity.
- Order size.
- Trading routes.
- Swap fees.
- Price impact.
- Transfer restrictions.
- Transaction ordering.
- Network costs.

For ATLAS order-book markets, execution quality may depend on:

- Bid and ask depth.
- Available liquidity at different price levels.
- Order size.
- Spread.
- Supported order types.
- Market volatility.
- Trading fees.
- Order execution and settlement behavior.

Aloy intends to help users evaluate these factors within one trading environment.

### 3. Infrastructure Duplication

Developers building trading terminals, analytics platforms, wallets, market dashboards, and other financial applications repeatedly need similar services.

These include market-data ingestion, historical candles, liquidity analytics, transaction monitoring, and execution integrations.

Rebuilding these systems across multiple applications introduces engineering costs and inconsistent implementations.

Aloy aims to provide reusable services that developers can integrate instead of rebuilding the same foundational components.


### 5. Cross-Market Portfolio Fragmentation

Users interacting with multiple trading environments may struggle to understand their combined exposure.

Spot balances, derivatives positions, collateral, fees, and trading histories may be distributed across different account systems.

Aloy aims to consolidate supported information into a coherent portfolio view without implying that the underlying assets, balances, or execution systems are interchangeable.

---

## Our Solution

Aloy will be developed around six complementary capabilities.

### 1. Unified Trading Access

Provide one terminal for supported ATLAS order-book markets and EVM/AMM markets.

The interface will adapt its trading controls to each market's execution mechanism.

### 2. Market Discovery

Enable discovery of:

- ATLAS spot and derivatives markets.
- Supported AMM tokens and pools.
- Newly created liquidity pools.
- Token launches.
- Bonding-curve markets.
- Active and emerging trading opportunities.

Discovery functionality will depend on verified integrations and market-data availability.

### 3. Unified Market Intelligence

Provide analytics appropriate to each trading environment, including:

- Market prices.
- Trading volume.
- Order-book depth.
- AMM liquidity.
- Historical charts.
- Execution-cost estimates.
- Market activity.
- Token risk indicators.
- Position and portfolio analytics.

### 4. Non-Custodial Trading

Allow users to execute supported trades through the appropriate market infrastructure while retaining control of their assets and authorization.

ATLAS orders and EVM swaps will use distinct execution adapters.

Aloy will not assume that one transaction model applies to both environments.

### 5. Shared Portfolio Visibility

Provide a common interface for balances, positions, trading activity, and eventually consolidated PnL across supported markets.

### 6. Reusable Developer Infrastructure

Expose selected indexing, market-data, analytics, and execution capabilities through APIs, SDKs, and embeddable components.

This infrastructure will support both Aloy Terminal and third-party applications.


---

## Aloy Terminal

Aloy Terminal is the planned user-facing application.

It is designed for traders interacting with supported order-book and permissionless token markets.

Its interface will provide a unified workspace while adapting the trading experience to each execution mechanism.

### 1. Unified Market Discovery

Planned discovery capabilities include:

**ATLAS Markets**

- Available spot markets.
- Perpetual derivatives.
- Market categories.
- Trading pairs.
- Price changes.
- Trading volume.
- Market activity.
- Supported position and instrument information.

**EVM/AMM Markets**

- Newly created tokens.
- Newly created liquidity pools.
- Recently active markets.
- Token and pool search.
- Liquidity changes.
- Trading volume.
- Launchpad activity.
- Bonding-curve markets.
- Configurable token filters.

Discovery coverage will depend on the available market-data interfaces and supported protocols.

### 2. Professional Market Analytics

Aloy intends to provide:

- Real-time and historical charts.
- OHLCV candle generation.
- Market volume statistics.
- Price changes.
- Market liquidity information.
- Trade activity.
- Fee estimates.
- Watchlists.
- Market comparisons.

### 3. ATLAS Trading Workspace

The ATLAS interface is intended to provide professional order-book trading functionality.

Planned capabilities include:

- Order-book visualization.
- Bid and ask depth.
- Market spread information.
- Supported order types.
- Order placement and cancellation.
- Open orders.
- Fill history.
- Open positions.
- Position-size information.
- Collateral and margin information where supported.
- Unrealized PnL.
- Funding information for supported perpetual markets.
- Relevant liquidation and risk information.

Actual functionality will follow ATLAS's documented account, execution, and market-data interfaces.

### 4. EVM/AMM Trading Workspace

The EVM interface will support permissionless token market discovery and trading through verified protocols.

Planned capabilities include:

- Pool liquidity analysis.
- Token contract information.
- Token launch tracking.
- Swap quotes.
- Estimated price impact.
- Slippage configuration.
- Supported trading routes.
- Wallet-based swap execution.
- Transaction confirmation monitoring.
- Trade history.

### 5. Token Risk Intelligence

The platform aims to identify technical warning signs in supported EVM tokens, including:

- Unusual transfer restrictions.
- Trading permission limitations.
- Minting privileges.
- Owner or administrator controls.
- Upgradeable contracts.
- Transfer taxes or fees.
- Concentrated holder ownership.
- Liquidity concentration.
- Other protocol-specific risks.

These signals are intended to support informed decisions, not guarantee token safety.

### 6. Unified Portfolio

The terminal will work toward a consolidated view of:

- EVM wallet balances.
- Supported ATLAS account balances.
- Open positions.
- Token holdings.
- Trading history.
- Portfolio valuations.
- Realized and unrealized PnL where accurately supported.


--- 

## Assumptions and Dependencies

Aloy is at the research and pre-integration stage. The following are not yet confirmed:

| Item | Status |
|---|---|
| ATLAS venue onboarding, API and SDK access | Pending |
| ATLAS account and authorization model (including delegated signing) | Unknown |
| ATLAS supported order types and market-data interfaces | To be confirmed from ATLAS docs |
| Zero EVM Zone testnet, RPC and gas model | Pending |
| AMMs and launchpads deployed in the EVM Zone | None announced at the time of writing |
| Cross-zone (EVM Zone to ATLAS) transfer behavior | Unknown; treated as asynchronous with visible states |

ATLAS is an order-book engine and does not provide AMM pools. The EVM/AMM rail
integrates AMMs, launchpads and bonding-curve markets deployed in Zero's EVM Zone
through verified adapters, each activated only once a deployment is confirmed.


## What We Need From LayerZero

- ATLAS venue onboarding process, API/SDK documentation and test environment
- ATLAS account and authorization model, including delegated or session signing
- Rebate tier requirements and ZRO staking details for venues
- EVM Zone testnet access, RPC details, gas model and account-abstraction support
- Guidance on cross-zone transfers and any expected EVM-Zone DEX and launchpad deployments
