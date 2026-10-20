# irmahs-labs

Small web apps by **Irma Houver Sing**, made with care and a lot of matcha green. They all live at [irmahs.dev](https://irmahs.dev).

## Apps

| | |
|---|---|
| **[irmahs.dev](https://irmahs.dev)** | The front door: a little retro desktop in matcha greens, with windows you can drag, the weather and time in Paris or Phnom Penh, and Tokkae, a pixel gecko who lives there |
| **[What’s in my pantry?](https://pantry-spinner.irmahs.dev)** | A mobile app that decides dinner: three reels spin from what is actually in your pantry, soonest-to-expire first |
| **[Album Cover Maker](https://album-cover-maker.irmahs.dev)** | Turn a photo into an album cover and a music-player mock-up, all in the browser. Photos never leave your device |
| **[Mini Games](https://minigames.irmahs.dev)** | Small games to play in the browser, starting with a Wheel of Fortune you fill in yourself |

## How they are built

- **One look:** every app uses **Cute Matcha**, Irma's own design system, in light and dark.
- **One sign-in:** [auth](https://github.com/irmahs-labs/auth) gives every app the same Google sign-in, and keeps private apps to the people invited.
- **One front door:** [proxy](https://github.com/irmahs-labs/proxy) is the Caddy server that routes each `*.irmahs.dev` address to its app.
- **The same rules everywhere:** new repos start from [template](https://github.com/irmahs-labs/template) and share their CI through [workflows](https://github.com/irmahs-labs/workflows). Every change goes in through a pull request, with lint, type-checks, tests and a Docker build.

Built with TypeScript, React, Next.js, Vite, Hono, Postgres and Docker, with a lot of help from Claude.
