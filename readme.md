# Discord.js Webhook forwarder
<div align="center">
<p>
<a href="https://nodei.co/npm/djs-webhook-forwarder/"><img src="https://nodei.co/npm/djs-webhook-forwarder.png"></a>
</p>
<br />
 <p>
 <a href="https://www.npmjs.com/package/djs-webhook-forwarder"><img src="https://img.shields.io/npm/v/djs-webhook-forwarder.svg?maxAge=3600" alt="NPM version" /></a>
<a href="https://www.npmjs.com/package/djs-webhook-forwarder"><img src="https://img.shields.io/npm/dt/djs-webhook-forwarder.svg?maxAge=3600" alt="NPM downloads" /></a>
  </p>
</div>

## About 
> A simple Discord.js Webhook forwarder from a channel.


## Example
```js
const Discord = require("discord.js")
const client = new Discord.Client()
const djswebhookforwarder = require("djs-webhook-forwarder")
const webhookForwarder = new djswebhookforwarder(client, "WEBHOOK ID", "WEBHOOK TOKEN", "SOURCE CHANNEL ID")

client.on("ready", () => {
  webhookForwarder.start()
})

client.login("BOT TOKEN")
```
