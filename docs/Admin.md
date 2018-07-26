# Administration / Moderation
Vexera supplies you with many **moderation and admin commands**. Useful for managing *high traffic guilds* or just to *punish* people much *easier*.

## Punishing Users

You got a **large range of commands to punish people**. Here, we will show and describe all of them.
To set a logging channel for infractions, check out [Logging](/docs/settings#logging)

### Warning
You can **warn** people by using `+warn <ID/Mention> [Reason]`.<br/>
For example, to warn the user `luke#0123` for misleading content, you may run `+warn luke#0123 Misleading Content`.

### Muting
You can **mute** people permanently or temporarily by using `+mute <ID/Mention> [Time] [Reason]`.<br/>
For example, to mute the user `luke#0123` for one week and 2 days, you would use `+mute luke#0123 1w2d Spamming`.<br/>
If you want your mute to be permanent, just leave out the time argument.<br/>
The muted role is created and set after the first mute has been issued. If you are having problems with the role, feel free to delete it in your server settings and mute someone afterwards so the roles is re-created.

### Kicking / Banning
If a user keeps violating the rules, you may want to **kick** or **ban** them. Vexera comes with these commands too. To kick a user from your guild, you use `+kick <ID/Mention> [Reason]`.<br/>
To ban someone the way to go is `+ban <ID/Mention> [Time] [Reason]`. So for example to ban the user `luke#0123` 10 minutes, you would use `+ban luke#0123 10m Annoying staff`. To kick `luke#0123` you would use `+kick luke#0123 No common sense`.<br/>
If you want your ban to be permanent, just leave out the time argument.

### Softbanning
Has someone spammed in a channel? Do you want to **remove their messages** but not to ban them yet? Then the `+softban` command is for you! A softban bans a user from your server, deletes their messages in the past seven days and immediately unbans them after.<br/>
To softban `luke#0123` you may use `+softban luke#0123 Spam` and the channel will be free from spam.

## Cleaning messages without punishing

To clean messages in a channel **without punishing** a user, like the softban does, you can use `+clean`. Using it is pretty simple.<br/>
To clean messages by a *specific user* in a channel, you use `+clean [Amount] [ID/Mention]`. If you want to clear messages by any user just leave out the User argument.

## Forcing a user to leave a voice channel

If a user is being very loud or just annoying people in a voice channel, you can use the implemented voice-kick by Vexera.<br/>
This will create a temporary voice channel, move the user into it and delete the temporary channel afterwards. This **kicks the user out of the voice channel**.<br/>
Warning: This does not stop the user from re-joining the voice channel. If they keep on annoying people, you can `+mute` them.