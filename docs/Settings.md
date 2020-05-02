# Settings & Customization
Vexera comes with a rich customization suite to provide you with the best experience.

## Setting a custom prefix
As the default prefix of Vexera is `+`, you may want to change it to something else which is **more handy for you**, like `!`.<br/>
You can do this by using `+prefix !` and after that, all commands may be ran like `!ping`.<br/>
To disable the custom prefix, do `[your prefix]prefix disable` or `@Vexera#8487 prefix disable`.

## Limiting the bot usage
You can limit the usage of the bot either by permissions [see permissions](/docs/permissions), by channels or by role.

### By channel
To deny the usage of Vexera's commands in specific channels, run `+channeltoggle` in the channels you don't want Vexera to work.<br/>
Users with either the `Administrator` Discord permission or the `vexera.disabledOverride` permission can bypass this.

### By role
**Be very careful using this feature as it could lock you out of Vexera's usage too!**  
To restrict Vexera to a specific role, such as the role `Commander`, you may run `+accessrole Commander` to do so.<br/>
Make sure you own this role too, so you can still use Vexera. To disable the accessrole just run `+accessrole disable`.<br/>
The server owner can bypass this.

## Greetings & farewells
Give users who join your server a warm welcome and/or a cold farewell.

### Greetings
To give users who join your server some basic info or just a welcome, you can set a greeting with `+greeting <channel> [text]`.<br/>
You can either post this greeting:
* In a channel, eg #general
* In direct messages (dm)
   * be warned that the user who joins the server needs to have direct messages enabled to get this message.
 
### Farewells
To say goodbye to users who left your server, do `+farewell <channel> [text]`.<br/>
So, as an example, you could do `+farewell #general Bye bye, %username%!`.<br/>
You are **not** able to use `dm` as the channel argument as Vexera isn't able to predict when a user leaves.

###### Variables
By using variables, you are able to mention the user, just display the username or display the servername.<br/>
These should be included in the text as follows:

 Variable | Used in | Usage | Display
 :--------: | :-------: | :----- | -------:
 %mention% | Greeting | +greeting #general Welcome %mention% to my server! | Welcome @luke#0123 to my server!
 %username% | Greeting & Farewell | +greeting #general Welcome %username% in my server! | Welcome luke#0123 in my server! 
 %server% | Greeting & Farewell | +greeting dm Welcome to %server%! Have fun out there! | Welcome to Vexera Official! Have fun out there!
 
## Locales
You are able to set your *personal* or *server-wide* **locale** (language) so you can always understand what Vexera is actually trying to tell you.<br/>
To view a list of available languages, do `+locale list`.

### Personal language
To set **your** language which overwrites the server-wide language, you may want to run, as an example, `+userlocale de`. This will result in all replies of Vexera globally to be in German.

### Server-wide language
To set the default language on your **server**, you may want to run as example `+locale de`. This will result in all replies of Vexera in your server to be in German.

## Logging
In Vexera you can log infractions, punishments, joins and leaves.<br/>
To set those up, you use the command `+log <action> <channel> [events]`.<br/>
The `action` argument is either `add` or `remove`, the channel is something like `#mod-log` or `#join-log` and the events are listed as follows:

Event | What it does | Usage
----- | ------------ | -------
joins | Displays recently joined users. | +log add #join-log joins
leaves | Displays recently left users. | +log add #leave-log leaves
infractions | Displays recently punished users. | +log add #infractions infractions

The events **can be bound together**, so as example `+log add #join-leaves joins leaves`.