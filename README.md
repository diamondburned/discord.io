
<p align="center"><img src="http://i.imgur.com/kFzW7Uo.png"></p>
<h1 align="center">discord.io</h1>

A small, single-file, fully featured [Discordapp](https://discordapp.com) library for browsers.

# File modified to only support web browser!

`npm install https://github.com/diamondburned/discord.io/tarball/master`

#### Example
```javascript
var Discord = require('discord.io');

var bot = new Discord.Client({
    token: "",
    autorun: true
});

bot.on('ready', function() {
    console.log('Logged in as %s - %s\n', bot.username, bot.id);
});

bot.on('message', function(user, userID, channelID, message, event) {
    if (message === "ping") {
        bot.sendMessage({
            to: channelID,
            message: "pong"
        });
    }
});
```
