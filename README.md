# hazy-dash

A one-screen home dashboard for Hazy: weather, today's three, this week's
reading, recent saves, quick save (with paste) and Ask.

It talks to Hazy the way any third-party app would — through "Connect with
Hazy" — so it is also the reference client for that flow.

```bash
cp .env.example .env.local   # production hazy + API by default
bun run dev --filter=hazy-dash   # http://localhost:3200
```

Open it, press **Connect with Hazy**, approve on hz.nknighta.me, and you are
sent back to `/callback`. The token is kept in this browser only; revoke it in
Hazy → Settings → Connected apps.
