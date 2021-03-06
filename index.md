## Welcome to discmds.js

A simple package for making the use of discord.js easier than ever!

## Join our discord Server!
- https://discord.gg/jjNkZGyGbK

### What it has?
- it has events like discord.js but it have some other events that discord.js don't have and it will make discord.js coding easier!

### Example
```js
const discord = require("discord.js")
const client = new discord.Client()
const discmd = require("discmds.js")
const dis = new discmd(client)

client.on("ready", async () => {
await dis.eventLoad() //Must be there to load events!
})

client.login("token")
```

# Events

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
dis.on('userBan', async (guild,user) => {
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
dis.on('msgUpdate', async (oldMessage, newMessage) => {
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

#### Event 13 [guildMemberNicknameUpdate]
This event happens when someones nickname updates
```js
dis.on("guildMemberNicknameUpdate", (newMember, oldNick, newNick) => {
    console.log(oldNick, newNick)
})
```

#### Event 14 [userAvatarUpdate]
```js
dis.on("userAvatarUpdate", (newUser, oldAvatar, newAvatar) => {})
```

#### Event 15 [userUsernameUpdate]
```js
dis.on("userUsernameUpdate", (newUser, oldUsername, newUsername) => {})
```

#### Event 16 [userDiscriminatorUpdate]
```js
dis.on("userDiscriminatorUpdate", (newUser, oldDiscrim, newDiscim) => {})
```

#### Event 17 [userFlagsUpdate]
```js
dis.on("userFlagsUpdate", (newUser, oldFlags, newFlags) => {})
```

#### Event 18 [rolePositionUpdate]
```js
dis.on("rolePositionUpdate", (newRole, oldPosition, newPosition) => {})
```

#### Event 19 [rolePermissionsUpdate]
```js
dis.on("rolePermissionsUpdate", (newRole, oldPermission, newPermission) => {})
```

#### Event 20 [guildRegionUpdate]
```js
dis.on("guildRegionUpdate", (newGuild, oldRegion, newRegion) => {
    console.log(oldRegion, newRegion)
})
```

#### Event 21 [guildAfkChannelUpdate]
```js
dis.on("guildAfkChannelUpdate", (newGuild, oldAfkChannel, newAfkChannel) => {})
```

#### Event 22 [guildVanityURLUpdate]
```js
dis.on("guildVanityURLUpdate", (newGuild, oldVanity, newVanity) => {})
```

#### Event 23 [guildAcronymUpdate]
```js
dis.on("guildAcronymUpdate", (newGuild, oldAcronym, newArconym) => {})
```

#### Event 24 [guildOwnerUpdate]
```js
dis.on("guildOwnerUpdate", (newGuild, oldOwner, newOwner) => {})
```

#### Event 25 [guildVanityURLUpdate]
```js
dis.on("guildVanityURLUpdate", (newGuild, oldVanity, newVanity) => {})
```

#### Event 26 [guildMaximumMembersUpdate]
```js
dis.on("guildMaximumMembersUpdate", (newGuild, oldMaxMembers, newMaxMembers) => {})
```

#### Event 27 [guildPartnerUpdate]
```js
dis.on("guildPartnerUpdate", (newGuild, oldPartner, newPartner) => {})
```

#### Event 28 [guildVerifyUpdate]
```js
dis.on("guildVerifyUpdate", (newGuild, oldVerified, newVerified) => {})
```

#### Event 29 [roleCreate]
```js
dis.on("roleCreate", role => {
console.log(role.id)
})
```

#### Event 29 [roleDelete]
```js
dis.on("roleDelete", role => {
console.log(role.id)
})
```

#### Event 30 [channelUpdate]
```js
dis.on("channelUpdate", (oldChannel, newChannel) => {})
```

# Functions

#### Function 1 [eventLoad] 
For creating a message!
```js
dis.createMsg(channelid, messagetosend, filelink not important)
```

#### Function 2 [createMsg] 
For creating a message!
```js
dis.createMsg(channelid, messagetosend, filelink not important)
```
