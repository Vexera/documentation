# Frequently Asked Questions (FAQ)
Do you have an important question? Check out our FAQ below. If you still need support after reading through the FAQ, feel free to contact us on our <a href="https://discord.gg/VzbRGWF" target="_blank">Discord</a>.

## Table of Contents:

* [General issues](#general-issues)
    * [Why do I see empty messages?](#why-do-i-see-empty-messages)
    * [Vexera is not responding to my commands](#vexera-is-not-responding-to-my-commands)
    * [Where, why and how to donate?](#where-why-and-how-to-donate)
* [Music issues](#music-issues)
    * [Vexera is not joining my voice channel](#vexera-is-not-joining-my-voice-channel)
    * [Vexera is saying "Voice Connection Timeout"](#vexera-is-saying-voice-connection-timeout)
    * [Vexera is in a voice channel but is not playing anything](#vexera-is-in-a-voice-channel-but-is-not-playing-anything)
* [Admin issues](#admin-issues)
    * [Some admin features do not work](#some-admin-features-do-not-work)
    * [How do you use +autorole?](#how-do-you-use-autorole)
    * [How can I let my friends use commands they do not have permission to?](#how-can-i-let-my-friends-use-commands-they-do-not-have-permission-to)
    * [How do I limit Vexera to a specific role?](#how-do-I-limit-vexera-to-a-specific-role)

## General issues

### Why do I see empty messages?
This is a client-side problem. Please check if **Link Preview** is enabled.<br/>
To check, go to *User Settings* -> *Text & Images* -> *Link Preview*.<br/>
Enable **Show website preview info from links pasted into chat.**.<br/>
You should now be able to see embed messages.

### Vexera is not responding to my commands
First of all, you should check if Vexera has permission to view the text channel you are using for bot commands.<br/>
If this seems to work, try `+channeltoggle`. Commands might have been disabled in the channel.<br/>
If that still does not work, try resetting the prefix to its default (`+`) by doing `@Vexera#8487 prefix disable`.<br/>
Last but not least you should check if you used an `+accessrole` to only allow one role to use the bot. If so, add the role to yourself and do `+accessrole disable`.<br/>
Owners bypass all permissions for Vexera and can use `+accessrole disable` without adding the role to themselves first.

### Where, why and how to donate?
If you subscribe for $3/month via <a href="https://www.patreon.com/bePatron?c=703870&rid=1291630" target="_blank">Patreon</a>, you get access to all the premium features.<br/>
Alternatively, you can make a one-time purchase on <a href="https://selly.gg/u/vexera" target="_blank">Selly</a>.<br/>
**Important information:** You get the features on every server you **own**!

## Music issues

### Vexera is not joining my voice channel
First, you should take a look at the channel- and role-permissions of Vexera. Make sure Vexera has permission to join the voice channel and also speak in it.<br/>
You should also check if the link you entered is **valid**. The bot only accepts YouTube, Twitch, SoundCloud and Mixer links.<br/>
Additionally, premium members are able to use **HTTP streams**. Want to know more about premium perks? [Click here](https://vexera.io/premium).

### Vexera is saying "Voice Connection Timeout"
Try kicking Vexera out of the voice channel by using `+vckick @Vexera#8487` to reset the voice connection.<br/>
If that doesn't work, switch the region the bot is connected to: `+join eu` if you're on the **US** node, `+join us` if you're on the **EU** node. If you are a premium user you can also do `+join premium`.<br/>
To check what voice node you are on, look at the bottom of the last *Now Playing* message. Alternatively, Vexera uses the node, which is closest to your server voice region.<br/>
When you're all done, play music again.

### Vexera is in a voice channel but is not playing anything
You're most likely experiencing the ["Voice Connection Timeout"](#vexera-is-saying-voice-connection-timeout) issue.<br/>
Try kicking Vexera out of the voice channel by using `+vckick @Vexera#8487` to reset the voice connection.<br/>
If that doesn't work, switch the region the bot is connected to: `+join eu` if you're on the **US** node, `+join us` if you're on the **EU** node. If you are a premium user you can also do `+join premium`.<br/>
To check what voice node you are on, look at the bottom of the last *Now Playing* message. Alternatively, Vexera uses the node, which is closest to your server voice region.<br/>
When you're all done, play music again.

## Admin issues

### Some admin features do not work
If for example the `+ban` command does not work, you should check Vexera's role- and channel-permissions.<br/>
In general, we **recommend** you to give Vexera the `Administrator` permission. This way, everything should work as intended.<br/>
Second, check if the highest role of Vexera is above the highest role of the target user.

### How do you use +autorole?
For information about autorole, please visit our [documentation about Autoroles](/docs/autorole).

### How can I let my friends use commands they do not have permission to?
For information about permissions, please visit our [documentation about Permissions](/docs/permissions).

### How do I limit Vexera to a specific role?
First, setup a role, if there is not already one.<br/>
Then, assign the role to people you want to be able to use Vexera.<br/>
Finally, execute the command `+accessrole <rolename>`.<br/>
**Note:** If you want to disable the accessrole, use `+accessrole disable`.<br/>
If you locked yourself out, assign the role to yourself, which has been used for `+accessrole`.