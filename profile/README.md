# irmahs-labs

Small web apps by **Irma Houver Sing**, made with care and a lot of matcha green. They all live at [irmahs.dev](https://irmahs.dev).

## Apps

| | |
|---|---|
| **[irmahs.dev](https://irmahs.dev)** | The front door: a little retro desktop in matcha greens, with windows you can drag, the weather and time in Paris or Phnom Penh, a festival calendar or what Irma is playing on Spotify, a chat bot you can ask about her, and Tokkae, a pixel gecko who lives there |
| **[Realms](https://realms.irmahs.dev)** | Worlds to step into: the **Book of Shadows**, a witch's book with your birth chart, numerology, moons, sabbats, tarot, Potion Brewing and Spell Creator, and the **Court of Draconia**, where you become a half-dragon draconoid and team up with others for duo ultimates |
| **[Tools](https://tools.irmahs.dev)** | Handy little makers: **Album Cover Maker** turns a photo into a 3000 × 3000 cover and a music-player mock-up, and **Character Maker** builds a level 1 fifth-edition character with a sheet to print. Both run in the browser, and photos never leave your device |
| **[Mini Games](https://minigames.irmahs.dev)** | Small games to play in the browser: a Wheel of Fortune you fill in yourself, Super Tic-Tac-Toe and Ouk Chaktrang (Cambodian chess), online against others with leaderboards, a Magic 8 Ball, and personality quizzes whose results follow your account to Realms |
| **[Irma in Paris](https://irma-in-paris.irmahs.dev)** | Paris right now: the weather and air, the next metro, RER, tram or bus, Vélib' bikes, and the restaurants Irma has eaten at, on a map |
| **[What’s in my pantry?](https://pantry-spinner.irmahs.dev)** | A mobile app that decides dinner: three reels spin from what is actually in your pantry, soonest-to-expire first |
| **[Tournament Leaderboard](https://tournament-leaderboard.irmahs.dev)** | Leaderboards, match stats and schedules for seasonal Valorant tournaments, such as Alsace Arena's Spike Tournament |

## How they are built

- **One look:** every app uses **Cute Matcha**, Irma's own design system, in light and dark.
- **One sign-in:** [auth](https://github.com/irmahs-labs/auth) gives every app the same Google sign-in, so your quiz results, games and draconoid follow you from one app to the next, and private apps stay with the people invited.
- **One front door:** [proxy](https://github.com/irmahs-labs/proxy) is the Caddy server that routes each `*.irmahs.dev` address to its app.
- **The same rules everywhere:** new repos start from [template](https://github.com/irmahs-labs/template) and share their CI through [workflows](https://github.com/irmahs-labs/workflows). Every change goes in through a pull request, with lint, type-checks, tests and a Docker build.

Built with TypeScript, React, Vite, Hono, Next.js, Postgres and Docker (plus Java, Spring Boot and Angular for the tournament site), with a lot of help from Claude.
