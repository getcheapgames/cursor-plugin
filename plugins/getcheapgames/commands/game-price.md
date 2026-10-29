---
name: game-price
description: Find where a game is cheapest right now, with the price on each platform and a link to compare every store.
---

# Game price

1. Ask which game, if it was not given, and which country the reader buys in (default ie).
2. Call `search_games` with the game's name and the `country`, and take the best match.
3. Call `get_game_offers` with its `slug` and the same `country`.
4. Answer with the lowest price on each platform, the cheapest store with its key's platform and region, any region-lock warning, the 30-day low if given, and the game's `pageUrl`.
