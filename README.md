# EIRA — League Coach & Stats

A free desktop assistant for League of Legends. Working prototype, Windows, in
active development.

**Product page:** `index.html` in this repository, published through GitHub
Pages. That page is the URL given to Riot Games in the developer portal.

---

## What EIRA does

| When | What |
|---|---|
| Champion select | Reads the lobby, works out the matchup and the enemy damage profile, proposes a rune page for the champion **and the position**. Written to the client only on your confirmation, never over a page you made yourself. |
| In game | An overlay reads Riot's official Live Client Data API and names the next item from what the enemy team actually bought and who is ahead. |
| After the game | The match timeline is used to reconstruct lane phase, gold curves, deaths and objectives, and to produce specific notes instead of generic advice. |
| Between games | Win rates per champion, matchup, rune page and item — counted from ranked matches EIRA samples itself, each with its sample size. |

## Where the data comes from

**Riot Games API** — ACCOUNT-V1, SUMMONER-V4, LEAGUE-V4, MATCH-V5 (matches and
timelines), SPECTATOR-V5.

**Local, on the player's machine** — the Live Client Data API for the running
match, the LCU for champion select and rune pages, Data Dragon and Community
Dragon for champions, items, runes and icons.

Nothing is scraped from op.gg, u.gg or any other statistics site.

## What it will never do

- No gameplay automation. EIRA does not press keys and does not move your champion.
- No reading or modifying game memory.
- Nothing shown during a match that the player cannot already see on their own screen.
- The API key is stored encrypted on the machine, never logged and never exposed.
- Free. No ads, no paid features.

## Status

| Game | State |
|---|---|
| League of Legends | working |
| Teamfight Tactics | in progress |
| VALORANT | planned |

Each game is registered separately with Riot, as the developer portal requires.

---

EIRA isn't endorsed by Riot Games and doesn't reflect the views or opinions of
Riot Games or anyone officially involved in producing or managing Riot Games
properties. Riot Games, and all associated properties, are trademarks or
registered trademarks of Riot Games, Inc.
