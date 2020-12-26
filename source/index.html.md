---
title: nexOS Developer References

language_tabs: # must be one of https://git.io/vQNgJ
  - javascript

toc_footers:
  - <a href='https://github.com/slatedocs/slate'>Powered with Slate.</a>
  - <a href='https://github.com/unifiton/documentation'>Contribute to the documentation!</a>

includes:
  - errors

search: true

code_clipboard: true
---

# Introduction

<aside class="info">
nexOS Developer References are not complete. This should not be relied on for up-to-date information.
</aside>

> You'll see references on this side.

Wwlcome to nexOS Documentation! Here you can find resources regarding nexOS. 

# Information

nexOS is a bot that aims to be extendable.

# Modules 

Modules are necessary for code to function, it is typically divided into three sections. Initiators, Executors, and Importers.
Modules make it easier for you to code instead of relying on one long file.

## Initiators

Initiators tell 'main.js,' to list your command in the index, otherwise known by its command "ne.help" or by its manager alias, Dependancy Manager.

```javascript
module.exports = {
	name: 'title',
	description: 'more about this in the next section',
	execute(message, args) {
		// your code here - this is called the executor 
	},
};
```
In an Initiator, you have optional stacks.



> The above is an example of an initiator, and an executor. 

## Importers 

An importer imports the required definitions of your code when necessary. You typically won't need an importer.
Importers are always above the Initiator.

```javascript
const https = require('https');
const Discord = require('discord.js');
const url = 'https://www.reddit.com/r/animemes/hot/.json?limit=100'
```
> Above is an example of an importer, (Specifically a HTTPS protocol importer.) 

## Executors


```
Your code here!
```
> Executors are your own code. Your code matters!


## Info

Initiators, Importers, Executors, and your own code make up a Module.

```javascript
const https = require('https');
const Discord = require('discord.js');
const url = 'https://www.reddit.com/r/animemes/hot/.json?limit=100'
module.exports = {
	name: 'title',
	description: 'more about this in the next section',
	execute(message, args) {
		Your code here!
	},
};
```
# Stacks
Stacks are added to a Initiator when necessary.

## Guild Only Stack
Makes module only function when used in a Guild.

```javascript
guildOnly: true,
```

## Args On Stack
Enables or Disables Args.

```javascript
execute(message, args) {
```

## Command Aliases Stack
Allows for multiple starter sequences after prefix. 
<aside class="warning">
This does not change the Prefix of nexOS and does not allow for clients to set a custom-prefix.
</aside>

```javascript
aliases: ['icon', 'pfp'],
```

## Cooldown Stack
The amount of seconds the client has to wait until another response can be given.

```javascript
cooldown: 5,
```
# Dependancies 
nexOS provides multiple dependancies ready to use when making modules. This list outlines the dependancy, its expected usage, and how to use it.

**List of Modules avaliable for use.**

- discord.js (Core)
- asynckit (Asynchronous Code)
- mime-db (Media Type Database)
- node-fetch (Rest-API, HTTP)
- prism-media (Transcode Media with node.js)

# nexOS/Packager

nexOS Packager is a multipurpose, public module usage service.
<aside class="warning">
You should **never** put access tokens, or access id's, in the Packager service. **Doing so can compromise those tokens/id's, as anyone can publicly access the Packager DB Tables.
</aside>
You can view the full legal section on the [Unifiton Website.](https://unifiton.ddns.net)



