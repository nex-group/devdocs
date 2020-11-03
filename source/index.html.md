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

> You will see the Javascript code references on this side. Notes like this one will also be present.

Wwlcome to nexOS Documentation! Here you can find resources regarding nexOS. 

# Information

<aside class="warning">
This section of the Documentation is not complete.
</aside>

> Currently, the nexOS project is closed-source. Information regarding the project will be added here later. 

# Modules 
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
Your code here!
```
> Executors are your own code. Your code matters!

Modules are necessary for code to function, it is typically divided into three sections. Initiators, Executors, and Importers.
Modules make it easier for you to code instead of relying on one single main.js file. 


# Managers
## Dependancy Manager

The Dependancy Manager is what manages Modules, Extentions, and Errors.

## Update Manager

The Update Manager will update nexOS to the latest version.

## Security Manager

<aside class="warning">
The Security Manager is incomplete and is being worked on.
</aside>

Protection of assets and manages the Security Module which allows for moderation commands.

##

Managers help nexOS stay afloat. You can learn more about the different types of Managers here! Optional Managers are called Extentions. Learn more about them in the next section.

# Extentions

## Extention-Core

Manages all centeral extention systems.

## Circuit Extention

Flow control of usage.

## HTTPS Extention

Registers HTTPS in nexOS.

Extentions are essentialy Managers however, extentions are optional.


# License

BSD 2-Clause License

Copyright (c) 2020, Friendsy, 
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

Currently nexOS is not open source, so this license does not apply yet.

However, any unauthorized cloning of the repository must retain this License.

# Legal 

Unifiton reserves a right to review all nexOS data for diagnostical purposes.

You can view the full legal section on the [Unifiton Website.](https://unifiton.ddns.net)



