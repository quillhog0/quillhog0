<div align="center">
  <img src="quillhog_banner_orange.svg?v=4" alt="Quillhog">
</div>

**I build trading and on-chain tools, and the guardrails that let AI agents work on them without wrecking anything.**

QA background. That's why the agents here get red tests and hard stops, not vibes.

---

## What I build

| Project | What it is | Status |
|---|---|---|
| **[Claime](https://github.com/quillhog0/claime)** | Non-custodial Solana rent reclaimer. It closes empty SPL / Token-2022 accounts and builds unsigned transactions that the user signs in their own wallet. The server never touches keys. 0% protocol fee. | Live at [quillhog.xyz](https://quillhog.xyz) · Python |
| **[safe-agent-kit](https://github.com/quillhog0/safe-agent-kit)** | Drop-in `AGENTS.md` role templates for AI coding agents. Covers DRY_RUN by default, keeping secrets untouchable, no irreversible actions without a human yes, and `file:line` evidence for every claim. | Public · MIT |
| **Record** | Zero-disk deterministic Solana transaction export (30, 90 or 365 days) as a sealed ZIP with a full ledger CSV. | Pay by USDC |
| **Till** | Non-custodial POS payment rail that settles on-chain. | Next |
| **Trading Machine** | A Python multi-agent trading bot for XAU/USD over cTrader FIX, with a risk guardian, broker sync, reconciliation and journaling. | Private · demo/prop environments |
| **Trading Machine L8** | A rebuild of the bot as a modular, white-label framework: uv monorepo, `mypy --strict`, ruff, pytest coverage gates, CCXT / cTrader / paper adapters and notifiers. Paper mode is the default. | In progress · private |

> No profit or win-rate claims here, ever. This is infrastructure, not a signal service.

## How I work

- **Agent orchestration.** Several AI agents run with fixed roles: a librarian/docs agent, project managers and implementers. Each role has its own rules and its own report format.
- **Guardrails first.** DRY_RUN is the default, nothing goes live without an explicit flag plus confirmation, and agents never read `.env`, keys or state.
- **Branch → PR → review.** Agents don't push to main, don't publish, and don't delete; they archive. Architecture decisions go into ADRs.
- **QA mindset.** Golden tests before any refactor of risk logic. Green tests, ruff and mypy at the end of every phase. A failing test never gets skipped.

## Stack

`Python` · `uv` · `pytest` · `mypy` · `ruff` · `cTrader FIX / Open API` · `CCXT` · `Solana` · `Jupiter` · `Cursor / Claude Code / Codex / Gemini CLI` · `Linux` · `git`

## Contact

- X: [@Quillhog0](https://x.com/Quillhog0)
- Web: [quillhog.xyz](https://quillhog.xyz)
