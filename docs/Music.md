# Music
Vexera provides a **feature-rich music system** so you can **play music** in the voice channels of your Discord server and enjoy high-quality music.

## Getting started
1. Join a voice channel in a server that has <a href="/invite">Vexera</a> in.
2. Use the command `+play <song name/URL>` e.g `!play marble soda`
3. Vexera will join the voice channel and start playing your music.
4. Queue up additional music using the `+play` command again!

### Searching a song
If Vexera adds an incorrect song to the queue, you can either copy the correct song's URL and `+play` it, or you can try to use `+search <query>` to be able to select a song out of the first five YouTube results. Just write the number of the wished song after issuing the command.  

### Music sources
Vexera can play music from YouTube, Spotify, SoundCloud, Bandcamp, Twitch, Vimeo and Mixer. The Spotify integration is only available with Vexera Premium. You can play singles, EPs and playlists. Please note that Spotify songs get played through YouTube and not through Spotify itself. You may hear a slightly or completely different version than expected. Additionally, albums are not yet supported but will be in the near future. As a Vexera Premium user you are also able to play a song from a custom url, for example `+play https://example.com/files/BrainPower.mp3`.

## Viewing the queue
You can view the queue by running `+queue`. If your queue has multiple pages, you can view them by doing `+queue <page>`.<br/>
The queue can hold up to 2000 songs. If you have reached this limit you may want to clear the queue by doing `+clear`.<br/>
If you want to get some information about the currently playing song, run `+np`.

### Advanced queue control
1. If you want to **randomize** the current song order, you may feel free to run `+shuffle` to shuffle all songs which are currently in the queue.
2. You are tired of using `+play` to replay a song over and over again? You can either use `+repeat one` to repeat the **currently playing** song or `+repeat all` to repeat the **whole queue**. To disable that, do `+repeat off`.
3. You added a *wrong song* to your queue? Check the position in `+queue` and do `+delete <position>` to **delete** the specific song.
4. You want to play the *last played* song once **again**? Use `+back` for doing that. 
5. You want to get to a **specific position** in the queue? Check the position in `+queue` and use `+jump <position>` to start playing that song!
6. You want to play something while the queue is empty or finished? By using `+autoplay` you can make the bot play a file, a playlist or a livestream while the queue is empty!

## Stopping music
To stop Vexera from playing music and disconnecting it from the channel, you may want to run `+stop` at any time. This will not clear the queue!

### Resuming after `+stop`
You can either use `+join` to summon Vexera into the currently connected channel or `+play <song name/URL>` something to resume the queue after the bot has been stopped.

## Pausing / resuming music
If you don't want the bot to disconnect from your channel, but be paused for a while, use `+pause` to pause the currently playing song. If you want Vexera to continue playing, use `+resume` to resume the song.

## Skipping music
Users can skip music by running `+skip`. If there are multiple users in the voice channel, it will initialize a voteskip. This can be overridden with the `music.forceskip` permission. Read more about permissions [here](/docs/permissions).

## Switching the voice node
Vexera uses the node which it thinks suits best for you. If you are experiencing bad streaming quality, you may want to switch the voice node manually by using `+join de-voice-1` or `+join de-voice-2` depending on what voice node you are currently connected to. As a premium user, you can change to any of the two premium voice nodes with `+join de-voice-1-1` and `+join de-voice-2-1`.

## Managing dumps / playlists [Premium]
See a list of your playlists: `+playlist list`. Note that playlists are per server and only available to the user that created them.
To create a playlist, which will copy the songs currently in the queue, use `+playlist create <name>`. To load the queue afterwards, use `+playlist load <name>` and finally, to delete it, use `+playlist delete <name>`.

### Sharing playlists [Premium]
To share a playlist you created with `+playlist`, use `+playlist share <Name>`. This will generate a *paste.vexera.io* link, which you can share with your friends. To play this dump, use `+play <URL>`.

## Advanced music control
1. To get to a specific time in a song, use `+seek`, e.g. `+seek 2m10s` will resume playing from two minutes and ten seconds. The time formation also works with hours.
2. With Vexera Premium, you can control the volume of your currently playing song in Vexera's end by using `+volume <2-150>`. What's Vexera Premium and how do I get it? Read more about it [here](/premium).
3. To view the lyrics of the currently playing song, do `+lyrics` and, if you want to get the lyrics of a specific song, do `+lyrics <song name>`.