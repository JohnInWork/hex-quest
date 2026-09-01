**English** · [Русский](README.ru.md)

# Hex Quest

Turn-based exploration of an endless hex map. The whole board is hidden under fog; every click reveals one neighbouring tile and immediately plays out whatever sits under it. The goal is to score as much as you can before health and food run out.

![Hex Quest](screenshots/gameplay.png)

## Rules

Three resources: **health** (6 hearts, never restored), **food** and **swords**. Food drains every turn, so standing still isn't an option.

| Tile | What it does |
|---|---|
| Grass, sand | Move in, +1 point; sand sometimes hides gems |
| Desert, snow | +2 and +3 points, but snow costs food |
| Water | Impassable, only revealed |
| Forest, cactus, mountain | Points paid for with food: +2, +2, +3 |
| House | +4 food, once |
| Castle | +1 sword |
| Wolf, tiger, skull, dragon | Fought with swords: the nastier the enemy, the bigger the reward and the risk |
| Coin, chest, beacon, portal | Coins, a rare big payout, teleport |

Points are awarded per tile only once, which keeps you pushing into new ground instead of pacing over what's already open. You can only move onto neighbours of tiles you've already revealed.

## What else is inside

- **A 4000×4000 map** with lazy generation: tiles are computed as you approach them, the world is never drawn all at once.
- **Landscape instead of randomness** — forests and mountains grow in clusters, water gathers into lakes, snow and desert form biomes, while enemies and buildings stand alone.
- **Inventory and gear** — a map, potions, a teleport stone, food and sword packs, a hunter's mark, iron armour, warm boots, a holy helmet, a sword, a mace, a wolf bow. Some are consumed, others change the rules while worn.
- **Progression between runs** — coins buy more inventory slots, more health, more starting food and swords.
- **The sea and what lives in it** — ships, sharks, an octopus with its own fight scene; a phoenix and a message in a bottle as rare finds.
- **Quests** — "explore 4 forests", "conquer 5 mountains"; the coin reward grows as you complete them.
- **15 playable characters** bought with coins — mage, berserker, collector, dragonslayer, mermaid, phoenix, bear, demon, vampire, robot, alien and more; each has an ability that bends the rules.
- Achievements, a leaderboard, an encyclopedia of objects, random events with choices, and a textured or texture-free mode.
- Music is off by default, sound effects are on — both toggle from the menu and in-game.

## Running it

Open `Hexagons.html` in a browser. Sounds live in `Sounds/`, icons in `Icons/`.

`Versions/` holds eight earlier builds, from the first prototype to the current one.

## Stack

A single HTML file: canvas, plain JS, no libraries.
