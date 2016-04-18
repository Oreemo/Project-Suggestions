# Overview
Reads, filters and modifies all traffic between osu! client and server.

# When?
The osu! relay server isn't the easiest thing to do as it being modular would be highly beneficial for public use, making it non modular would take less time though so that is a possibility that one can use on the very first release of the osu! relay server.

# Features
1. Censor banned words to prevent silence (modify: fuck -> f***)
1. OR Intercept bannable words, returning a bancho warning message
1. Ask if score should be submitted (only if better than current player skill / hacked?)
1. Prevent spectating / skip suspicious frames (jumping cursor)
1. Spoof multiplayer score
2. Spoof Processlist / Screenshots / Appdata / other data that could lead to a ban
1. Custom server-side commands/macro's (eg: !downloadmap [id], !massmessage [message], !playerinfo [playerid/playername])
1. Integrate IRC, aqn or stream chat
1. Integrate RSS feed as chat
1. Encrypt chat with other Relay Server users (RSA)
1. Connect with Calendar (Like google's), + Notifications
1. Macros, like _DATE, _LOCATION or _USERNAME (Replace with dynamic data in message)
1. Spoof hardware data (hwid, unique id..., location, ip)
1. Gives general connection data on connectivity issues + http://stat.ppy.sh/
1. Gives you pp of last play / Mikuia Bot Functionality
1. Informs of specifiable players' new plays / maps
1. Automatically download multiplayer maps if player doesn't have them
1. Fake messages of other people (gotta make those false accusations)
1. Use command line from chat
1. AFK Messages
1. Translate messages with Google Translator
1. Masking names/nameprotect (for those who like to stream, also for friends / people who send private messages)
1. Hide or spoof pp/score, as a protection for streamers
2. Make client display Guest status while still submitting stuff
1. Multi-server support, submit to 2 servers at once.
2. memes
3. easter eggs
4. Private Multiplayer (Scores submitted online, lobby only exists on relay servers)
5. Restricted Ranker (Show pp and other data even on restricted accounts)
6. Lua Scripting support for modularity (Probably the easiest and there will be no problems with C++ or C# preferences)
7. Could work well with [Ingame Overlay](Ingame Overlay.md)
8. Make friends appear in a custom color in chat
9. Spoof Online leaderboards 
10. Spoof Client version
11. Enable and Simulate osu!direct (Bloodcat or something)
12. Spoof beatmap version (Or just a completely different beatmap altogether)
13. Automatically put replays of fcs in a database usable with [Replay Studio](Replay Studio.md)
14. Stats (Sent, recieved messages, traffic size...)
15. Score fixer (You did get that fc after all / Could modify replay data accordingly)
16. Stay online on 2 (or more) accounts simultanously (chat, scores?)
17. Make it able to edit the user panel (such as Hakurei Reimu back in the day used to have a pseudo userpanel made in Photoshop). This allows you to display different information. (like other name, pp etc...)
18. Break Suggester (Suggests people to take a break after 2 hours of activity, might block connection until break was taken)


## Possible commands
| Command            | Explanation  | 
| -------------------|------------- |
| !maps [name]       | Gets all maps by this user |
| !downloadmap [id]  | Downloads map using client-side program      |
| !playerinfo [name] | Get extended playerinfo returned as bancho message|
| !chatfilters       | Sends [this](https://gist.github.com/shavitush/798987e2fe32225b9125) list. |
| !ping [server]     | Pings a server and gives the results
| !pp [id] [mods]    | Gets Tillerino style pp calculation for the current map.|
| !ar [mod]          | Calculates the ar with the selected mod as well as the time in ms.|

## Output methods
Method | Explanation
--- | ---
Bancho message | Bancho message in main chat channel (#osu)
Custom channel | Bancho-like message in custom chat channel (#log, #console)
Notifier | Bancho can trigger notifier balloons, which can be used for output
