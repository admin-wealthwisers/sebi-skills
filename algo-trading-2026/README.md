# SEBI Algo Trading 2026

A Claude skill that operationalises India's SEBI framework for retail
algorithmic trading (effective 1 April 2026) into a procedural knowledge
layer Claude can use when helping users write, deploy, or evaluate trading
strategies in Indian capital markets.

## What this skill does

When loaded into Claude, this skill ensures that conversations about
Indian algo trading are framework-aware. Claude will:

- Classify strategies as White Box, Black Box, or Ambiguous, with reasoning
- Surface OPS thresholds, static IP, OAuth, 2FA, and daily-logout requirements
- Flag market order conversion to MPP for strategies that depend on it
- Apply the family-only distribution rule
- Enforce Indian server hosting requirements
- Generate compliance-aware code when asked to write trading scripts

## Sources

- SEBI Circular SEBI/HO/MIRSD/MIRSD-PoD/P/2025/0000013, dated 4 February 2025
- NSE Circular NSE/INVG/67858, dated 5 May 2025
- Plus subsequent NSE/BSE corrigenda

See `references/sources.md` for full citations and links.

## Installation

See the top-level [repo README](../README.md) for installation instructions.

## Not legal advice

This skill is a starting point for governance design. It is not legal advice
and does not certify compliance with any regulation. The SEBI and NSE
circulars cited are the authoritative sources. Consult your broker,
compliance function, an RA-registered advisor, or qualified legal counsel
before deployment.

## Version

v0.1.0 — Initial release, May 2026.
