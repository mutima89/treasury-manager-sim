<div align="center">
  <br>
  <h1>&#127974; Global Treasury Manager</h1>
  <p><strong>FX Hedging &amp; Cash Sweep Simulator · Educational Edition</strong></p>
  <p>
    <em>Manage 5 multinational subsidiaries across 4 currencies.
    <br>Hedge FX exposure. Sweep cash. Minimize losses.</em>
  </p>
  <br>
  <p>
    <a href="#-features"><img src="https://img.shields.io/badge/Features-📋-06b6d4?style=for-the-badge" alt="Features"></a>
    <a href="#-educational-value"><img src="https://img.shields.io/badge/Education-📖-14b8a6?style=for-the-badge" alt="Education"></a>
    <a href="#-quick-start"><img src="https://img.shields.io/badge/Quick_Start-▶-0891b2?style=for-the-badge" alt="Quick Start"></a>
    <a href="#-theory"><img src="https://img.shields.io/badge/Theory-🎓-06b6d4?style=for-the-badge" alt="Theory"></a>
  </p>
  <br>
  <p>
    <img src="https://img.shields.io/badge/Chart.js-4.x-FF6384?style=flat-square&logo=chartdotjs&logoColor=white" alt="Chart.js">
    <img src="https://img.shields.io/badge/vanilla-JS-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="Vanilla JS">
    <img src="https://img.shields.io/badge/dependencies-Chart.js_only-22c55e?style=flat-square" alt="Minimal Dependencies">
    <img src="https://img.shields.io/badge/license-MIT-22c55e?style=flat-square" alt="MIT License">
    <img src="https://img.shields.io/badge/status-active-22c55e?style=flat-square" alt="Status Active">
  </p>
  <br>
</div>

---

## &#128203; Overview

**Global Treasury Manager** is an interactive, real-time browser-based simulation that places you in the seat of a **corporate treasurer** at a multinational company. You manage FX exposure and liquidity across 5 subsidiaries in 4 currencies, using forward contracts and cash sweeps to protect the company's P&amp;L.

> *"Every day, currencies move. Every day, cash flows. Your job: make sure neither one sinks the company."*

Built as a **single HTML file** — open in any browser and press Start.

### Who Is This For?

| Audience | Use Case |
|----------|----------|
| **Corporate Treasury Professionals** | Practice FX hedging strategy and cash concentration techniques |
| **Finance Students** | See FX risk management in action with live P&amp;L attribution |
| **CFO / FP&A Aspirants** | Understand how currency volatility affects multinational P&amp;L |
| **Business School Educators** | Demonstrate hedging, cash sweeps, and liquidity management |
| **Self-Taught Finance Enthusiasts** | Explore corporate treasury through an interactive simulation |

---

## &#10024; Features

### Core Simulation

| Feature | Description |
|---------|-------------|
| **5 Multinational Subsidiaries** | US (HQ), EU, UK, Japan, Brazil — each with local currency, cash balance, and daily cash flows |
| **4 Currency Pairs** | EUR/USD, GBP/USD, USD/JPY, USD/BRL — each with configurable volatility |
| **GBM FX Rate Process** | Exchange rates follow Geometric Brownian Motion with realistic volatility |
| **Forward Contracts** | Hedge FX exposure by locking in rates for future cash flows |
| **Automatic Cash Sweeps** | Excess cash is swept to a central pool; deficits are covered from it |
| **Daily Cash Flows** | Each subsidiary generates random daily net cash flows with seasonal patterns |
| **Overdraft Detection** | Negative cash balances trigger expensive overdraft fees |

### Educational Features

| Feature | Description |
|---------|-------------|
| **P&L Attribution Waterfall** | Visual breakdown: FX Translation + Hedge Settlement + Interest &minus; Overdraft Fees |
| **Per-Currency Hedge Ratios** | Individual sliders for each currency (0–100%) — set different strategies per region |
| **Educational Theory Panel** | Collapsible sidebar with treasury concepts, hedging mechanics, and scenario guides |
| **Color-Coded Log** | Every hedge settlement, sweep, and overdraft explained in plain English |
| **4 Scenario Injectors** | EM Crisis, EUR Weakens, Global Risk-Off, Liquidity Crunch |
| **Subsidiary Dashboard** | Each sub shown with flag, cash balance, USD equivalent, daily flow, status, hedge slider |
| **Consolidated Chart** | Total USD cash + FX rate overlay for visual correlation analysis |

### Interactive Controls

