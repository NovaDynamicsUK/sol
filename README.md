![Logo](https://github.com/NovaDynamicsUK/.github/blob/main/media/Nova_large.png?raw=true)

# Sol
**Evolve - Secure - Inspire**

Moderation bot designed to enhance community management on Discord. With features tailored for effective oversight and user engagement, Solstice ensures a safe and enjoyable environment for all members with multi-server automated moderation through a federated-servers database.

## Features

- **Profanity Filtering**: Sol monitors messages in real-time and automatically deletes messages containing profanity or other flagged words and phrases. Users receive a private message notifying them of the infraction allowing them to revise their message. Support for whole-word matching ensures that only explicit terms are flagged, preventing false positives (e.g., "Ike" won't be flagged in "Strike").
- **Ban Tracking**: Automatically fetches and logs user bans from all guilds that the bot is a member of. Storing user warnings in a SQLite database for easy retrieval and moderation actions to better protect your server, on your terms automatically in most cases.
- **AI Interaction**: Sol uses a trained neural network to provide intelligent responses to user queries. Users can interact with Sol directly by mentioning the bot and asking questions or making requests. Whether that's in the guild it's a part of, or through direct messages with Sol.
- **ARC checks**: ARC's also known as "Age Restricted Channels" (NSFW Channels typically) if a channel is ARC'd Sol will use a much more relaxed profanity filtering system.

## Commands

- **Record**: `/record {user}` will pull up the database record for the specified user. You do not need a role requirement to use this command. Once a user has 3 strikes, they'll be blacklisted.
- **Blacklist**: `/blacklist {user}` will check if a given user has been blacklisted. This means they've been banned in multiple servers or have reached 3 strikes across 3 independent servers. You do not need a role requirement to use this command.

![image](https://github.com/user-attachments/assets/c0bb9281-680b-4145-93e5-93d0cf79e053)

- **Strike**: `/strike {user} {reason}` will add a strike against a user to the database record. One strike to a user per server to avoid abuse. You need a 'moderator' role to use this command.
- **Unstrike**: `/unstrike {user} {agent_id}` will remove a strike against a user to the database record. You must have the original issuers agent_id. You need a 'administrator' role to use this command or contact us to carry this out for you.
- **Tag**: `/tag {user}` will remove all roles on a specified user, then 'tags' them based on strikes in the database. This is in beta and is a great way to soft-ban a user in your server. You need a 'moderator' role to use this command.
- **Enforce** `/enforce` will bans or unbans users based on strikes across the blacklist database. If a user has joined it, they'll be banned. If they are no longer in it, they'll be unbanned. You need a 'administrator' role to use this command.
- **Mimic** `/mimic {channel} {message}` sends a message to any channel in the server through Sol. You need a 'moderator' role to use this command.

![image](https://github.com/user-attachments/assets/7c9fb7d8-07eb-4478-9fd1-d3ea0c2b1ab9)

- **Embed** `/embed {args}` sends an embed to any channel in the server through Sol. You need a 'moderator' role to use this command.

![image](https://github.com/user-attachments/assets/60ba6801-5fc8-4c89-a3a3-7b9f13497529)

- **Uptime** `/uptime` will let you know how long Sol has been up for. You do not need a role requirement to use this command.

## Get Sol

Invite Sol [here](https://discord.com/oauth2/authorize?client_id=1299139751789592628&permissions=1495721574038&integration_type=0&scope=bot). You will need a role assigned to yourself that fulfils an 'administrator' or 'moderator' requirement.
For example a role named `KC` or `Mod`/`Moderator` for moderator level commands, or `KC+`, `Admin`/`Administrator` for adminstrator level commands. **This will be simplified in later releases**.

## Contact Us

Want to learn more or get involved? Feel free to reach out:

- **Website**: [novacrew.uk](https://NovaCrew.uk)
- **Discord**: [Join here](https://discord.gg/xP5rCFn2Ep)
