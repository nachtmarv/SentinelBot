# SentinelBot
Code for the Sentinel bot we use on our discord server

### Database
I am using a mysql database for several features.
Some of them need unicode emoji support so make sure you configured your database correctly.
Here are the necessary tables:
```
EmojiBinds
  pK: int, autogenerate
  channelId: bigInt
  isUnicode: bit
  unicodeString: varchar utf8mb4
  emojiId: bigInt
  roleId: bigInt
```

```
RoleReactionAssignmentChannel
  channelId: bigInt 
```

### Config File
Run
```
cp config.txt.template config.txt
```
Edit the config.txt with your correct database string, id's and tokens.

### External Libraries
This project uses additional libraries, both of which I do not upload to github for legal reasons.
> Discord4j v2.10.0

> mysql connector java v5.1.45
