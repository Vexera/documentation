# Music

Vexera provides a **feature-rich music system** so you can **play music** in the voice channels of your discord server and enjoy music *alone* or with *friends*.

## Getting started with music

1. Join a voice channel in a server which you have <a href="/invite">Vexera</a> in.
2. Use the command `+play <songname/url>` e.g `!play marble soda`
3. Vexera will join the voice channel and start playing your music.
4. Queue up additional music using `+play`!

### Searching a song
If Vexera adds an incorrect song to the queue, you can either copy the song's URL and `+play` it, or you try to use `+search <query>` to be able to select a song out of the first five YouTube-results. Just write the number of the wished song after issueing the command.  

### Music sources
Vexera can play music from Youtube, Soundcloud, Bandcamp, Twitch, Vimeo and Mixer. With Vexera-Premium you are able to play a song from a custom url, as example `+play https://example.com/files/BrainPower.mp3`.

## Viewing the queue

You can view the queue by running `+queue`, if your queue has multiple pages, you can view them by doing `+queue <page>`.
The queue can hold up to 2000 songs, if you have reached this limit you may want to clear the queue by doing `+clear`.
If you want to get some info about the currently playing song, run `+np`.

### Advanced queue control

1. If you want to **randomize** the current song-order, you may feel free to run `+shuffle` to shuffle all songs, which are currently in the queue.
2. You are tired of using `+play` to replay a song over and over again? You can either use `+repeat one` to **repeat** the currently playing song or `+repeat all` to repeat the whole queue. To disable that, do `+repeat off`.
3. You added a *wrong song* to your queue? Check the queue ID in `+queue` and do `+delete <queue-id>` to **delete** the specific song.
4. You want to play the *last played* song once **again**? Use `+back` for doing that. 
5. You want to get to a **specific point** in the queue? Check the queue ID in `+queue` and use `+jump <queue-ID>` to start playing that song!

## Pausing / Resuming music

If you don't want the bot to disconnnect from your channel, but be paused for a while, do `+pause` to pause the currently playing song. If you want Vexera to continue playing, do `+resume` to resume the song.

## Skipping music

Users can skip music by running `+skip`, if there are multiple users in the voice channel, it will initialize a voteskip. This can be overridden with the `music.forceskip` permission.

## Switching the voice-node

Vexera uses the node, which it thinks it best for you, but if you are experiencing bad streaming quality, you may want to switch the voice-region manually by using `+join us` for United States or `+join eu` for Europe. With Vexera-Premium you are also able to run `+join premium` to connect to the premium-node. This is the default node if you bought premium.

## Managing dumps / playlists [Premium]
To create a playlist, which will copy the songs currently in the queue use `+playlist create <name>`, to load the queue afterwards use `+playlist load <name>` and finally, to delete it use ``+playlist delete <name>`.

### Sharing playlists
To share a with `+playlist` created playlist, do `+playlist share <name>`- This will generate a *paste.vexera.io* link which you can share with your friends. To play this dump, use `+play <url>`.


## Stopping music

To stop Vexera from playing music and disconnecting it from the channel, you may want to run `+stop` at any time. This will not clear the queue!

### Resuming after `+stop`
You can either use `+join` to summon Vexera into the currently connected channel or `+play <songname/url>` something to resume the queue after the bot has been stopped.


## Advanced music control

1. To get to a specific time in a song, use `+seek`, e.g. `+seek 2m10s` will resume playing from two minutes and ten seconds, this also works with hours.
2. With Vexera-Premium you can control the volume of your currently playing song in Vexera's end by using `+volume <2-150>`.
