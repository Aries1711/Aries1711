# Project Workflow — smart-contract-exercise

## Overview
Structured Solana smart contract training curriculum. One concept per exercise, hands-on, on devnet.
Arisqi writes the code with Claude guiding — not the other way around unless explicitly asked.

## Curriculum Order

### Phase 1 — Native Rust (no framework)
Goal: understand exactly what happens under the hood. Every byte, every check, written by hand.

0. Hello World (native) — entrypoint, process_instruction, msg! logging, program structure
1. Counter (native) — Borsh serialization, account state, instruction dispatch
2. Profile / access control (native) — manual signer + owner checks, break-it-first exploit
3. UserStats with PDA (native) — find_program_address, create_account via CPI, bump storage
4. SOL transfer via CPI (native) — invoke(), system_instruction::transfer
5. Vault + two-program CPI (native) — invoke_signed(), PDA signing, delegated authority
6. SPL Tokens (native) — spl-token CPI, mints, ATAs, approve/revoke
7. Token vault capstone (native) — PDAs + CPI + tokens, program-defined release condition

### Phase 2 — Anchor Framework
Same 7 exercises repeated. Goal: see exactly what Anchor generates vs. what you wrote by hand.
0–7. Mirror of Phase 1 exercises using Anchor macros, IDL, and TypeScript tests

### Exercise 8 — Security Checklist Capstone (Final)
A dedicated security audit session that synthesizes all 7 prior exercises.
- Review programs from Ex 1–7 against the complete 7-point checklist
- For each exercise: identify what checks were present, what was missing, what Anchor handles vs. what you must write manually
- Write a "deliberately broken" version of the Ex 5 vault (missing 2-3 checks), audit it, and fix it
- Score each program 0-7 on the checklist — target is 7/7 on the capstone
- Mix points: signer (Ex 2), owner (Ex 2-3), address check (Ex 3), data size (Ex 1), instruction data (Ex 1), arithmetic (Ex 1+7), state check (Ex 7)

## Task Routing
| Signal | Action |
|--------|--------|
| New exercise | brainstorming → explain concept → guide implementation step by step |
| Something broke | systematic-debugging → find root cause → fix with explanation |
| Exercise done | Security question: "what could go wrong if someone attacked this?" |
| Ready to move on | Quick comprehension check before advancing |
