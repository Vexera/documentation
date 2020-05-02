# Autorole
Not sure how the `+autorole` command works? Then you've come to the right place! You'll find everything you need down below.

## About
The `+autorole` command is for letting the bot add roles to users or bots when they join, or when members use `+getrole`.<br/>
Before we begin, here are some important notes:

* Vexera's highest role must be above the role it is trying to assign!
* The role you are trying to automate already needs to exist on your server!

## Add an autorole
Basic command: `+autorole add <type> <role>`.

### New server member joins the server (join)
To give users who join the server the *Members* role, use `+autorole add join Members`.

### New bot joins the server (bot)
To assign the *Bots* role to bots when they join, use `+autorole add bot Bots`.

### A member executes +getrole (get)
To let users get the *User* role by typing `+getrole User`, use `+autorole add get User`.

## Remove an autorole
Basic command: `+autorole remove <Yype> <Role>`.<br/>
To remove any autorole, you basically just have to replace `add` with `remove`. Do not forget the type (`join`, `bot`, `get`)!

### New server member joins the server (join)
To remove the autorole for users who join the server (in this example, the *Members* role), use `+autorole remove join Members`.

### New bot joins the server (bot)
To remove the autorole for bots who join the server (in this example, the *Bots* role), use `+autorole remove bot Bots`.

### A member executes +getrole (get)
To remove the autorole for members who use `+getrole` (in this example, the *User* role), use `+autorole remove get User`.

## List all active autoroles
You can see all active autoroles with the `+autorole list` command.