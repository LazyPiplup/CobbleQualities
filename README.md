# CobbleQualities

CobbleQualities adds a selection of quality-of-life and cosmetic enhancement items to Cobblemon, focusing on portable utility and player-driven customization. Manage, heal, and personalize your Pokémon anywhere.

---

## TO-DO
- **Finish the discord**
- **Finish setting up the github to allow for bug reports and issues**
- **Refactor and organize the project files in a cleaner manner**
- **Quit Being a Lazy Piplup**

**THIS IS EMPTY FOR NOW UNTIL I REORGANIZE THE PROJECTS FILES AND NAMING ARCHITECTURE**

---

## Features

- **Portable PC (utility)** — Opens your Pc interface anywhere, perfect for exploring.
- **Portable Healer (utility)** — Heals your parties Pokémon, fast and convenient after a tough fight.
- **Shiny Shard (consumable)** — Use to turn one of your Pokémon ✨Shiny✨.
- **AND MORE TO COME!**

---

## Usage

- **Portable PC**: Right-click while holding to open your storage UI.  
- **Portable Healer**: Right-click to heal the current Pokémon in your party.  
- **Shiny Shard**: Upon use select a Pokémon to apply the shiny effect to.
  
---

## Configuration

All drops and drop chances for shiny pokemon are configurable in:  
`config/cobblequalities/shinylootpool.json`

Configs can be reloaded during runtime by using:  
`/cobblequalities reloadconfigs`

If for some reason you want to disable shiny drops you can use the gamerule:  
`/gamerule toggleShinyDrops` otherwise it is set to "true" by default.

Example snippet:
```json
{
  "ultrarare": {
    "chance": 0.01,
    "entries": [
      { "item": "modid:item_ultrarare", "amount": 1, "weight": 10 }
    ]
  },
  "rare": {
    "chance": 0.05,
    "entries": [
      { "item": "modid:item_rare", "amount": 2, "weight": 8 }
    ]
  },
  "uncommon": {
    "chance": 0.15,
    "entries": [
      { "item": "modid:item_uncommon", "amount": 1, "weight": 6 }
    ]
  },
  "common": {
    "chance": 0.79,
    "entries": [
      { "item": "modid:item_common", "amount": 1, "weight": 4 }
    ]
  }
}
```