| Control | Range | Purpose |
|---------|-------|---------|
| **FX Volatility** | 2–25% | Global FX volatility multiplier |
| **Sweep Threshold** | 5–50% | % above/below target cash that triggers a sweep |
| **Interest Rate** | 1–12% | Annual interest rate on central pool balance |
| **Speed** | 1×–5× | Simulation speed |
| **Overdraft Cost** | 5–40% APR | Annual penalty rate for negative cash balances |
| **Hedge Ratios** | 0–100% | Per-currency, set independently via sliders on subsidiary cards |

---

## &#127937; Quick Start

```bash
# 1. Open the HTML file in any modern browser
open index.html

# 2. Review your 5 subsidiaries (shown as cards with flags)
#    - Each has a cash balance, daily flow, and current FX rate

# 3. Set hedge ratios for each currency using the sliders
#    - EUR: 60%, GBP: 40%, JPY: 20%, BRL: 10%
#    - Higher ratio = more protection, but more hedge cost

# 4. Press "Start"
#    FX rates move, cash flows arrive, hedges settle, sweeps execute

# 5. Watch the P&L waterfall — learn where your gains/losses come from

# 6. Use scenario buttons to test extreme conditions
#    - EM Crisis: BRL drops 20%
#    - EUR Weakens: EUR drops 8%
#    - Risk-Off: All EM currencies sell off
#    - Liquidity Crunch: All subsidiaries hit simultaneously
```

### System Requirements

| Requirement | Detail |
|-------------|--------|
| **Browser** | Chrome, Firefox, Edge, Safari |
| **Internet** | Once (for Chart.js CDN) |
| **Dependencies** | Chart.js 4.x |
| **Storage** | ~250 KB |
| **OS** | Windows, macOS, Linux |

---

## &#127974; The Five Subsidiaries

| Sub | Currency | Flag | Initial Cash | Daily Flow | FX Vol | Key Risk |
|-----|----------|------|-------------|------------|--------|----------|
| **US HQ** | USD | 🇺🇸 | $2,000,000 | +$8,000 | — | None (base currency) |
| **EU Ops** | EUR | 🇪🇺 | €800,000 | −€2,500 | 7% | Largest non-USD exposure |
| **UK Sub** | GBP | 🇬🇧 | £500,000 | +£1,500 | 6% | Moderate exposure |
| **Japan** | JPY | 🇯🇵 | ¥10,000,000 | −¥60,000 | 8% | Large notional, low per-unit vol |
| **Brazil** | BRL | 🇧🇷 | R$500,000 | +R$3,000 | 14% | Highest volatility |

---

## &#127891; Educational Value

### What You Will Learn

| Concept | How the Simulator Teaches It |
|---------|------------------------------|
| **FX Transaction Exposure** | Each subsidiary's cash flows in local currency — when converted to USD, the value fluctuates with FX rates |
| **FX Translation Exposure** | Even without cash movement, the USD value of foreign cash balances changes daily with FX rates |
| **Forward Hedging** | Setting a hedge ratio per currency creates forward contracts that lock in rates, offsetting FX P&L |
| **The Hedge Ratio Tradeoff** | 0% = full exposure to FX (volatile P&L). 100% = no exposure but forward costs. The optimal ratio depends on your risk tolerance. |
| **Cash Concentration** | Sweeping excess cash to a central pool earns interest and prevents overdrafts in other subsidiaries |
| **Overdraft Cost** | Negative cash balances trigger daily penalties at configurable APR — motivates proactive cash management |
| **P&L Attribution** | The waterfall chart decomposes total P&L into FX translation, hedge settlement, interest income, and overdraft fees |
| **Correlation & Diversification** | Different currencies have different volatilities and correlations — a diversified hedge strategy matters |
| **Scenario Testing** | Use EM Crisis, EUR Weakens, Risk-Off, and Liquidity Crunch to stress-test your treasury strategy |

### Suggested Learning Path

1. **Start with 50% hedge on all currencies.** Observe how the P&L waterfall behaves over 20–30 days.
2. **Drop all hedges to 0%.** See the P&L volatility increase. Run the EM Crisis scenario — watch your Brazilian subsidiary's value collapse.
3. **Set EUR hedge to 100%, others to 0%.** Run the EUR Weakens scenario. See how a perfect hedge on one currency protects it while others are exposed.
4. **Experiment with sweep thresholds.** Set it high (50%), then low (5%). Observe how overdrafts change.
5. **Hit the Liquidity Crunch scenario.** See how fast overdrafts accumulate when multiple subsidiaries hit cash shortfalls simultaneously.
6. **Try a dynamic strategy.** Adjust hedge ratios periodically based on market conditions.

---

## &#127891; Theory

### FX Exposure Types

| Exposure Type | Definition | In This Simulator |
|---------------|-----------|-------------------|
| **Transaction** | P&L impact of converting foreign cash flows at spot rates | Daily cash flows × (spot rate − hedge rate) |
| **Translation** | Change in USD value of foreign cash balances due to rate moves | Cash balance × (current rate − previous rate) |

