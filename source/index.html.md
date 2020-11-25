---
title: nexOS Documentation

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
The documentation for nexOS is not complete snd is constantly evolving and changing. Click "Contribute to the Documentation!" button on the sidebar to view the repository.
</aside>

> You'll see references on this side.

Wwlcome to nexOS Documentation! Here you can find resources regarding nexOS. 

# Information

<aside class="warning">
This section of the Documentation is not complete.
</aside>

> Currently, the nexOS project is closed-source. Information regarding the project will be added here later. 

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


# Extend
<aside class="warning">
Extending Capabilities are not actively worked on, information here are not guaranteed to work. 
</aside>
It's easy to extend the capabilities already provided by the backend of nexOS.





You can view the full legal section on the [Unifiton Website.](https://unifiton.ddns.net)



