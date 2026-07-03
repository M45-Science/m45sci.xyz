# M45 Player Help

## Membership and Roles
- Auto-register by scoring points while you play.
- `Member`: Play public maps to unlock private servers.
- `Regular`: More channels, more servers, and extra say in banish votes.
- `Veteran`: Double vote power and the ability to banish misbehaving Regulars.

## Discord Commands
These commands work in map-specific Discord channels.

- `/register` - Run this first so the bots know who you are.
- `/vote-map` - Rewind, reset, or skip the scheduled reset.
- `/info [options:verbose]` - Show server details.
- `/modpack` - Get a link to the installed mods.
- `/players` - List current players.
- `/pause-game [action:pause|cancel]` - Pause for 3 minutes while you connect, or cancel a pending pause.
- `/whois search:<player>` - Look up a player.
- `/scoreboard` - Show top 40 players.
- `/list-mods` - Show mods on this map.
- `/get-roles` - Manage notification roles.

## Map Channel Status
Map channels bridge Discord and Factorio. Icons show status:

- `⚪` Public map, anyone can join
- `🟢` Members-only, `@Member` required
- `🟠` Regulars-only, `@Regular` required
- `🔴` Veterans/invite-only, `@Veteran+` required
- `⚫` No players online

If a number comes first, that is the current player count.

## Logs and Activity
- ChatWire messages use `days-hours-minutes-seconds`; Discord shows your local time.
- Look for autosave messages in Discord and pair them with Factorio timestamps to rewind.
- Need a save older than 25 autosaves? Ask in `❓moderation-help`.
- Activity logs: https://m45sci.xyz/u/fact2/new-logs/
- ChatWire game logs are named `game-YYYY-MM-DD.log`.
- Logs use UTC.

## Notification Roles
- Use `/get-roles` anytime to manage subscriptions.
- No `@everyone` pings; opt into what you care about.
- Roles: `Emergency Alert`, `Help-Vote`, `Factory-Help`, `Announcements`.
