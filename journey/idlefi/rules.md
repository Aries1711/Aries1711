# Project Rules — idlefi

## Stack
- Backend: NestJS (TypeScript) — `backend/src/`
- Frontend: Flutter (Dart) — `frontend/app-platform/lib/`
- Multi-platform: iOS (Swift), Windows (C++), Android (Kotlin/Java)
- Auth: email register/login, confirm, forgot/reset password, JWT refresh
- Storage: S3 uploader (`backend/src/files/infrastructure/uploader/s3/`)
- DB: Relational ORM with mapper pattern (`toDomain` / `toPersistence`)

## Constraints
(filled after brainstorming — tech constraints, architecture decisions, no-go zones)

## Non-Negotiables
- No code before brainstorm is approved
- No fix without root cause
- No "done" claim without running verification
