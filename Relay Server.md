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


# Possible commands
| Command           | Explanation  | 
| -------------------|-------------|
| !maps [name]       | Gets all maps by this user |
| !downloadmap [id]  | Downloads map using client-side program      |
| !playerinfo [name] | Get extended playerinfo returned as bancho message|
|!chatfilters        | Sends [this](https://gist.github.com/shavitush/798987e2fe32225b9125) list. |
