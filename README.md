# Open-SteamDB

**This is not the official SteamDB repository.**

After SteamDB was [acquired by Nexus Mods’ parent company](https://steamdb.info/blog/steamdb-nexus-mods/), I started this project to recreate its tracking system.

I want to keep these records public, so anyone can look them up for personal projects, research, or other non-commercial purposes.

## What you can find

This archive keeps records of:

- **Game details** — names in available languages, genres, features, release status, and links to Steam’s images and videos.
- **Player counts** — how many people are playing, along with recorded averages and peaks.
- **Reviews** — positive and negative review totals and how they change over time.
- **Prices** — regional prices, discounts, availability, and price history.
- **Game updates** — changes to Steam’s game information, builds, and download packages.

The tracker follows Demo releases, Early Access launches, and full releases. Each Steam AppID keeps its own history, including changes in release status.

## How to find a game

You can search this repository for a game’s name or its Steam AppID.

An AppID is the number in a game’s Steam store address. For example, [No Man’s Sky](https://store.steampowered.com/app/275850/No_Mans_Sky/) has this address:

```text
https://store.steampowered.com/app/275850/No_Mans_Sky/
```

Its AppID is **275850**.

Search for that number to find any records available for the game. Game records are stored under `data/`, with a separate folder for each AppID.

## Updates

| Records | Usual update schedule |
|---|---|
| Player counts | Every 15 minutes |
| Review totals | Daily |
| Regional prices | Daily |
| Game details | Daily |
| Game updates and builds | Every 15 minutes |
| New release discovery | Every 15 minutes |

Daily price checks start at **10:05, 10:10, and 10:15 Pacific Time**.

New entries are added to price history only when the price, discount, or availability changes. Unchanged prices are not added again.

Update records are also saved when a change is found, rather than repeating the same information at every check.

## Where the history comes from

The tracker records current information directly from Steam.

Some games were already available before tracking began, so this archive does not have its own records of their earlier prices. Where available, those older Steam prices are imported from **IsThereAnyDeal**.

Imported prices are saved in the same price file as the tracker’s records, but in a separate list, so you can tell which source they came from.

Older player-count records may also come from **Steam Charts**. Their source is kept with the imported data.

## Acknowledgments

- Thank you to [SteamDB](https://steamdb.info/) for years of service to the Steam community and for inspiring this project.
- **Special thanks to [GitHub](https://github.com/) for providing the infrastructure that makes this archive possible.**
- Very special thanks to [IsThereAnyDeal](https://isthereanydeal.com/) for its historical price data and for generously sharing it with the community.
- Very special thanks to [Steam Charts](https://steamcharts.com/) for its historical player data and for generously sharing it with the community.

## Use and limitations

This archive is intended for **non-commercial use**.

I can’t guarantee that every change will be captured or that every record will be complete or accurate. All information is provided for reference.

A missing record does not mean that nobody was playing, that a game was free, or that nothing changed.

This archive contains information about games, not game files.

Steam and its related trademarks belong to Valve. Game titles, artwork, and other third-party content belong to their respective owners. This project claims no ownership of that content.
