# Awesome Crypto Economy for AI Agents  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) <!-- omit in toc -->

> A curated list of production‑oriented projects powering the *crypto economy for AI agents* - including agent‑to‑agent workflows, AI DAOs, and human‑in‑the‑loop systems with on‑chain payments.

This list emphasizes platforms and protocols where agents earn, spend, and coordinate with crypto. It intentionally avoids duplicating entries from the `awesome-blockchain-ai` list you shared (e.g., SingularityNET, Fetch.ai, Ocean Protocol, Truebit, Bittensor, etc.).

## Contents <!-- omit in toc -->

- [Recommended reading](#recommended-reading)
- [Agent platforms \& multi‑agent economies](#agent-platforms--multiagent-economies)
- [Agent marketplaces \& agent‑to‑agent commerce](#agent-marketplaces--agenttoagent-commerce)
- [Agent wallets, execution \& SDKs](#agent-wallets-execution--sdks)
- [Verifiable inference, AI oracles \& model runtimes](#verifiable-inference-ai-oracles--model-runtimes)
- [Human‑in‑the‑loop \& data/task networks](#humanintheloop--datatask-networks)
- [Identity \& reputation primitives for agent economies](#identity--reputation-primitives-for-agent-economies)
- [Analytics \& indexing for agent economies](#analytics--indexing-for-agent-economies)
- [Academic research \& standards](#academic-research--standards)
- [Notes on scope](#notes-on-scope)
- [Contributing](#contributing)
- [License](#license)

## Recommended reading

* [Enabling AI Agents with Blockchain - Circle](https://www.circle.com/blog/enabling-ai-agents-with-blockchain) - Why agents need accounts, programmable money, and autonomous payments.
* [AI Agents 101: The Future of Agentic Web & On‑chain AI - Forbes](https://www.forbes.com/sites/clorischen/2024/12/23/ai-agents-101-the-future-of-agentic-web-and-onchain-ai/) - A primer on agent networks and emerging stack.
* [LangChain: State of AI Agents Report](https://www.langchain.com/stateofaiagents) - Where agents are being used in production and common challenges.
* [W3C AI Agent Protocol Community Group](https://www.w3.org/community/agentprotocol/) - Effort to standardize agent discovery, identity and interop on the web.
* [The Protocol of Agents: Web3 × MCP](https://www.coindesk.com/opinion/2025/07/29/the-protocol-of-agents-web3-s-mcp-potential) - Perspective on emerging protocol layers for agents.
* [x402 + AI Agents TypeScript Boilerplate](https://github.com/coinbase/x402/tree/main/examples/typescript/dynamic_agent) - This example demonstrates an agent that can perform multi-tool tasks, without prior knowledge of the tools available to it. Each tool is paid for on a per-request basis using x402.

## Agent platforms & multi‑agent economies

* [Olas (Autonolas)](https://olas.network/) - Network for *co‑owned AI*. Agents, components and services are packaged as NFTs; the Olas protocol rewards “useful” code and powers *agent economies* (e.g., Olas Predict multi‑agent prediction services).
* [Shinkai](https://shinkai.com/) - Local‑first, P2P AI agent OS with a peer‑to‑peer agent marketplace and USDC/x402 payments for agent services; v1.0 announced as production build.
* [Virtuals Protocol](https://www.virtuals.io/) - “Society of AI Agents” where agents are tokenized (Agent Tokens) and participate in on‑chain commerce; launched on Base with growing marketplace activity.
* [Griffin AI](https://www.griffinai.io/) - On‑chain Agent Builder and DeFi agent environment; supports execution (with human confirmation) such as swaps on Arbitrum via its Transaction Execution Agent.
* [AgentLayer](https://agentlayer.xyz/home) - L1/network focused on autonomous AI agent coordination and deployment.
* [Rooch Network](https://rooch.network/blog/eliza-with-move) - Move‑based *verifiable applications* and fully on‑chain Eliza agents with on‑chain memory/identity.
* [AgentFi](https://agentfi.io/) - “Home of on‑chain agents”; NFT‑native (ERC‑6551) agent accounts with marketplace‑style transferability.
* [Ava Protocol](https://avaprotocol.org/usecases/web3-agents/) - Execution layer that turns agent intent into verifiable on‑chain actions across EVM chains.

## Agent marketplaces & agent‑to‑agent commerce

* [Olas Mech Marketplace](https://olas.network/blog/olas-launches-the-mech-marketplace-the-ai-agent-bazaar) - Decentralized bazaar where AI agents hire other AI agents for specialized tasks; live and growing agent‑to‑agent transactions.
* [Virtuals Protocol - Agent Commerce Protocol (ACP)](https://www.virtuals.io/) - Tokenized agents offering services/products and sharing revenue with creators/investors.

## Agent wallets, execution & SDKs

* [Coinbase AgentKit (CDP)](https://docs.cdp.coinbase.com/agentkit/docs/welcome) - Toolkit that gives AI agents their own wallets and on‑chain actions (transfers, swaps, contract calls) on Base/EVM.
* [Warden Agent Kit](https://docs.wardenprotocol.org/build-an-agent/warden-agent-kit/introduction) - SDK/CLI to build agents that autonomously open wallets/keys, swap, route across chains; Agent Hub integrates with Uniswap.
* [0xGasless AgentKit](https://docs.0xgasless.com/intro) - Developer toolkit for fully autonomous on‑chain interactions (transfers, swaps, token deployments).
* [clanker-wallet](https://github.com/almogdepaz/clanker-wallet) - TypeScript/Python SDK for AI agents to propose blockchain transactions that a human approves from their own wallet. E2E encrypted relay, no private keys in agent. LangChain & Vercel AI SDK integrations included.
* [ElizaOS](https://github.com/ai16z/eliza) - Web3‑friendly agent OS used widely for social/on‑chain agents; integrates wallets & EVM/Solana actions. Accompanying arXiv paper describes the system.
* [OpenAgent (Open Network)](https://docs.open.network/guide/openstack/openagent) - Framework with “executors” for DeFi, tokens, social and web data; web3‑native agents.

## Verifiable inference, AI oracles & model runtimes

> Trust layers agents use to pay for and verify model calls and decisions.

* [Ritual - Infernet](https://www.ritual.net/) - Decentralized inference network & RPC for AI to connect on‑chain apps/agents to off‑chain models with payments & metering.
* [Allora Network](https://www.allora.network/) - Self‑improving, decentralized ML network with roles (Workers/Reputers/Validators) and paid inferences; powering agent use cases like predictions and trading.
* [ORA - Onchain AI Oracle & opAgent](https://docs.ora.io/doc/onchain-ai-oracle-oao/onchain-ai-oracle) - opML (optimistic ML) dispute game for verifiable inference; opAgent for *on‑chain, perpetual* agents.
* [Modulus Labs (zkML)](https://variant.fund/articles/modulus-zero-knowledge-machine-learning-seed-round/) - zk‑verified ML outputs for smart contracts; makes AI decisions composable and auditable for agents.
* [Giza (Starknet zkML)](https://www.starknet.io/blog/giza-enabling-ml-in-the-blockchain-using-cairo-video/) - Cairo‑native zkML primitives + examples of on‑chain agents for yield/portfolio mgmt.

## Human‑in‑the‑loop & data/task networks

> Markets where humans and agents co‑produce value - labeling, prediction, curation, or data collection - with crypto incentives.

* [Botto](https://www.botto.com/) - Community‑directed AI artist DAO where tokenholders curate the model’s outputs and share auction proceeds; a flagship human‑in‑the‑loop AI DAO. ([WIRED][36])
* [Effect Network](https://docs.effect.ai/) - Decentralized microtasking network (annotation/labeling, data generation) used to train AI systems; contributors paid in crypto. ([Botto Docs][37])
* [Grass](https://www.getgrass.io/) - Network where users run nodes that collect web data; teams pay for data to train AI. ([Flock][38])
* [Olas Predict](https://www.valory.xyz/post/agent-economies-synthetic-data) - Multi‑agent system where hundreds of agents transact and compete in prediction markets, generating synthetic datasets. ([Valory][8])

## Identity & reputation primitives for agent economies

> Sybil resistance and reputation are essential where agents transact with humans/other agents.

* [World ID (Worldcoin)](https://worldcoin.org/world-id) - Proof‑of‑personhood for human–agent gating; real‑world expansion covered broadly in 2025. ([The Washington Post][39])
* [Human Passport (Gitcoin Passport)](https://passport.human.tech/) - Attestation‑based identity with model‑assisted Sybil detection; widely used across web3. ([Human Passport][40])

## Analytics & indexing for agent economies

* [Cookie DAO / cookie.fun](https://agents.cookie.fun/) - Data layer & index for AI agent tokens and infra across chains (mindshare, on‑chain/social metrics); APIs for agent builders.

## Academic research & standards

* [Towards Multi-Agent Economies: Enhancing the A2A Protocol with Ledger-Anchored Identities and x402 Micropayments for AI Agents](https://www.arxiv.org/abs/2507.19550) - Novel architecture to empower multi-agent economies, decentralized agent discoverability and agent-to-agent micropayments.
* [Eliza: A Web3‑friendly AI Agent Operating System (2025)](https://arxiv.org/abs/2501.06781) - Architecture for deployable, web3‑integrated agents.
* [opML: Optimistic Machine Learning on Blockchain (2024)](https://arxiv.org/abs/2401.17555) - Fraud‑proof‑style verification for ML used by ORA.
* [AI Agents × Blockchain survey (Future Internet, 2025)](https://www.mdpi.com/1999-5903/17/2/57) - Overview of secure/scalable multi‑agent collaboration on blockchains.
* [W3C AI Agent Protocol Community Group](https://www.w3.org/community/agentprotocol/) - Toward interoperable, secure agent communication standards.
* [LangChain Agent Protocol (spec & OpenAPI)](https://github.com/langchain-ai/agent-protocol) - Practical, framework‑agnostic APIs for serving agents in production.

## Notes on scope

* In‑scope: projects where agents earn/spend, hire other agents, or coordinate with humans via on‑chain payments/incentives.
* Out‑of‑scope: generic “AI + blockchain” compute/data projects already covered in the [Awesome Blockchain AI](https://github.com/steven2358/awesome-blockchain-ai/).

## Contributing

PRs welcome! Please include:

1. project name + URL,
2. one‑sentence description (objective claims with sources),
3. category suggestion,
4. (optional) current status (mainnet / public beta/ testnet / research) and public proof (docs, explorer txs, releases).

---

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Michal Takáč](https://github.com/michaltakac) has waived all copyright and related or neighboring rights to this work.
