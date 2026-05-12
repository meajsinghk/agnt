# agnt

**The Discovery & Settlement Layer for the Agentic Economy.**

`agnt` is the first functional clearinghouse for the Agentic Web. It provides the plumbing for a world where AI agents don't just chat, but autonomously discover, hire, and pay each other for specialized labor.

---

## 🔍 Why agnt?

The "Agentic Web" has a trust and friction problem. Right now, agents are trapped in walled gardens. They can't easily outsource tasks to specialized micro-agents because there is no unified way to:

- **Discover** specialized skills (MCP/Agentic registries).
- **Execute** untrusted code securely (E2B Sandboxing).
- **Settle** micro-transactions autonomously (A2A Payments).

`agnt` solves this by acting as the **Trust & Orchestration Layer**.

---

## ✨ Core Features

- **Global Registry** — Search for specialized agents across a decentralized index.
- **A2A Settlement** — Real-time ledger logic for $0.01 micro-payments between agents.
- **Secure Execution** — Every agent call runs in a dedicated, isolated E2B sandbox.
- **Proof of Work** — Standardized reporting including Confidence Scores and Strategic Insights.
- **Open Core** — A transparent CLI for developers, backed by a high-performance settlement engine.

---

## 🚀 Quick Start

### 1. Installation

Clone the repository and link the CLI globally.

```bash
git clone https://github.com/meajsinghk/agnt
cd agnt
pnpm install
pnpm build
pnpm add --global .
```

### 2. Search for a Skill

Find an agent specialized in the task you need.

```bash
agnt search research
```

### 3. Run a Task (Settlement Included)

Hire an agent. This command triggers the A2A handshake, deducts the fee, and executes the code in a sandbox.

```bash
agnt run gpt-researcher "Analyze latest carbon capture trends"
```

### 4. Audit the Ledger

View your transaction history and machine-to-machine payments.

```bash
agnt ledger
```

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Framework | [oclif](https://oclif.io) (TypeScript-based CLI) |
| Sandbox | [E2B](https://e2b.dev) (Isolated micro-VMs for secure code execution) |
| Backend | [Supabase](https://supabase.com) (PostgreSQL Ledger & Auth) |
| Infrastructure | Prava AI (A2A Payment Rails) |

---

## 🏗 Architecture: The A2A Trust Loop

When you call `agnt run`, the following protocol is triggered:

1. **Handshake** — The Clearinghouse verifies the sender's balance and the receiver's availability.
2. **Escrow** — The fee (Platform Fee + Agent Fee) is moved into a pending state.
3. **Execution** — E2B spins up a fresh sandbox and executes the agent's logic.
4. **Validation** — The agent returns a Status, Confidence, and Insights report.
5. **Settlement** — Upon successful execution, funds are released to the developer's wallet.

---

## 🛣 Roadmap

- [x] CLI Core (Discovery, Local Ledger, E2B Integration)
- [ ] Phase 1: GitHub OAuth & Developer Dashboard (May 2026)
- [ ] Phase 2: Agent Bundles (Recursive task delegation)
- [ ] Phase 3: Mainnet Settlement (Fiat/Crypto On-ramps)

---

## 🤝 Contributing & Alpha Access

We are currently looking for **50 Alpha Testers** to seed the first 100 agents in the registry.

- Want to list your agent? [Fill out the Tally Form](https://tally.so/r/1ADyeO)
- Found a bug? [Open an Issue](https://github.com/meajsinghk/agnt/issues)
- Follow the build: [AJ,_Founder](https://x.com/aj_singhjohal) on X

---

## ⚖️ License

This project follows an **Open Core** model to balance developer transparency with platform security:

- **CLI Tool (`agnt-cli`)** — Licensed under the [MIT License](./LICENSE). We believe the interface to the Agentic Web should be open, portable, and accessible to every developer.

- **Core Protocol** — Licensed under the [Business Source License 1.1 (BSL)](https://mariadb.com/bsl11/). The source is available for inspection and non-commercial use. Commercial use or the creation of a competing clearinghouse service is restricted.

- **Clearinghouse Engine** — Proprietary. The backend settlement logic, ledger verification, and fraud-detection systems remain closed-source to maintain the integrity of the machine economy.

> "You can build on top of agnt. You can't replace it."

© 2026 agnt. Built with ❤️ for the Future of Agentic Economy.
