---
title: API Documentation
description: Reference documentation for HaloRuns API endpoints and usage.
leaderboard: https://haloruns.com/api/request?query=recentRuns&format=json
discord: https://haloruns.com/discord
---

The HaloRuns API is entirely contained in the subdirectory `/api/`. There are some conventions that multiple API calls follow.

## Level IDs

Each level on HaloRuns can be referred to by a 4-character string of numerals. This string is produced by concatenating the number of the game that the level occurs in with the level's number within that game. For example, Tip of the Spear in Halo: Reach's ID is `0504`.

## Game Numbers

| Game                 | Number |
|----------------------|--------|
| Halo: Combat Evolved | 01     |
| Halo 2               | 02     |
| Halo 3               | 03     |
| Halo 3: ODST         | 04     |
| Halo: Reach          | 05     |
| Halo 4               | 06     |
| Halo 2 MCC           | 07     |
| Halo 5               | 08     |

## Level Numbers

### Halo: Combat Evolved

| Level                       | Number |
|-----------------------------|--------|
| Pillar of Autumn            | 01     |
| Halo                        | 02     |
| Truth and Reconciliation    | 03     |
| The Silent Cartographer     | 04     |
| Assault on the Control Room | 05     |
| 343 Guilty Spark            | 06     |
| The Library                 | 07     |
| Two Betrayals               | 08     |
| Keyes                       | 09     |
| The Maw                     | 10     |

### Halo 2

| Level             | Number |
|-------------------|--------|
| Cairo Station     | 01     |
| Outskirts         | 02     |
| Metropolis        | 03     |
| The Arbiter       | 04     |
| Oracle            | 05     |
| Delta Halo        | 06     |
| Regret            | 07     |
| Sacred Icon       | 08     |
| Quarantine Zone   | 09     |
| Gravemind         | 10     |
| Uprising          | 11     |
| High Charity      | 12     |
| The Great Journey | 13     |

### Halo 3

| Level         | Number |
|---------------|--------|
| Sierra 117    | 01     |
| Crows Nest    | 02     |
| Tsavo Highway | 03     |
| The Storm     | 04     |
| Floodgate     | 05     |
| The Ark       | 06     |
| The Covenant  | 07     |
| Cortana       | 08     |
| Halo          | 09     |

### Halo 3: ODST

| Level            | Number |
|------------------|--------|
| Prepare to Drop  | 01     |
| Tayari Plaza     | 02     |
| Uplift Reserve   | 03     |
| Kizingo Blvd.    | 04     |
| ONI Alpha Site   | 05     |
| NMPD HQ          | 06     |
| Kilowani Station | 07     |
| Data Hive        | 08     |
| Coastal Highway  | 09     |

### Halo: Reach

| Level                | Number |
|----------------------|--------|
| Winter Contingency   | 01     |
| ONI: Sword Base      | 02     |
| Nightfall            | 03     |
| Tip of the Spear     | 04     |
| Long Night of Solace | 05     |
| Exodus               | 06     |
| New Alexandria       | 07     |
| The Package          | 08     |
| The Pillar of Autumn | 09     |

### Halo 4

| Level      | Number |
|------------|--------|
| Dawn       | 01     |
| Requiem    | 02     |
| Forerunner | 03     |
| Infinity   | 04     |
| Reclaimer  | 05     |
| Shutdown   | 06     |
| Composer   | 07     |
| Midnight   | 08     |

### Halo 5

| Level                | Number |
|----------------------|--------|
| Osiris               | 01     |
| Blue Team            | 02     |
| Glassed              | 03     |
| Unconfirmed          | 04     |
| Evacuation           | 05     |
| Reunion              | 06     |
| Swords of Sanghelios | 07     |
| Enemy Lines          | 08     |
| Battle of Sunaion    | 09     |
| Genesis              | 10     |
| The Breaking         | 11     |
| Guardians            | 12     |

## API Calls

## Global Modifiers

### Format

Specifies how the API call's response will be formatted.

### json

JSON format. Example: <https://haloruns.com/api/request?query=recentRuns&format=json>

### prettyjson

JSON format, where each item in the object is a pretty printed string. Example: <https://haloruns.com/api/request?query=recentRecords&format=prettyjson>

### Country

Only display information associated with runners from the country specified by an ISO 3166 country code.

Example: <https://haloruns.com/api/request?query=country&country=mx>

## Recent Runs

`GET /api/request?query=recentRuns[&limit=N]`

Returns a list of the most recent verified runs submitted to the site. If `GET[limit]` isn't specified as a number below 50, the 50 latest runs are returned.

## Records

`GET /api/request?query=records&level=levelID[&isCoop=0&difficulty=0]`

Returns the current records for the level specified by `GET[level]`. If `GET[isCoop]` isn't specified, both solo and co-op records are returned. If `GET[difficulty]` isn't specified, both easy and legendary records are returned. If neither is specified, all 4 records for the level are shown in the following order: Solo Easy, Solo Legendary, Co-op Easy, Co-op Legendary.

## Recent Records

`GET /api/request?query=recentRecords[&limit=N]`

Returns a list of the most recent verified world records submitted to the site. If `GET[limit]` isn't specified as a number below 50, the 50 latest records are returned.

### default

If GET\[format\] isn't specified, then a comma-separated list of pretty-printed run descriptions is returned.

## Streams

`GET /api/request?query=streams`

Returns a list of the current streams being displayed on the HaloRuns homepage. This list is updated every 5 minutes.

### default

If GET\[format\] isn't specified, then a comma-separated list of HaloRuns usernames is displayed.

## User

`GET /api/request?query=user[&user=username]`

Grabs the username, total points, and describes the most recent run submitted by the user specified by `GET[user]`.

## Record Vods

`GET /api/request?query=wrVods&level=levelID[&difficulty=0&isCoop=0]`

Returns a link to the vod of the world record for the level specified by `GET[level]`. If `GET[difficulty]` isn't specified, the Easy record is fetched. If `GET[isCoop]` isn't specified, the Solo record is fetched.

## Record Holders

`GET /api/request?query=wrHolders`

Returns a list of every user on HaloRuns who has ever held a world record at any point.
