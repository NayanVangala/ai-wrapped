# AI Wrapped

Spotify Wrapped, but for your AI usage. Connect your AI accounts, get your year in review: total tokens, spend in USD, favorite models, peak hours, topics, streaks — everything.

## The idea

Every December, Spotify tells you who you were. AI is eating the same amount of our lives, but nobody wraps it. AI Wrapped reads your data and turns it into a shareable story:

- **Tokens & spend** — total tokens used, estimated USD across providers
- **Favorite models** — which model you actually lived in this year
- **Rhythm** — peak hours, best days, longest streaks
- **Topics** — what you kept asking about
- **Personality** — your AI alter ego, Wrapped-style

## Data sources

Most AI companies don't offer consumer usage APIs, so v1 works from what you can actually get:

| Source | How |
|---|---|
| ChatGPT | Data export (`conversations.json`) |
| Claude | Data export |
| OpenAI API | API key → real usage + cost endpoints |
| Demo mode | Built-in synthetic year, zero setup |

All parsing happens client-side. Nothing leaves the browser. Token counts from exports are estimates (~4 chars/token) and always labeled as such.

## Roadmap

- [ ] ChatGPT export parser
- [ ] Claude export parser
- [ ] OpenAI usage API connector
- [ ] Wrapped story UI (slides, animated counters)
- [ ] Share card image export
- [ ] Gemini / Copilot / other sources

## Honest limits

- No usage APIs exist for most consumer AI plans — exports are the source of truth.
- Token and cost figures from exports are estimates, shown as estimates.
- Built in the open. PRs welcome.
