# Beatzy — Brainstorm Plan (MVP → Phases)

## 0) Current repo status (facts)
- `beatzy-web/` exists (Next.js App Router + TS + ESLint).
- Tailwind packages are present, but `tailwind.config.*` and `postcss.config.*` are missing.
- Current UI is default scaffold (not Beatzy-branded).

## 1) Bootstrap / Brand foundation
### Goal
Make the app feel premium, futuristic, neon + glassmorphism.

### Tasks (frontend)
- Add Tailwind + PostCSS config manually:
  - `beatzy-web/tailwind.config.js`
  - `beatzy-web/postcss.config.js`
- Replace `beatzy-web/app/page.tsx` + styling with Beatzy landing UI.
- Update `beatzy-web/app/globals.css` to include Tailwind base/components/utilities + neon theme variables.
- Add core layout components:
  - `TopNav`
  - `NeonSidebar` (optional for desktop)
  - `NowPlayingBar` (sticky)
  - `NeonCard`, `GlassPanel`, `WaveformViz` (UI-only placeholders)

## 2) Phase 1 — MVP (streaming + playlists + social)
### Features
- Accounts (stub UI if backend not ready)
- Music upload (stub/placeholder)
- Music streaming UI
- Playlists
- Like/comment
- Follow artists
- Artist profiles

### UI pages/routes (suggested)
- `/` Home (Trending + Recently played + Recommended)
- `/discover` (genres, search, mood/daypart AI playlists placeholder)
- `/artist/[id]`
- `/track/[id]` (player + comments)
- `/playlist/[id]`
- `/library` (liked + playlists)

### Data approach (initial)
- Mock JSON data + in-memory state.
- Later swap to backend.

## 3) Phase 2 — Creator economy
### Features
- Beat marketplace UI
- Beat licensing tiers UI
- Producer verification badge UI
- Trending rankings + analytics panel UI (mock)

### Pages/routes
- `/marketplace` (listings + filters)
- `/beat/[id]`
- `/earnings` (creator earnings panel)
- `/analytics` (dashboard)

### Data approach
- Mock marketplace items + mock purchase modal.

## 4) Phase 2/early Phase 3 — Reels
### Features
- Vertical reels feed
- Infinite scroll stub
- Like/comment/save stub
- Auto-play stub
- “Use sound” modal stub

### Pages/routes
- `/reels`

## 5) Phase 3 — AI expansion
### Features
- AI music generator UI (prompt → preview)
- AI remixing/mastering/lyrics/voice conversion UIs (stubs)
- Export/download UI stubs (MP3/WAV + stems)
- AI assistant chat UI

### Pages/routes
- `/ai/generate`
- `/ai/tools` (remix/mastering/etc)
- `/ai/assistant`

### Backend integration placeholders
- A generation job endpoint contract (later):
  - `POST /api/ai/generate`
  - `GET /api/ai/jobs/:id`

## 6) Phase 4 — Global ecosystem
### Features
- Concert ticketing UI stub
- NFTs/music collectibles UI stub
- Creator agencies + education UI stub
- Label partnership UI stub

## 7) Backend + Infrastructure (architecture notes)
### Backend
- Node.js + Express REST API.
- Auth later via Firebase Auth (or OAuth) but MVP can be mock.

### Streaming
- HLS output pipeline placeholder.
- Caching + CDN placeholder.

### Storage
- S3 or Firebase Storage placeholder.

### Database
- PostgreSQL schema plan OR Firebase collections plan.

### Safety & copyright
- Upload metadata + scanning hooks placeholders.
- Voice impersonation prevention policy & UI placeholders.

## 8) Monetization (UI first)
- Subscription plans UI stub
- AI credits meter UI stub
- Marketplace commission panel UI stub
- Ads and sponsorship placeholders

## 9) Validation / testing
- Run `npm run dev` and verify landing route.
- Add basic UI smoke checks.
- Ensure responsive behavior (mobile-first).

