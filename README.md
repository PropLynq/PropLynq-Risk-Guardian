# PropLynq Risk Guardian — MT5 Drawdown Monitor & TradingView Risk Tools

**PropLynq Risk Guardian** is a collection of proprietary trading risk-management utilities for **MetaTrader 5 (MT5)** and **TradingView**. The tools are designed to help traders understand daily drawdown, maximum drawdown, trading-day requirements, profit-target progress, and pre-trade exposure.

Created by [PropLynq](https://proplynq.com/) for traders using simulated prop trading challenges and other configurable risk frameworks.

> **Availability:** This repository is the official documentation and distribution hub. The MT5 and TradingView tools are undergoing native-platform release validation. **No compiled MT5 download or public TradingView publication is claimed to be available yet.** Tool source code and internal development files are not distributed through this repository.

## Trading tools

| Tool | Platform | Main capabilities | Distribution |
| --- | --- | --- | --- |
| **Risk Guardian for MT5** | MetaTrader 5 (Expert Advisor; monitoring only) | Account equity observations, daily/max drawdown, configurable challenge presets, trading days, profit-target candidates, gap warnings, risk scenarios | Compiled `.ex5` when validated and released through an official channel |
| **Risk Guardian for TradingView** | TradingView | Configurable challenge limits, manual account snapshot, approximate risk visualization and data-integrity warnings | **Protected** Pine Script publication when approved |
| **Trade Planner for TradingView** | TradingView | Position sizing, stop-loss scenarios, approximate risk/reward and drawdown-pressure estimates | **Protected** Pine Script publication when approved |

### Risk settings

The intended tools support configurable **daily loss limits**, **maximum drawdown** (static or trailing where appropriate), **starting balance**, **profit targets**, **trading-day requirements**, and user-defined rule parameters. Presets are convenience references, not authoritative verification of a provider's current terms. Confirm all limits and reset rules with your account provider.

### Important limitations

- **MT5 monitoring requires MT5 to remain connected** while trades are open to collect local equity observations. Missing historical floating-equity peaks and troughs cannot be reconstructed with certainty.
- **TradingView Pine cannot connect to an MT5 account or obtain live broker equity**. The Risk Guardian's manual snapshot or explicitly selected indicator proxy is **not** independent account verification.
- The Trade Planner uses assumptions about instrument contracts, currency conversion and execution; its projections are not guaranteed prices or fills.
- Profit-target and drawdown indications are **informational**, not official evaluations. These tools do not open or close trades and cannot guarantee a challenge result or trading outcome.
- Native compilation, broker demo checks and platform approval must be completed before downloadable tools are described as available or production-certified.

## Installation and releases

**MT5:** When an official compiled release is available, install the `.ex5` in the MT5 terminal's `MQL5/Experts/` folder and use it on a demo account first. Do not install purported third-party builds or files from unverified sources.

**TradingView:** When the official **Protected** scripts are published, open their TradingView pages and select **Add to favorite indicators** or **Use on chart** as offered by TradingView. Protected publications allow traders to use indicators without seeing their Pine source (subject to TradingView plan and publication rules).

Official download links and version details will be added **only after the releases exist and have passed verification**. Do not treat the current repository as a binary download.

## Frequently asked questions

**Is PropLynq Risk Guardian a trading bot?** No. MT5 Guardian is an account-monitoring Expert Advisor; the TradingView indicators are monitoring/planning aids. They do not place trades.

**Can TradingView monitor an MT5 account automatically?** No. The Pine tools do not have access to an MT5 account or its trading history.

**Does MT5 continue recording risk when my computer is off?** No. Local recording stops unless MT5 is running in another continuously operating environment. Unobserved periods must not be assumed compliant.

**Can I use these tools with rules from another prop firm?** Configurable limits allow personal planning under different rule frameworks. Always enter the correct terms; this does not indicate affiliation with other providers.

**Is this repository open source?** **No.** This public repository contains product information and user guidance, not the proprietary source code. Copyright and software rights are reserved; see [`LICENSE`](LICENSE).

**When will download links be available?** After the applicable platform compilation, runtime checks and release approval. No release date is promised here.

## Official publisher and licensing

Published by **[PropLynq](https://proplynq.com/)**. This repository provides documentation and release information for the **MT5 Risk Guardian** and **TradingView Risk Guardian/Trade Planner** only.

Copyright © 2026 PropLynq. All rights reserved. **No permission is granted to copy, reuse, redistribute, resell or republish proprietary program source through this repository.** Separately released compiled tools may include their own end-user terms. See [`LICENSE`](LICENSE) and [`SECURITY.md`](SECURITY.md).

**Disclaimer:** Educational risk-management information only. Not investment advice. No warranty, guaranteed performance, guaranteed account status, or official third-party account verification.
