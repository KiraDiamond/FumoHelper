# FumoHelper

Public information page for **FumoHelper**.

FumoHelper is an unofficial Discord app for **FUMO**. It provides player stat lookups,
raid stat views, activity tracking, guild contribution leaderboards, war counts,
and guild raid logs.

This repository is public so people can see what the project is.
It does **not** contain the actual bot source code.

## Included Here

- Project overview
- Feature list
- Command list with explanations
- Public landing page

## Not Included Here

- Bot source code

## Notes

- FumoHelper is **not** an official guild app.
- The source for the running bot is not public.
- The site entry point is `index.html`.

## Active Command Reference

Below is the current public command overview for the running bot.

### `commands/player.py`

**Command:** `/player`

Shows a player card for a Wynncraft account.

Includes:
- Main profile overview
- Class summary
- General account progress and visible profile stats

### `commands/rstats.py`

**Command:** `/rstats`

Shows raid-specific stats for a player.

Includes:
- Raid completion totals
- Raid-by-raid breakdowns
- Visual stat card for quick comparison

### `commands/activity.py`

**Command:** `/activity`

Shows tracked activity data gathered by the bot over time.

Includes:
- Recent tracked stat gains
- Playtime tracking
- Activity summary card
- Recent raid/activity context where available

### `commands/contribution_leaderboard.py`

**Command:** `/gxp`

Shows the guild contribution leaderboard.

Modes:
- Recent contribution leaderboard
- All-time contribution leaderboard

### `commands/warcount.py`

**Command:** `/warcount`

Shows tracked war totals for a guild member over a selected timeframe.

Useful for:
- Checking recent war participation
- Comparing tracked war counts between members

### `commands/graids.py`

**Commands:**
- `/graids`
- `/graids_recent`
- `/graids_total`
- `/aspect_log`

Guild raid tracking commands.

What they do:
- `/graids` shows detected guild raids for one player
- `/graids_recent` shows recently detected guild raids across the guild
- `/graids_total` shows a raider leaderboard by tracked raid count
- `/aspect_log` shows tracked owed aspects based on raid participation

### `commands/guild.py`

**Command:** `/guild`

Shows a guild overview.

Includes:
- Guild lookup information
- General guild summary data
- Member and level-related information from the lookup result

### `commands/guild_action.py`

**Command:** `/guild_action`

Shows recent tracked guild events.

Includes:
- Joins
- Leaves
- Promotions
- Demotions
- Guild level-ups

### `commands/xpcon.py`

**Command:** `/xpcon`

Admin-facing contribution lookup command.

Used for:
- Looking up one player’s tracked contribution totals
- Viewing a contribution ranking list from tracked data

### `commands/tracker.py`

**Commands:**
- `/debug forcepoll`
- `/debug tracker_status`

Owner-only tracker/debug commands.

What they do:
- `forcepoll` forces the tracker to refresh tracked guild/player data
- `tracker_status` reports whether the tracker is currently running

## Current Public Feature Summary

- Player stats
- Raid stats
- Activity tracking
- Guild contribution leaderboards
- War counts
- Guild raid logs
- Guild action history
- Tracker/debug tools for maintenance
