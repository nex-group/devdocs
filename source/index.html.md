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

Wwlcome to nexOS Documentation! Here you can find resources regarding nexOS. 

# Information

<aside class="warning">
This section of the Documentation is not complete.
</aside>


# Modules 101
## Initiators

Initiators tell 'main.js,' to list your command in the index, otherwise known by its command alias, 'ne.help.' 

```javascript
module.exports = {
	name: 'title',
	description: 'more about this in the next section',
	execute(message, args) {
		// your code here - this is called the executor 
	},
};
```

> The above is an example of an initiator, and an executor. 

## Importers 

An importer imports the required definitions of your code when necessary. You typically won't need an importer.

```javascript
const https = require('https');
const Discord = require('discord.js');
const url = 'https://www.reddit.com/r/animemes/hot/.json?limit=100'
```
> Above is an example of an importer, (Specifically a HTTPS protocol importer.) 

## Executors


```
Your code!
```
> Executors are your own code. Your code matters!

Modules are necessary for code to function, it is typically divided into three sections. Initiators, Executors, and Importers.

## HTTP Request

`GET http://example.com/api/kittens`



ID | The ID of the kitten to delete

