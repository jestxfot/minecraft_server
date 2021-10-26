help [search]   Show help menu. Optionally search.
exit    Exit DiscordConsole
exec    Execute a shell command
run     Run a LUA file with DiscordConsole's special functions
alias <command> <new command>   Add a new alias for a command.
lang <language> Same as starting with --lang
latency Shows the last heartbeat's ping.
permcalc [preset]       Open the permission calculator, and optionally with pre-set values.

guilds          List guilds/servers you're in.
guild <id>      Select a guild to use for further commands.
channels        List channels in your selected guild.
channel <id>    Select a channel to use for further commands.
pchannels       List private channels a.k.a. 'DMs'.
vchannels       List voice channels in your selected guild.
dm <user id>    Create a DM with specific user.

region <list/set> (<region>)    Set current guild region.

info <user/guild/channel/settings> (for user: <id/@me>) [property] (or info u/g/c/s)    Get information about a user, server, channel or your set Discord settings!
read <message id> [property]    Read or get info from a message. Properties: (empty), text, channel, timestamp, author, author_email, author_name, author_avatar, author_bot, embed; 'cache' may be used as message ID.
pin <message id>        Pin a message to the current channel.
unpin <message id>      Unpin a message from the current channel.

name <name>     Change username completely.
avatar <link/file>      Change avatar to a link or file.

say <stuff>     Send a message in your selected channel. `say toggle` starts chat-mode, and `toggle` ends it.
${Placeholders}:        Replaces e.g. ${u.name} with ЙЦУКЕН - Бот.
sayfile <path>  Send the contents of a file (auto-splitted).
big <stuff>     Send a message, but attempt to make it using emojis!
embed <json>    Send an embed! (ADVANCED!) See https://discordapp.com/developers/docs/resources/channel#embed-object
tts <stuff>     Send a TTS message in your selected channel.
file <file>     Upload file to selected channel.

edit <message id> <stuff>       Edit a message in your selected channel.
editembed <message id> <json>   Edit a message embed in your selected channel.
del <message id>        Delete a message in the selected channel.
delall [since message id]       Bulk delete messages since a specific message
log <directly/file> <amount OR filename>        Log the last few messages in console or to a file.
react add/del <message id> <emoji unicode/id>   React to a message
react big <message id> <stuff>  Like the 'big' command, but in reactions!
react delall <message id>       Delete all reactions

playing [game]  Set your playing status. Run without an argument to clear.
streaming [url] [game]  Set your streaming status.
game <streaming/watching/listening> <name> [details] [extra text]       Set a custom status.
typing  Simulate typing in selected channel.

members List (max 100) members in selected guild
invite create [expires] [max uses] ['temp'] OR invite accept `code` OR invite read `code` OR invite list OR invite revoke `code` Create an invite, accept an existing one, see invite information, list all invites or revoke an invite.

role list       List all roles in selected guild.
role add <user id> <role id>    Add role to user
role rem <user id> <role id>    Remove role from user
role create     Create new role
role edit <role id> <flag> <value>      Edit a role. Flags are: name, color, separate, perms, mention
role delete <role id>   Delete a role.

nick <id> [nickname]    Change somebody's nickname
nickall [nickname]      Change ALL nicknames!

messages [scope]        Intercepting messages. Optionally, scope can have a filter on it: all, mentions, private, current (default), none
intercept [yes/no]      Toggle intercepting 'console.' commands in Discord.
output [yes/no] Toggle showing 'console.' outputs directly in Discord.
back    Jump to previous guild and/or channel.

new <channel/vchannel/guild/category> <name>    Create a new guild or channel
bans [text]     List all bans, can also be shown in text form to show full ban reasons.
ban <user id> <optional reason> Ban user
unban <user id> Unban user
kick <user id> <optional reason>        Kick user
leave [id]      Leave a guild! Run with no arguments to leave the selected one.
ownership <id>  Transfer ownership.

delete <guild/channel/category> <id>    Delete a channel, guild or category.

play <dca audio file>   Plays a song in the selected voice channel
stop    Stops playing any song.
move <user id> <vchannel id>    Move a user to another voice channel.

status <value>  Set the user status. Possible values are: online, idle, dnd and invisible.

friend <add/accept/remove/list> (<user id>)     Manage your friends. Add, accept, remove and list them.
block <user id> Block a user.
note <user id> <note>   Set a note. Remove with `note <user id> ""`.

bookmarks       List all bookmarks in the console.
bookmark <name> Create new bookmark out of current location. If the name starts with -, it removes the bookmark.
go <bookmark>   Jump to the specified bookmark.

rl [full]       Reload cache. If 'full' is set, it also restarts the session.
