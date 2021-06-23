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
dis.on('msgCreate', async message => {
message.channel.send("hi") //discord.js sending
dis.createMsg(message.channel.id, "hi") //discord.js + discmds.js
//If you also want to send a attachment with message do dis.createMsg(channeid, content, filelink)
})
```



For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/discmds/discmds/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
