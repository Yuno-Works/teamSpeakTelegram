# TeamSpeakTelegram
TeamSpeakTelegram is a telegram bot that tells you who is connected to the teamspeak server to know when your friends are online. It can be used both in private and in a group chat.


## Installing
1. Install or upgrade teamSpeakTelegram from pip:
  ```
  $ pip install teamSpeakTelegram --upgrade
  ```
Or you can install from source:
  ```
  $ git clone https://github.com/jossalgon/teamSpeakTelegram.git
  $ cd teamSpeakTelegram
  $ python setup.py install
  ```

2. Create a config.ini file with:
  ```
  [Telegram]
  token_id = YOUR_TELEGRAM_BOT_TOKEN
  admin_id = YOUR_TELEGRAM_ID
  
  [TS]
  ts_host = YOUR_TS_HOST
  ts_user = serveradmin (OR YOUR TS USERNAME AS ADMIN)
  ts_pass = YOUR_TS_PASSWORD
  
  [Database]
  DB_HOST = YOUR_MYSQL_HOST
  DB_USER = YOUR_MYSQL_USER
  DB_PASS = YOUR_MYSQL_PASS
  DB_NAME = YOUR_MYSQL_DB_NAME
  ```
If you don't know your telegram id, leave it blank, start the bot and use the command /id.

3. Run the bot
  ```
  python3 -m teamSpeakTelegram
  ```

4. Invite users

  Use the command /generate to generate invitation links, the users logged with this link could use the bot.


## Commands
Command | Uses
------- | -----
/start | Reply with a welcome message
/who | Reply with the connected users
/ts | Reply with the channels and connected users
/mention | Join to receive a forwarded messsage if contains @flandas
/generate | Generate an invitation link
/id | Reply with your telegram id
/notify | Send a message with the args received from the command to all the telegram users
/users | Manage users with intuitive buttons
/groups | Manage user groups with intuitive buttons
/gm | Send a global message to your teamSpeak server


/user command                               |  User detail
:------------------------------------------:|:-------------------------------------------:
![TS command](http://imgur.com/giUiHUb.png) | ![TS command](http://imgur.com/uyjMQHz.png)

/ts command                                 |
:------------------------------------------:
![TS command](http://imgur.com/KJ41dUK.png) |