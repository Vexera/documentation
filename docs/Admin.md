# Administration / Moderation  
Vexera supplies you with many **moderation- and admin-commands**. Useful for managing *high-traffic-guilds* or just to *punish* people much *easier*.

## Punishing Users 

You got a **large range of commands to punish people**. Here, we will show and describe all of them.

### Warning
You can **warn** people by using `+warn <ID/Mention> [Reason]`
E.g. to warn the user `luke#0123` for misleading content, you may run `+warn luke#0123 Misleading Content`

### Muting
You can **mute** people permanently or temporarily by using `+mute <ID/Mention> [Time] [Reason]`
As example, you would mute the user `luke#0123` for one week and 2 days by using `+mute luke#0123 1w2d Spamming`
If you want your mute to be permanently just leave out the time argument.
The muted role is created and set after the first mute has been issued. If you are having problems with the role, feel free to delete it in your server settings and mute someone afterwards so the roles is re-created. 

### Kicking / Banning
If a user keeps violating the rules, you may want to **kick** or **ban** them. Vexera comes with these commands too. To kick a user from your guild, you run `+kick <ID/Mention> [Reason]`.
To ban someone the way to go is `+ban <ID/Mention> [Time] [Reason]`. So as example to ban the user 'luke#0123' for 10 minutes, you would do `+ban luke#0123 10m Annoying staff`. To kick `luke#0123` you would use `+kick luke#0123 No common sense`.
If you want your ban to be permanently just leave out the time argument.

### Softbanning
Someone has spammed in a channel and you want to **remove their messages** but not to ban them yet? Then `+softban` is for you! The softban bans a user from your server, deletes the messages in the past seven days and immediately unbans them after. 
To softban `luke#0123` you may run `+softban luke#0123 Spam` and the channel will be free from spam.

## Infractions
Every punishment is logged in our database, so you can access them either by setting up a mod-log by using `+modlog [channel]` and searching in it or per user by `+infractions [ID/Mention].
Pretty useful if you want to check, that someone **may stood out negatively in the past** already.

## Cleaning messages without punishing

To clean messages in a channel **without punishing** a user, like the softban does, you can use `+clean` Using it is pretty simple.
To clean messages by a *specific user* in a channel, you run `+clean [Amount] [ID/Mention], if you want to clear messages by any user just leave out the User argument.

## Forcing a user to leave a voice-channel

If a user screams very loud or is just annoying people in a voice-channel, you can use the implemented voice-kick by Vexera.
This will create a temporary voice-channel, move the user into it and delete the temporary channel afterwards. This **kicks the user out of the voice-channel**.
Warning: The user will still be able to join the voice-channel which he got kicked out. You could `+mute` them if they keep on annoying people.
