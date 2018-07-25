# Settings & Customization
Vexera comes with a rich customization-suite to provide you with the best experience.

## Limitting the bot-usage

You can limit the usage of the bot either by permissions [see permissions](https://vexera.io/docs/permissions), by channels or by role.

### By Channels
To deny the usage of Vexera's commands in specific channels, run `+channeltoggle` in the channels you don't want Vexera to work.
Users with either the `Administrator` Discord-permission or the `vexera.disabledOverride` permission can bypass this.

### By Role
**Be very careful using this feature, as it could lock you out of Vexera's usage too!**
To restrict Vexera to a specific role, as example the role `Commander`, you may run `+accessrole Commander` to do so.
Make sure you own this role too, so you can still use Vexera. To disable the accessrole just run `+accessrole disable`
The server-owner can bypass this.

## Greetings & Farewells

Give people who join your server a warm welcome and/or a cold farewell.

### Greetings
To give people who join your server some basic info or just a welcome, you can set a greeting with `+greeting <channel> [text]`
You can either post this greeting:
* In a channel, eg #general
* In direct messages (dm)
   * be warned, that the user who joins the server needs to have direct messages enabled to get this message.

Also, using variables you are able to mention the user, just display the username or display the servername.
These should be included in the text as follows:
 Variable | Usage | Display
 -------- | ----- | -------
 %mention% | +greeting #general Welcome %mention% to my server! | Welcome @luke#0123 to my server!
 %server% | +greeting dm Welcome to %server%! Have fun out there! | Welcome to Vexera Official! Have fun out there!
 
### Farewells
