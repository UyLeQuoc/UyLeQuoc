# Le Quoc Uy

**Full-stack engineer · LLM & AI agents · Sui & Walrus**

I'm a Full-Stack Engineer at CommandOSS (Mysten Labs Vietnam) in Ho Chi Minh City. I build LLM and AI-agent products end to end: MCP servers and plugins, agent memory, tool-calling agents, and the tests and evals that check them.

[LinkedIn](https://www.linkedin.com/in/uydev) · [Portfolio](https://uydev.vercel.app) · [lequocuyit@gmail.com](mailto:lequocuyit@gmail.com)

## At CommandOSS

- **[MillionTPS](https://www.sui.io/blog/sui-processes-over-6-million-transactions-per-second-in-ai-agent-livestream-experiment)**: the public app for Sui Tunnels' throughput runs: 40.6M TPS at Sui Basecamp 2026 ([verified by CertiK](https://www.certik.com/blog/certik-independently-verifies-suis-new-performance-benchmark)) and 6.09M TPS at the July livestream. I was the largest frontend contributor to the July version (Google sign-in with sponsored gas, a Web Worker tunnel engine).
- **[Walrus Memory](https://github.com/MystenLabs/walrus-memory)** (open source): rewrote the MCP tools so agents save and recall memory on their own, and built the automatic-memory plugin for Claude Code, Codex, Cursor and Antigravity.
- **Dopamint Arena**: LLM agents play poker on Sui. Top committer to the web app: cut 3D GPU memory from 415 to 150 MB and built the Open league that outside agents join on their own.
- **AI Video Maker**: Claude Code turns a code repo into a product video. I built the video engine, the agent review loop and a Rust renderer 3.2× faster than Chromium.
- **[cmdocs](https://cmdocs.sh)** (first engineer) and **[wal-0](https://wal-0.commandoss.com)** (pay-per-prompt billing), both deploying to Walrus.

Company repos are private, so the links above go to public pages.

## Side project

- **[walrus-docs-rag](https://github.com/UyLeQuoc/walrus-docs-rag)** (Python, FastAPI): question answering over the Walrus docs with hybrid retrieval (BM25 + embeddings, fused with RRF) and cited answers. An eval set of 82 labelled questions gates CI. Hybrid retrieval reaches 0.95 recall@5, and on 17 paraphrased questions 0.76 vs 0.53 for BM25 alone.

## Hackathons

| Project | What it is | Result |
| --- | --- | --- |
| [WalForm](https://github.com/UyLeQuoc/sui-walform) | Encrypted form builder on Sui mainnet. It became the entry form for Walrus Sessions 3–8. | 1st, Walrus Session 2 |
| [Continuum v2](https://github.com/UyLeQuoc/walrus-session-7) | A privacy-safe, deterministic memory prompt on Walrus. | 1st, Walrus Session 7 |
| [hippo](https://github.com/UyLeQuoc/walrus-session-8-chatbots) | A chatbot with user-owned memory on Walrus. Cut median first-reply recall from 3.76 s to 1.97 s. | 2nd, Walrus Session 8 |
| [Remora](https://github.com/UyLeQuoc/walrus-session-10-remora) | An agent whose spending limit is enforced on Sui. A 28-case red-team eval runs in CI with 0 overspends. | Walrus × Tatum Total Recall |
| [Flicky](https://github.com/nikola0x0/flicky) | PvP prediction duels on DeepBook (team of 3, I did most of the backend). | 4th, DeepBook track, Sui Overflow 2026 |

Also 1st place in Walrus Session 1 (my portfolio as a Walrus Site) and Session 9 (RedSentinel red-teaming).

## How I work

I write the spec first, build with Claude Code under repo rules I write (AGENTS.md, skills), and ship each change with tests, CI and a measured before/after. Where an LLM makes the decision, an eval suite gates the merge.

**Stack:** TypeScript, React, Next.js, Node.js / Bun, Hono, PostgreSQL, Rust, Python (FastAPI), Vercel AI SDK, OpenRouter, MCP, Claude Code, Sui, Walrus.