### How Forward Hedging Works

A forward contract locks in an exchange rate today for a future cash flow:

```
Forward Rate ≈ Spot Rate × e^((r_USD − r_local) × T)

Hedge P&L at Settlement = Qty × (Locked Rate − Spot Rate)
```

- If the spot rate moves **against** you (currency weakens), the forward pays you → offsets the FX loss
- If the spot rate moves **in your favor** (currency strengthens), you pay the forward → caps the FX gain

### P&L Decomposition

```
Total Treasury P&L = FX Translation + Hedge Settlement + Interest Income − Overdraft Fees
```

| Component | Sign | What It Represents |
|-----------|------|-------------------|
| **FX Translation** | ± | USD value change of foreign cash due to FX rate moves |
| **Hedge Settlement** | ± | Net P&L from maturing forward contracts |
| **Interest Income** | + | Interest earned on the central treasury pool |
| **Overdraft Fees** | − | Penalties for negative subsidiary cash balances |

### The Hedge Ratio Spectrum

| 0% Hedge | 50% Hedge | 100% Hedge |
|----------|-----------|------------|
| Full FX exposure | Balanced protection | No FX exposure |
| Highest P&L volatility | Moderate volatility | Zero FX P&L impact |
| No hedge cost | Moderate hedge cost | Highest hedge cost |
| Max upside/downside | Capped upside/downside | Predictable outcome |

---

## &#127911; Scenarios

| Scenario | Trigger | What Happens | Teaches |
|----------|---------|-------------|---------|
| **EM Crisis** | 🇧🇷 BRL −20% | Brazilian Real crashes. Unhedged BRL exposure takes a major hit. | Emerging market risk premium |
| **EUR Weakens** | 🇪🇺 EUR −8% | Euro weakens sharply against USD. Largest non-USD sub is impacted. | Concentration risk |
| **Risk-Off** | 🌐 All EM −15% | Global risk aversion hits all currencies. Tests diversified hedging. | Correlation in crises |
| **Liquidity Crunch** | 💧 All subs −30–50% | Major customer delays payments across the board. Cash deficits everywhere. | Liquidity planning |

---

## &#128187; Interface Guide

```
┌────────────────────────────────────────────────────────────────────┐
│ 🌐 Global Treasury · FX Hedging & Cash Sweep Sim      [Theory][▶] │
├────────────────────────────────────────────────────────────────────┤
│ EUR/USD 1.0800 | GBP/USD 1.2700 | USD/JPY 150.0 | BRL 5.26 ...   │
├────────────────────────────────────────────────────────────────────┤
│ [Stats: Subs 5 | Hedges 0 | Sweeps 0 | ODs 0 | P&L +$0 | ...]    │
├────────────────────────────────────────────────────────────────────┤
│ [P&L Waterfall: FX Translation | Hedge | Overdraft | Interest]    │
├────────────────────────────────────────────────────────────────────┤
│ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐          │
│ │🇪🇺 EU  │ │🇬🇧 UK  │ │🇯🇵 JP  │ │🇧🇷 BR  │ │🇺🇸 US  │          │
│ │Cash..  │ │Cash..  │ │Cash..  │ │Cash..  │ │Cash..  │          │
│ │Hedge:◉─│ │Hedge:─◉│ │Hedge:─│ │Hedge:─│ │(base)  │          │
│ └────────┘ └────────┘ └────────┘ └────────┘ └────────┘          │
├────────────────────────────────────────────────────────────────────┤
│ [Chart: Consolidated Cash + FX Rates]                             │
├────────────────────────────────────────────────────────────────────┤
│ [Controls: Vol | Sweep | Rate | Speed | OD]         [Scenarios]  │
├────────────────────────────────────────────────────────────────────┤
│ [Active Hedges Table]                    [Treasury Activity Log] │
└────────────────────────────────────────────────────────────────────┘
```

---

## &#128679; Project Structure

```
treasury-manager-sim/
├── index.html      # Complete simulator (single-file)
├── README.md       # This file
└── LICENSE         # MIT License
```

### Technologies

| Technology | Purpose |
|------------|---------|
| **HTML5** | Structure |
| **CSS3** | Dark-themed enterprise dashboard |
| **Vanilla JS** | All simulation logic, FX math, and UI |
| **Chart.js 4.x** | Real-time chart (CDN) |

---

## &#128220; License

MIT — see [`LICENSE`](LICENSE).

---

## &#9888; Disclaimer

Educational tool only. All market data is synthetically generated. Nothing herein constitutes financial advice.

---

<div align="center">
  <br>
  <p><sub><em>"The best hedge is the one you have in place before the currency moves."</em></sub></p>
  <br>
</div>
