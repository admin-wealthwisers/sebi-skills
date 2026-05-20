# SEBI Skills for Claude

Claude skills that encode India's SEBI regulatory frameworks as procedural
knowledge, so that Claude — and the people using Claude to build, deploy, or
audit financial systems for Indian capital markets — operate within the
regulatory perimeter by default.

**This is the first skill in a planned series.** The current release covers
SEBI's framework for retail algorithmic trading, effective 1 April 2026.
Further skills (RIA Obligations, Research Analyst Regulations, Finfluencer
Guidelines, DPDP for financial AI) are on the roadmap.

## Why this exists

Most people using AI to write, deploy, or assess trading strategies for
Indian markets don't know the operational specifics of the regulatory
framework that applies to them. The code AI generates by default isn't
framework-aware. This project addresses that gap by encoding the framework
into Claude skills that load automatically when relevant.

Compliance shifts left — from deployment review to the moment the strategy
is being designed.

## Skills in this repo

| Skill | Description | Status |
|-------|-------------|--------|
| [`algo-trading-2026`](./algo-trading-2026/) | SEBI's framework for retail algorithmic trading (effective 1 April 2026) | v0.1.0 |
| `ria-obligations` | Investment Advisor / Registered Investment Advisor obligations | Planned |
| `research-analyst-regulations` | SEBI Research Analyst regulations | Planned |
| `finfluencer-guidelines` | SEBI advertising and finfluencer rules | Planned |
| `dpdp-financial` | DPDP Act applied to financial-services AI | Planned |

## Installation

> ⚠️ Verify installation steps against current Claude Desktop documentation
> before publishing this section. Skill installation mechanics have been
> evolving and may differ from the description below.

### For Claude Desktop

1. Download the skill folder you want (e.g. `algo-trading-2026/`) from this repo.
2. Open Claude Desktop and navigate to **Settings → Skills** (or equivalent).
3. Add the skill by pointing Claude Desktop to the downloaded folder.
4. The skill will load automatically when you discuss topics in its scope.

### For Claude Code

If you use Claude Code, place the skill folder in your project's skills
directory or in your global skills folder (consult Claude Code docs for the
current location).

## Usage

Once a skill is loaded, you don't need to invoke it explicitly. Claude
will recognise when the skill's domain applies (writing trading code,
classifying strategies, deploying to Indian brokers, etc.) and load the
relevant procedural knowledge automatically.

For ad-hoc questions, just ask Claude naturally:

- "Help me write a momentum strategy for Zerodha Kite Connect"
- "Is this strategy White Box or Black Box?"
- "What do I need to do before April 1 for my algo setup?"

## License

MIT. See [LICENSE](./LICENSE).

## Not legal advice

The skills in this repo encode published regulatory guidance as procedural
knowledge. They are not legal advice and do not certify compliance with any
regulation. The authoritative sources are the SEBI and NSE circulars cited
in each skill. Consult your broker, compliance function, RA-registered
advisor, or qualified legal counsel before deployment.

## About the author

[Anjan Roy](https://anjanroy.in) — author of *Machines That Think. Systems
That Judge.* (2026), founder of WealthWisers, and Head of Data Governance
& AI at Felicitas. This project applies the EGA discipline (Evidence,
Governance, Accountability) from the book to specific Indian regulatory
contexts.

## Contributing

PRs welcome — especially from compliance officers, Research Analysts, broker
tech teams, and lawyers who can sharpen the regulatory accuracy. Issues
also welcome for edge cases the current skill doesn't handle well.

For corrections or substantive disagreements with the skill's interpretation
of any regulation, open an issue with the specific source citation you're
referencing.
