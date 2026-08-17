# Project Rules — smart-contract-exercise

## Constraints
- Devnet only — never use mainnet wallet (~/.config/solana/main-wallet.json) for exercises
- All exercises are self-contained learning projects — no business requirements injected
- Break-it-first approach for every access control concept (build insecure → verify exploit → fix)

## Stack
- Rust 1.97.1 + Cargo
- Solana CLI 4.0.3 (Agave)
- Anchor 0.31.1 (via AVM 1.1.2)
- Node.js v22.2.0 / npm 10.7.0
- Network: Devnet

## Non-Negotiables
- No code before brainstorm is approved
- No fix without root cause
- No "done" claim without running verification
- After every exercise: ask "what could go wrong if someone attacked this?"
