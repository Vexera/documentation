# Permissions
To control what can be used on Vexera, we offer an advanced permissions system so you can decide who can do what on your server.

## Permission Nodes

A permission node represents a single command or a whole category of commands. Examples:

- `music.play` - The 'play' command.
- `music.*` - Every command in the 'music' category.
- `*` - Every command on the bot. Use with caution.

A permission node can be:

- **Allowed**: The command(s) can be used. e.g `admin.vckick`.
- **Denied**: The command(s) cannot be used. A denied permission is handled internally as `-music.play`.
- **Neutral**: No override has been set.

## Where can I find all the permission nodes?

You can either get a list within discord by doing `+perms nodes` or by visiting the [commands page](/commands).

## How do I use permissions?

Permissions can be controled by using [Vexera's web dashboard](/auth), or within Discord by running `+perms`.