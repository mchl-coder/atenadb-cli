# Atena CLI

![Atena CLI](Atena%20CLI.png "Atena Logo")

### The official CLI of Atena DB.

Atena-CLI is the Atena command line interface. It allows to send commands and queries to Atena and read the replies sent by the server, directly from the terminal.
Thanks to Atena-CLI you will be able to manage and easily use your Atena installation. We reccomend spending some times to familiarize with it in order to work more effectivly with Atena once you know all the tricks of its command line interface.

Atena has a number of commands and sometimes, as you test things, you may not remember the exact command. Atena-CLI provides help for commands use, using the `help` command.

> 💡: Remember, Atena CLI default connects to AtenaDb server at localhost:5001. This choice is for security reasons. It is meant to prevent "accidentally" running commands and taking control of others AtenaDb. (If their owners haven’t changed their Admin default password)

## Atena commands

By typing `help` you'll get all commands:

```console
Atena> help

User and DB Management      (These commands are available only when there are no db selected)

New User        syntax: newuser username password
Change Password syntax: changepsw newPassword newPassword
New Db          syntax: newdb dbName
Delete Db       syntax: deletedb dbName
Select Db       syntax: selectdb dbName


DB Operation                (These commands are available only after you selected a DB)

Set             syntax: set key : value
Get             syntax: get key
Modify          syntax: mod key : value
Increment       syntax: incr key : increment
Delete          syntax: del key
RemoveAll       syntax: removeall
Quit            syntax: quit


General commands             (Always available)

Current User    syntax: cu
DB Name         syntax: dbname
Logout          syntax: logout
Exit            syntax: exit
Clear           syntax: clear
Help            syntax: help
```

AtenaDb will drive you through complex commands step by step.


> 💡: Use Atena-CLI to learn how Atena DB works and master it.

## Security

Atena-CLI is secure :lock:

In order to communicate with Atena DB it uses the TLS encryption with HTTP2 using the default `https` provided by Atena DB Client Library.

## Releasing

Releases are built by manteiners.

Atena-CLI is cross-platform and is available in:

* Windows   :+1:
* Linux     :+1:
* macOS     :+1:
* ARM       :+1:

## Installation

1. Download the pre-compiled version of Atena-CLI compatible with you system from the Release section of Github AtenaCLI repo. 
2. Then simply run it.
3. Congratulation Atena CLi is set up 🎉

> ⚠️ RECOMMENDATION: Once you have logged in, change your default Admin password immediately.

### Requirements:

:white_check_mark: Atena DB: up and running 

## Next Features - Coming Soon :dart:

- Atena-CLI for the new Atena DDB, when Atena DB will turn distributed.
