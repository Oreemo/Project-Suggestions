# Overview
Reads filters and modifies all traffic between osu! client and server.

# Features
1. Censor banned words to prevent silence (modify: fuck -> f***)
1. OR Intercept bannable words, returning a bancho warning message
1. Ask if score should be submitted (only if better than current player skill / hacked?)
1. Prevent spectating / skip suspicious frames (jumping cursor)
1. Spoof multiplayer score
1. Custom server-side commands/macro's (eg: !downloadmap [id], !massmessage [message], !playerinfo [playerid/playername])
1. Use bancho messages as output
1. Use notifier as output
1. Integrate IRC, aqn or stream chat
2. Integrate RSS feed as chat
3. Ecrypt chat with other Relay Server users (RSA)
4. Connect with Calender (Like google's), + Notifications
5. Macros, like _DATE, _LOCATION or _USER_NAME (Replace with dynamic data in message)
6. Spoof Unique data (hwid, unique id..., location, ip)
7. Gives general connection data on connectivity issues + http://stat.ppy.sh/
8. Gives you pp of last play / Mikuia Bot Functionality
9. Informs of specifiable players' new plays / maps
10. Automatically download multiplayer maps if player doesn't have them
11. Fake messages of other people (gotta make those false accusations)
12. Use command line from chat
13. AFK Messages
14. Translate messages with Google Translater


# Possible commands
| Command           | Explanation  | 
| -------------------|-------------|
| !maps [name]       | Gets all maps by this user |
| !downloadmap [id]  | Downloads map using client-side program      |
| !playerinfo [name] | Get extended playerinfo returned as bancho message|
| !chatfilters       | Sends [this](https://gist.github.com/shavitush/798987e2fe32225b9125) list. |
| !ping [server]     | Pings a server and gives the results
| !pp [id] [mods]    | Gets Tillerino style pp calculation for the current map.|

Eastereggs
