# Galin Ganchev

**Full-Stack AI Engineer · Blockchain & Fintech** · 6 years in software, 4 in Web3 · TypeScript, NestJS, Solidity · LLM products & coding agents · ex-Coinbase contractor · Sofia, Bulgaria (remote worldwide, or on-site/hybrid in Sofia)

I build systems that move money and the AI that works on them: event-driven services that stay correct under failure, smart contracts designed and tested against known attack classes, and LLM features backed by evals and guardrails. Open to senior full-stack AI, backend, blockchain and smart-contract security roles.

## Selected work

- **[LimeForge](https://limechain.tech/limeforge)** (LimeChain's client-facing AI platform that turns Web3 ideas into build-ready specs): contributed during the research phase.
  - Researched GraphRAG and LightRAG for the Web3 knowledge layer and documented the retrieval, guardrail and eval design.
  - Contributed to the eval and regression harness, IP-protection guardrails (output scanner, probing detection) and prompt caching, which cut the cost per request ~10×.
- **[preaudit](https://github.com/realgalinganchev/preaudit)** (open source): a pre-audit pipeline for Foundry projects that runs Slither, fuzz and invariant tests, Medusa, Halmos and Gambit and merges them into one report. On Cyfrin's PuppyRaffle benchmark, with a purpose-written harness, it finds all nine known bugs. Claude Code GitHub Actions with Pashov's AI-audit skills review every PR.
- **Coinbase** (contractor via LimeChain, Feb 2025 – Jun 2026), working directly under the Head of Tokenization:
  - Built and presented an EVM indexer proof of concept: chain-reorg handling and a dual-queue RabbitMQ topology separating historical and live event streams, with rate-limited RPC access.
  - Built the Forward Flow Agreement fund contracts on top of MetaMorpho (ERC-4626) vaults, and closed a yield-theft vulnerability before deployment.
  - Delivered full-stack features end to end for tokenized-securities tooling (reconciliation history, token-holder lists): gRPC backend, frontend views, released through multi-round review.
  - Built a tokenized-loan marketplace backend: versioned REST APIs with JWT auth, idempotency keys and transactional DB locks for retry-safe writes, PostgreSQL, Kubernetes, Terraform, CI/CD.
- **Institutional credit vault on Rayls**: a Morpho Blue-style lending market with an ERC-4626 vault, NAV-priced collateral, permissionless liquidation and bad-debt socialization. Verified with stateful invariant fuzzing, 100% branch coverage and mutation testing. [Verified contract ↗](https://testnet-explorer.rayls.com/address/0x105e0d578377594b892c9d7b43d56b43a707a8c8)
- **MetaWin prediction markets**: wrote, deployed and verified the ERC-1155 conditional-token and CTF exchange contracts, with UMA oracle resolution.
- **[blockchain101](https://github.com/realgalinganchev/blockchain101)** · **[live demo ↗](https://blockchain101.founderexchange.co)**: a from-scratch proof-of-work chain mirroring pre-Merge Ethereum (Keccak-256, RLP, nonce mining), TypeScript, Node.js and React. Live on AWS: EC2 provisioned with Terraform, automatic HTTPS, GitHub Actions deploying through OIDC and SSM (no SSH, no stored keys), and API hardening for public traffic. Built with AI coding agents.

## Stack

- **Backend:** TypeScript, Node.js, NestJS, PostgreSQL, MongoDB, Redis, REST, GraphQL, gRPC
- **Event-driven:** Kafka, RabbitMQ, Temporal, BullMQ
- **Blockchain:** Solidity, Foundry (invariant & fuzz testing), ERC-4626 / 1155 / 20, Morpho, ethers.js, viem, The Graph, Solana (Metaplex)
- **Infra:** AWS, Terraform, Docker, Kubernetes, GitHub Actions
- **AI engineering:** RAG / GraphRAG, eval & regression harnesses, guardrails, prompt caching
- **AI tooling:** Claude Code (custom skills, hooks, subagents), MCP servers, Codex, Gemini, OpenRouter, AI code review
- **Security:** smart contract audits & security research, Slither, Halmos, Medusa / Echidna, Gambit mutation testing
- **Also:** Go, React / Next.js · Languages: Bulgarian, English, German

## How I work

Agent-first but careful: I direct Claude Code from the terminal every day with my own skills, hooks, MCP servers and subagents, plan before implementing, and let specs and tests decide what ships. An AI review pass runs on every PR, and AI-assisted code ships only after tests and human review. I completed Snyk's AI Security Training (secure AI-assisted coding, AI red teaming). I write things down (ADRs, runbooks, design docs), which keeps distributed teams aligned.

## Contact

📫 galin.ganchev11@gmail.com · [LinkedIn](https://linkedin.com/in/realgalinganchev)

<details>
<summary>The fun version 🖥️</summary>

```
 __________________________________________________________________________________________________
/                                                                                                  \
|   ____________________________________________________________________________________________ |
|  | MINGW64:/c/users/galin/repos/life                                                          | |
|  |                                                                                            | |
|  | Galin@GalinGanchev MINGW64 c/users/galin                                                   | |
|  | $ git config --global alias.lg 'log --oneline --color --decorate --graph --branches'       | |
|  |                                                                                            | |
|  | Galin@GalinGanchev MINGW64 c/users/galin                                                   | |
|  | $ cd ./repos/life/about-me                                                                 | |
|  |                                                                                            | |
|  | Galin@GalinGanchev MINGW64 c/users/galin/repos/life/about-me (master)                      | |
|  | $ git lg                                                                                   | |
|  | * a1b2c3d Merge branch 'galin' into master                                                 | |
|  | |\                                                                                         | |
|  | | * f9e8d7c (galin, origin/galin) See you on the flipside                                  | |
|  | |                                                                                          | |
|  | | * 7c6b5a4 Merge branch 'galin/interests' into galin                                      | |
|  | | |\ 3d2e1f0 (galin/interests, origin/galin/interests) reading                             | |
|  | | | * 9a8b7c6 reading about smart contract security                                        | |
|  | | | * 5e4d3c2 playing chess                                                                | |
|  | | |/                                                                                       | |
|  | | * b7a6c5d Merge branch 'galin/tech' into galin                                           | |
|  | | |\ e4d3c2b (galin/tech, origin/galin/tech) AWS + Terraform + Docker + Kubernetes         | |
|  | | | * 0b1c2d3 Claude Code + MCP + skills + hooks + subagents                               | |
|  | | | * 1d2e3f4 GraphRAG research for LimeForge                                              | |
|  | | | * c1b0a9f Kafka + RabbitMQ                                                             | |
|  | | | * a8f7e6d NestJS + Next.js + React                                                     | |
|  | | | * 9d8c7b6 Foundry / Anvil + Hardhat + ethers.js + viem                                 | |
|  | | | * 6b5a4f3 Go                                                                           | |
|  | | | * 4f3e2d1 TypeScript                                                                   | |
|  | | | * 2c1b0a9 Solidity                                                                     | |
|  | | |/                                                                                       | |
|  | * d5c4b3a Owned ERC-1155 conditional-token contracts for MetaWin's                         | |
|  |           prediction-market platform (separate LimeChain engagement)                       | |
|  | * a2b1c0d Former Senior Blockchain Developer at LimeChain, embedded with                   | |
|  |           Coinbase as a contractor -- open to new opportunities now                        | |
|  | * f0e9d8c My name is Galin Ganchev                                                         | |
|  | /                                                                                          | |
|  | * 0942ca8 Initial commit                                                                   | |
|  |                                                                                            | |
|  | Galin@GalinGanchev MINGW64 c/users/galin/repos/life/about-me (master)                      | |
|  | $                                                                                          | |
|  |____________________________________________________________________________________________| |
|____________________________________________________________________________________________________|
 \__________________________________________________________________________________________________/
        . -------------------------------------------------------------------.
        | [Esc] [F1][F2][F3][F4][F5][F6][F7][F8][F9][F0][F10][F11][F12] o o o|
        |                                                                    |
        | [`][1][2][3][4][5][6][7][8][9][0][-][=][_<_] [I][H][U] [N][/][*][-]|
        | [|-][Q][W][E][R][T][Y][U][I][O][P][{][}] | | [D][E][D] [7][8][9]|+||
        | [CAP][A][S][D][F][G][H][J][K][L][;]['][#]|_|           [4][5][6]|_||
        | [^][\][Z][X][C][V][B][N][M][,][.][/] [__^__]    [^]    [1][2][3]| ||
        | [c]   [a][________________________][a]   [c] [<][V][>] [ 0  ][.]|_||
        `--------------------------------------------------------------------'
```

</details>
