# Music

Vexera provides a feature-rich music system so you can play music in the voice channels of your discord server.

## Getting started with music

1. Join a voice channel in a server which you have <a href="/invite">Vexera</a> in.
2. Use the command `+play <songname/url>` e.g `!play marble soda`
3. Vexera will join the voice channel and start playing your music.
4. Queue up additional music using `+play`!

### Music sources
Vexera can play music from Youtube, Soundcloud, Bandcamp, Twitch, Vimeo and Mixer.

## Viewing the queue

You can view the queue by running `+queue`, if your queue has multiple pages, you can view them by doing `+queue <page>`.

## Skipping music

Users can skip music by running `+skip`, if there are multiple users in the voice channel, it will initialize a voteskip. This can be overridden with the `music.forceskip` permission.

## Stopping music

`+stop`