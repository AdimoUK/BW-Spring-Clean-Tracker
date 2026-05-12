# BadWolfMC Spring Cleaning Challenge Tracker

A browser-based daily task tracker for the BadWolfMC Minecraft server's Spring Cleaning Challenge (11 May – 1 June 2026).

**Live page:** https://adimouk.github.io/BW-Spring-Clean-Tracker/

---

## What it does

- Lists all 21 daily tasks with their expiry times (shown in your local timezone)
- Lets you tick off each day after visiting Cesar at the Mall
- Tracks your progress toward the 18/21 day prize — an **Unbreakable Feather Duster**
- Saves your progress automatically in your browser (localStorage)
- Printable — fits on one page with dotted lines for pen-and-paper use

## How the quest data works

Each day's requested items are stored in [`quests.json`](quests.json). This file is updated daily as new tasks are revealed. You don't need to enter quest info yourself — just refresh the page to pick up the latest data.

If a day's quest hasn't been filled in yet, the column will show a blank dotted line.

## Updating quest data (maintainer)

Edit [`quests.json`](quests.json) and fill in the item(s) requested for that day, then push to `main`. GitHub Actions will deploy the update automatically within a minute.

```json
{
  "1": "63x Rotten Flesh",
  "2": "64x Stick",
  "3": ""
}
```

## Challenge details

| Detail | Info |
|---|---|
| Duration | 21 days |
| Daily reset | 0:00am ET (midnight Eastern) |
| Prize threshold | 18 out of 21 days |
| Max days you can miss | 3 |
| Prize | Unbreakable Feather Duster |

Each daily task is only available for 24 hours and **cannot be made up** if missed.
