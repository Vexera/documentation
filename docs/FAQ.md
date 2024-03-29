# Frequently Asked Questions (FAQ)

Do you have an important question? Check out our FAQ below. If you still need support after reading through the FAQ, feel free to contact us on our <a href="https://discord.gg/VzbRGWF" target="_blank">Discord</a>.

## Table of Contents:

- [General issues](#general-issues)
  - [Why do I see empty messages?](#why-do-i-see-empty-messages)
  - [Vexera is not responding to my commands](#vexera-is-not-responding-to-my-commands)
  - [Where, why and how to get Vexera Premium/Pro?](#where-why-and-how-to-get-vexera-premium-pro)
  - [I bought Vexera Premium/Pro but the features do not work](#i-bought-vexera-premium-pro-but-the-features-do-not-work)
- [Music issues](#music-issues)
  - [Vexera is not joining my voice channel](#vexera-is-not-joining-my-voice-channel)
  - [Vexera is not playing music](#vexera-is-not-playing-music)
  - ["The queue can only hold 2000 songs!"](#quot-the-queue-can-only-hold-2000-songs-quot)
- [Admin issues](#admin-issues)
  - [Why are some admin features not working?](#why-are-some-admin-features-not-working)
  - [How do you use +autorole?](#how-do-you-use-autorole)
  - [How do I use the built-in permission system?](#how-do-i-use-the-built-in-permission-system)
  - [How do I limit Vexera to a specific role?](#how-do-i-limit-vexera-to-a-specific-role)

## General issues

### Why do I see empty messages?

This is a client-side problem. Please check if **Link Preview** is enabled.<br/>
To check, go to _User Settings_ -> _Text & Images_ -> _Link Preview_.<br/>
Enable **Show website preview info from links pasted into chat**.<br/>
You should now be able to see embed messages.

### Vexera is not responding to my commands

First of all, you should check if Vexera has permission to view the text channel you are using for bot commands.<br/>
If that is valid, try `+channeltoggle`. Commands might have been disabled in the channel.<br/>
If that still does not work, try resetting the prefix to its default (`+`) by doing `@Vexera#8487 prefix disable`.<br/>
Last but not least, you should check if you used an `+accessrole` to only allow one role to use the bot. If so, add the role to yourself and do `+accessrole disable`.<br/>
Owners bypass all permissions for Vexera and can use `+accessrole disable` without adding the role to themselves first.

### Where, why and how to get Vexera Premium/Pro?

If you subscribe for $3/month via Patreon, you get access to all the premium features.<br/>
If you subscribe for $5/month however, you get access to all premium features **and** Vexera Pro. This way you can have two Vexeras in your server!<br/>
**Important information:** You get the features on every server you **own**!<br/>
You can find our Patreon [here](https://www.patreon.com/bePatron?c=703870&rid=1291630)!

### I bought Vexera Premium/Pro but the features do not work

Please make sure you actually **own** the server. The `Administrator` permission is not enough to activate premium on your server. To check if you are the owner of the server, you can go to _Server Settings_ → _Members_ and search for your name. If you have a crown next to your name, you are the owner of the server. There can only be a **single** owner.<br/>
You can transfer your subscription to the server owner in order to activate premium features by using `+transfer @serverowner`. Replace `@serverowner` with the mention of the server owner.<br/>
**Note that this will transfer all perks to this server owner and you will lose access to Vexera Premium on any other servers you own.**<br/>
Also, make sure you linked your Discord account with your Patreon account. This can be done on Patreon's website.<br/>
A similar issue could be that you bought Vexera Premium, or linked your account, in the last few minutes. Please allow up to **five** minutes until Vexera Premium is available to you.

## Music issues

**This is a step-by-step guide to resolve most music issues:**

1. Try changing your server region to something other than Europe.
2. Use `​+stop`​, then `​+join de-voice-1`​
3. Use `​+stop`​, then `​+join de-voice-2`​
4. Try changing your server region again. After this, repeat step 2 or 3.
5. Clear your queue with `​+clear`​. After you have cleared the queue, repeat steps 1 to 3.

**If you are a premium user, please use the following guide instead:**

1. Try changing your server region to something other than Europe. Go to step 2/3.
2. Use `​+stop`​, then `​+join de-voice-1-1`​
3. Use `​+stop`​, then `​+join de-voice-2-1`​
4. Try changing your server region again. After this, repeat step 2 or 3.
5. Clear your queue with `​+clear`​. You can save it first by using `​+dump all`​ before clearing, I'd advise doing this only if the queue content is important. After you have cleared the queue, repeat steps 1 to 3. Copy the link from the dump command and use `​+play`​ with it to get all songs back in the queue.

### Vexera is not joining my voice channel

First, you should take a look at the channel and Vexera's permissions. Make sure Vexera has permissions to join the voice channel and also to speak in it.<br/>
You should also check if the link you entered is **valid**. The bot only accepts Twitch and SoundCloud links.<br/>
Additionally, premium members are able to use **HTTP streams** and **Spotify playlists**. Interested in Vexera Premium? You can know more about it by [clicking here](https://vexera.io/premium).

### Vexera is not playing music

Try kicking Vexera out of the voice channel by using `+vckick @Vexera#8487` to reset the voice connection.<br/>
If that doesn't work, switch the region the bot is connected to: `+join de-voice-1` or `+join de-voice-2` depending on what voice node you are currently connected to. As a premium user, you can change to any of the two premium voice nodes with `+join de-voice-1-1` and `+join de-voice-2-1`.<br/>
To check what voice node you are on, look at the bottom of the last **now playing message**.<br/>
When you're all done, play music again.

### "The queue can only hold 2000 songs!"

The queue is capable of holding up to 2000 songs. To reset the queue, use `+clear`, otherwise, you will not be able to add new songs to the queue.

## Admin issues

### Why are some admin features not working?

If, for example, the `+ban` command does not work, you should check Vexera's role and channel permissions.<br/>
In general, we **recommend** you to give Vexera the `Administrator` permission. This way, everything should work as intended.<br/>
Second, check if the highest role of Vexera is above the highest role of the target user.

### How do you use +autorole?

For information about autorole, please visit our [documentation about autoroles](/docs/autorole).

### How do I use the built-in permission system?

For information about the built-in permission system, please visit our [documentation about permissions](/docs/permissions).

### How do I limit Vexera to a specific role?

First, setup a role if there is not already one.<br/>
Then, assign the role to the users you want to be able to use Vexera.<br/>
Finally, execute the command `+accessrole <Role>`.<br/>
**Note:** the `<` and `>` are not actually used in the command.<br/>
If you want to disable the accessrole, use `+accessrole disable`.<br/>
In the case you locked yourself out, assign the role to yourself which has been used for `+accessrole`.<br/>
Owners bypass all permissions for Vexera and can use `+accessrole disable` without adding the role to themselves first.
