## Welcome to discmds.js

A simple package for making the use of discord.js easier than ever!

### What it has?
- it has events like discord.js but it have some other events that discord.js don't have and it will make discord.js coding easier!

### Example
```js
const discord = require("discord.js")
const client = new discord.Clienr()
const discmd = require("discmds.js")
const dis = new discmd(client)

client.on("ready", async () => {
await dis.eventLoad() //Must be there to load events!
})

client.login("token")
```

#### Event 1 [msgCreate] 
Like you are creating message event using discord.js you can use discmds.js for creating this event!
```js
dis.on('msgCreate', async message => {
message.channel.send("hi") //discord.js sending
dis.createMsg(message.channel.id, "hi") //discord.js + discmds.js
//If you also want to send a attachment with message do dis.createMsg(channeid, content, filelink)
})
```

#### Event 2 [userBan] 
This event happens when someone in the server gets banned!
```js
dis.on('msgCreate', async (guild,user) => {
console.log(`${user.user.tag} got banned in ${guild.name}!`)
})
```

#### Event 3 [userUnBan] 
This event happens when someone in the server gets unbanned!
```js
dis.on('userUnBan', async  => {
console.log(`${user.id} got banned in ${guild.name}!`)
})
```

#### Event 4 [emojiAdd] 
This event happens when new emoji has been added in the server!
```js
dis.on('emojiAdd', async emoji => {
console.log(emoji.id)
})
```

#### Event 5 [emojiRemove] 
This event happens when emoji has been deleted in the server!
```js
dis.on('emojiRemove', async emoji => {
console.log(emoji.id)
})
```

#### Event 6 [emojiUpdate] 
This event happens when emoji has been updated in the server!
```js
dis.on('emojiUpdate', async  => {
console.log(emoji.id)
})
```

#### Event 7 [guildMemberJoin] 
This event happens when new members joins the server!
```js
dis.on('guildMemberJoin', async member => {
console.log(member.user.tag)
})
```

#### Event 8 [guildMemberLeave] 
This event happens when members leave the server!
```js
dis.on('guildMemberLeave', async member => {
console.log(member.user.tag)
})
```

#### Event 9 [guildJoin] 
This event happens when the bot join servers!
```js
dis.on('guildJoin', async guild => {
console.log(guild.id)
})
```

#### Event 10 [guildLeave] 
This event happens when the bot leave servers!
```js
dis.on('guildLeave', async guild => {
console.log(guild.id)
})
```

#### Event 11 [msgUpdate] 
This event happens when the bot join servers!
```js
dis.on('guildJoin', async (oldMessage, newMessage) => {
console.log(newMessage.id)
})
```

#### Event 12 [msgDelete] 
This event happens when the bot join servers!
```js
dis.on('msgDelete', async message => {
console.log(newMessage.id)
})
```
