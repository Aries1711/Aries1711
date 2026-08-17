# Journey Memory — smart-contract-exercise
Started: 2026-08-13
Session Orchestrator: Claude Code (claude-sonnet)

## Index
- **2026-08-13** — Environment setup complete: Rust 1.97.1, Solana CLI 4.0.3, AVM 1.1.2, Anchor 0.31.1, Node v22.2.0, Yarn. Devnet keypair at ~/.config/solana/devnet-training.json, 2.5 SOL airdropped.
- **2026-08-13** — Curriculum expanded: Phase 1 = 8 native Rust exercises (Ex 0–7), Phase 2 = same 8 in Anchor. Exercise 8 = Security Capstone added (audit + break + fix). Schedule extended to Aug 23.
- **2026-08-17** — Ex 0 (Hello World) ✅ + Ex 1 (Counter) ✅ complete. Key lessons: platform-tools mismatch (fixed via agave-install v4.0.3), data_is_empty() vs is_initialized bool pattern, checked_add for overflow safety. Security checklist items covered: signer check, owner check, re-initialization guard, arithmetic overflow.
