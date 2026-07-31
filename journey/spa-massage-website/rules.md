# Project Rules — spa-massage-website

## Constraints
- Single-page landing site — anchor-link navigation only, no routing
- All booking CTAs must link to WhatsApp (wa.me)
- No git commit or push without explicit user approval
- WhatsApp number in site.ts is a personal placeholder — must swap to business number before production deploy

## Stack
- Next.js 16.2.12 (App Router, src/ directory)
- React 19.2.4 — Server Components by default, minimal 'use client'
- Tailwind CSS v4 — CSS-first config via @theme block in globals.css, no tailwind.config.js
- TypeScript strict mode, path alias @/* → ./src/*
- Fonts: Cormorant Garamond (display) + Geist Sans (body) via next/font/google

## Non-Negotiables
- No code before brainstorm is approved
- No fix without root cause
- No "done" claim without running verification
- Never commit or push without user review
