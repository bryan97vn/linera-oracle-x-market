# linera-oracle-x-market

A modular **Prediction Market + Oracle** system built on **Linera Microchains**, designed for speed, scalability, and parallel execution.  
This project demonstrates how market logic, user-owned state, oracle data delivery, and cross-chain messaging work together on Linera.

---

## 🚀 Features

### **Prediction Market**
- Create markets (binary or multi-choice)
- Buy/Sell outcome shares
- Automated settlement and payout distribution
- Per-user chain logic with microchain-native performance

### **Oracle System**
- Oracle contract for delivering verified results
- Off-chain oracle worker that fetches data and submits updates
- Cross-chain messaging to notify prediction markets

### **Frontend (Vercel-ready)**
- Wallet connection
- Market creation + participation
- Trade positions
- Claim rewards

### **Smart Contract Modules**
- `market/` — Prediction market contract
- `oracle/` — Oracle system
- `oracle-worker/` — Off-chain worker to fetch real data
- `user/` — User registry and account structure
- `token/` — Simple token for trading
- `shared/` — Shared types and logic
- `frontend/` — UI for interacting with markets
- `scripts/` — Deployment scripts

---

## 🏗 Tech Stack
- **Rust + Linera SDK** (smart contracts)
- **Oracle Worker** (Rust async)
- **TypeScript + Vercel** (frontend)
- **Microchains + Cross-Chain Messaging** (Linera architecture)

---

## ▶️ Run Locally

### Setup toolchain
```bash
rustup override set nightly
rustup target add wasm32-unknown-unknown
```
Build contracts
cargo build --release --target wasm32-unknown-unknown

Start a local Linera network
`linera net up`

Deploy apps
`./scripts/deploy.sh`

📁 Project Structure
```
market/
oracle/
oracle-worker/
user/
token/
shared/
frontend/
scripts/
Cargo.toml
vercel.json
README.md
```
🔮 Vision

Building a next-generation prediction market leveraging microchains, parallel execution, and trust-minimized oracle inputs.
---

