# M45 Staff ChatWire Help

Paste sections as needed in Discord. Slash command examples use Discord option names.

## Ban / Player Level
Do not casually ban and unban. Use banish or jail for time-outs if you are not certain.

- Set player level: `/player-level name:<factorioName> level:<choice> ban-reason:<reason>`
- Quick-ban example: `/player-level name:grieferName level:Banned ban-reason:logged in and started deleting everything: https://m45sci.xyz/u/fact2/new-logs/a/game-01-April-2069.log`
- Levels: `Moderator`, `Veteran`, `Regular`, `Member`, `New`, `Banned`, `Deleted`

## Uploads
- Upload save: `/upload save-game:<file attachment>`
- Replace mod list: `/upload mod-list:<file attachment>`
- Replace mod settings: `/upload mod-settings:<file attachment>`

Mod settings files contain global mod settings, not map-specific settings.

## Mods
- Show installed mods: `/list-mods`
- Enable mods: `/editmods enable-mod:<mod1,mod2>`
- Disable mods: `/editmods disable-mod:<mod1,mod2>`
- Add mods by name or portal URL: `/editmods add-mod:<mod-url-1,mod-name-2>`
- Set version preference: `/editmods set-version-pref:<mod=version>`
- Use latest or clear preference: `mod=auto` or `mod=`
- Erase all mod files: `/editmods clear-all-mods:true`
- Show mod history: `/editmods mod-history:true`
- Show full mod history: `/editmods full-history:true`
- Clear mod history: `/editmods clear-history:true`

## Map Reset Schedule
- Set interval: `/map-schedule interval-months:<number> interval-weeks:<number> interval-days:<number> interval-hours:<number>`
- Force reset hour UTC: `/map-schedule reset-hour:<0-23>` (`0` means none)
- Force next reset date UTC: `/map-schedule reset-date:<YYYY-MM-DD HH-MM-SS>`
- Disable automatic reset schedule: `/map-schedule disable:true`
- Set open hours UTC: `/config-hours start-hour:<1-23> end-hour:<1-23> enabled:<true|false>`

## Maps
- Rewind menu: `/change-map`
- List older saves: `/change-map list:true`
- Load save: `/change-map load:<save name>`
- Archive and generate new: `/map-reset`
- Generate new map: `/factorio action:new-map`
- Choose future map generator: `/map-generator`
- Map generator editor: https://mapgen.m45sci.xyz
- Generate from exchange string: `/map-exchange exchange-string:<map exchange string>`
- Archive current map: `/factorio action:archive-map`
- Sync mods from save: `/factorio action:sync-mods`
- Update all mods: `/factorio action:update-mods`

## Map Settings
- Name: `/config-server name:<name>`
- UDP port: `/config-server port:<1024-65535>`
- Members only: `/config-server members-only:<true|false>`
- Regulars only: `/config-server regulars-only:<true|false>`
- Map preset: `/config-server map-preset:<default|rich-resources|marathon|death-world|death-world-marathon|rail-world|ribbon-world|island|lakes>`
- Friendly fire: `/config-server friendly-fire:<true|false>`
- Auto-pause when empty: `/config-server auto-pause:<true|false>`
- Game speed: `/config-server speed:<0.01-10>`
- Autosave minutes: `/config-server autosave-mins:<5-30>`
- AFK kick minutes: `/config-server afk-kick-mins:<5-120>`
- Next-map seed: `/config-server map-seed:<seed>`

## M45-Softmod
- Inject softmod scripts: `/config-server soft-mod-inject:<true|false>`
- Restrict new players: `/config-server restrict-new-players:<true|false>`
- Disable blueprints: `/config-server disable-blueprints:<true|false>`
- One-Life: `/config-server one-life:<true|false>`
- Scenario for new maps: `/config-server scenario:<name|none>`
- Scenarios: `freeplay`, `pvp`, `rocket-rush`, `sandbox`, `supply`, `team-production`, `wave-defense`

## Factorio
- Start or restart: `/factorio action:start`
- Stop: `/factorio action:stop`
- Update Factorio: `/factorio action:update-factorio`
- Force reinstall: `/factorio action:install-factorio`
- RCON all maps: `/rconall command:<command>`
- RCON current map channel: `/rcon command:<command>`
- Factorio console reference: https://wiki.factorio.com/console#Multiplayer_commands

## ChatWire
- Reboot: `/chatwire action:reboot`
- Reboot when empty: `/chatwire action:queue-reboot`
- Reboot Factorio only when empty: `/chatwire action:queue-fact-reboot`
- Reload config after SSH edits: `/chatwire action:reload-config`
- Last resort, can corrupt data: `/chatwire action:force-reboot`
- Hide autosaves: `/config-server hide-autosaves:<true|false>`
- Hide research: `/config-server hide-research:<true|false>`

## Firewall IP Bans
Primary server only. Ban and unban require a public IPv4 address; list has no IP.

- List UFW deny rules: `/ip-ban action:list`
- Ban public IPv4: `/ip-ban action:ban ip:<public IPv4>`
- Unban public IPv4: `/ip-ban action:unban ip:<public IPv4>`

## Advanced
- Auto-update Factorio: `/config-server auto-update-factorio:<true|false>`
- Auto-update mods: `/config-server auto-mod-update:<true|false>`
- Experimental Factorio builds: `/config-server auto-update-experimental:<true|false>`
- Auto-start Factorio on boot: `/config-server auto-start-factorio:<true|false>`
- Server group prefix: `/config-global group-name:<2-5 chars>`
- Global command handler: `/config-global primary-server:<callsign>`
- User report channel: `/config-global report-channel:<channel>`
- Announcement channel: `/config-global announce-channel:<channel>`
- Server browser description: `/config-global description:<text>`
- Maximum autosaves to keep: `/config-global autosave-max:<64-1024>`
- Disable chat spam protection: `/config-global disable-spam-protect:<true|false>`
- Mute suspicious activity messages: `/config-global sus-shutup:<true|false>`
- FCL warn only: `/config-global fcl-warn-only:<true|false>`
- Warn regulars about FCL bans: `/config-global fcl-warn-regulars:<true|false>`
