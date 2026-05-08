# Beatzy build steps

## Bootstrap
- [x] Initialize `beatzy-web` (Next.js App Router + TS + ESLint).
- [x] Create `beatzy-api` folder (Node/Express placeholder).

## UI foundation
- [ ] Add Tailwind + PostCSS config (manually; `tailwindcss init -p` currently fails).
- [ ] Replace landing page with Beatzy dark neon starter layout.

## MVP (Phase 1) implementation
- [ ] Authentication: basic user model + login UI (MVP stub if no backend yet).
- [ ] Music streaming MVP: upload placeholder + player UI + playlist UI.
- [ ] Social: like/comment + follow artist (local/mock data first).
- [ ] Search + discovery: trending + recently played + genre categories (mock).

## Phase 2: Creator economy
- [ ] Beat marketplace UI (listing, licensing tiers, earnings panel) + mock purchase flow.
- [ ] Analytics dashboard UI (mock for now).
- [ ] Reels UI (vertical cards, autoplay stub, like/comment/save stub).

## Phase 3: AI expansion
- [ ] AI music generator UI (prompt -> generation request stub).
- [ ] Remix/mastering/lyric/voice tool UIs (stubs).
- [ ] AI creator assistant chat UI (stubs).

## Infrastructure
- [ ] Backend: Express server with API routes + DB schema (Postgres) or Firebase integration.
- [ ] Storage: integrate S3/Firebase Storage placeholder.
- [ ] Streaming: HLS endpoint + CDN placeholder.

## Safety & compliance
- [ ] Copyright detection/upload policy placeholders.
- [ ] Voice impersonation prevention UI rules placeholders.

## Validation
- [ ] Run `npm run dev` and verify the UI loads.
- [ ] Add basic smoke tests (lightweight).

