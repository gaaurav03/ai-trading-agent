# 🤖 AI Trading Agent
 
> **An autonomous, AI-powered trading system** that analyzes live market data, computes technical indicators, and executes trades — all in real time.
 
[![Built with Bun](https://img.shields.io/badge/Runtime-Bun-black?style=flat-square&logo=bun)](https://bun.sh)
[![TypeScript](https://img.shields.io/badge/Language-TypeScript-3178C6?style=flat-square&logo=typescript)](https://www.typescriptlang.org)
[![Prisma](https://img.shields.io/badge/Database-Prisma-2D3748?style=flat-square&logo=prisma)](https://www.prisma.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)
 
---
 
## 🌟 Overview
 
AI Trading Agent is a **modular, production-grade trading automation system** built for speed and extensibility. It combines real-time market data ingestion, rule-based and AI-driven decision logic, and programmatic order execution into a single cohesive pipeline — all powered by [Bun](https://bun.sh) for blazing-fast TypeScript performance.
 
> ⚠️ **Disclaimer:** This project is for educational and experimental purposes only. It does not constitute financial advice. Use at your own risk.
 
---
 
## ✨ Features
 
| Feature | Description |
|---|---|
| 📊 **Market Data Analysis** | Fetches and processes real-time stock and market data |
| 📈 **Technical Indicators** | Built-in calculations (e.g., RSI, moving averages) for signal generation |
| 🤖 **AI Decision Engine** | Prompt-driven logic to simulate intelligent, context-aware trading |
| 💼 **Portfolio Management** | Track holdings, open positions, and account balance |
| ⚡ **Order Execution** | Create, manage, and cancel orders programmatically |
| 🔄 **Real-time Price Tracking** | Continuously monitors price movements and updates state |
| 🧩 **Modular Architecture** | Clean service-based structure for easy extensibility |
 
---
 
## 🏗️ Project Structure
 
```
ai-trading-agent/
│
├── frontend/             # Frontend interface (visual dashboard)
├── prisma/               # Database schema & migrations
├── types/                # Shared TypeScript type definitions
├── lighter-sdk-ts/       # Custom SDK integration layer
│
├── index.ts              # 🚀 Main entry point
├── backend.ts            # Backend orchestration logic
├── config.ts             # Environment & app configuration
│
├── stockData.ts          # Market data fetching & normalization
├── indicators.ts         # Technical indicator calculations
├── priceTracker.ts       # Real-time price monitoring loop
│
├── createPosition.ts     # Open new trade positions
├── cancelOrder.ts        # Cancel existing orders
├── openPositions.ts      # Query active positions
├── getPortfolio.ts       # Portfolio snapshot & analytics
├── accounts.ts           # Account & balance management
│
├── markets.ts            # Market metadata & utilities
├── prompt.ts             # AI decision prompts & templates
│
├── prisma.config.ts      # Prisma ORM configuration
├── package.json
├── tsconfig.json
└── bun.lock
```
 
---
 
## ⚙️ Installation
 
**Prerequisites:** [Bun](https://bun.sh) runtime
 
```bash
# Install Bun (if not already installed)
curl -fsSL https://bun.sh/install | bash
 
# Clone the repository
git clone https://github.com/gaaurav03/ai-trading-agent.git
cd ai-trading-agent
 
# Install dependencies
bun install
```
 
---
 
## ▶️ Running the Project
 
```bash
bun run index.ts
```
 
---
 
## 🧠 How It Works
 
The agent operates as an automated pipeline with five core stages:
 
```
  [1] Fetch Market Data
         ↓
  [2] Apply Technical Indicators
         ↓
  [3] AI Prompt → Decision Engine
         ↓
  [4] Execute Trade (Create / Cancel)
         ↓
  [5] Update Portfolio & Track Prices
```
 
1. **Data Ingestion** — `stockData.ts` fetches live market prices and OHLCV data
2. **Signal Generation** — `indicators.ts` computes technical signals (RSI, MAs, etc.)
3. **AI Decision** — `prompt.ts` feeds context into an AI prompt to determine buy/sell/hold
4. **Execution** — `createPosition.ts` / `cancelOrder.ts` act on the decision
5. **State Update** — `priceTracker.ts` and `getPortfolio.ts` keep everything in sync
 
---
 
## 🛠️ Tech Stack
 
| Layer | Technology |
|---|---|
| **Runtime** | [Bun](https://bun.sh) — ultra-fast JS/TS runtime |
| **Language** | [TypeScript](https://www.typescriptlang.org) — end-to-end type safety |
| **Database ORM** | [Prisma](https://www.prisma.io) — type-safe DB access |
| **AI Logic** | Prompt-driven decision system via LLM integration |
| **Architecture** | Modular, service-based with clear separation of concerns |
 
---
 
## 🔭 Roadmap
 
- [ ] 🔐 Risk management strategies (stop-loss, position sizing)
- [ ] 📉 Backtesting engine with historical data
- [ ] 🌐 Web dashboard with visual analytics
- [ ] 🤝 Broker API integrations (Alpaca, Interactive Brokers)
- [ ] 🧠 Advanced ML models for signal prediction
 
---
 
## 👤 Author
 
**Gaurav Gupta**
🐙 GitHub: [@gaaurav03](https://github.com/gaaurav03)
 
---
 
<p align="center">
  Built with ⚡ Bun · TypeScript · Prisma
</p>
 
