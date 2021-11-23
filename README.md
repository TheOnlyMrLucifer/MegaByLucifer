
---

## Features 💫
 - Mega accounts are not needed!
 - Uses two download engines for downloading links!
 - Speed improved with heroku and vps too!
 - Parallel downloads are supported! (This means many users can use the bot at the same time. 😇)
 - Multitasking is also supported! (This means You (owner) and telegram users who you set as auth users will be able to download multiple links at the same time! 😋)
 - Custom thumbnail support!
 - Custom caption support!
 - Ban unwanted users!
 - See your bot's user count!
 - Broadcast any message to every user of your bot!
 - Ability to download any file under 5GB! (If you provide a pro/business account when deploying there will be no file size limits! 😍)

<b>Notes</b> :- 
1. Due to telegram API limits I can't upload files which are bigger than 2GB so such files will be spliited and uploaded to you!
2. Quota limits can occur if you don't provide a pro/business account!
3. Folder support is not implemented yet but can be added in the near future!
---

## Deploying Methods

<details>
  <summary><b>Deploying to Heroku</b></summary>

<br>

- Examples of needed bot variables are mentioned below in this readme!
 
 <b>Note</b> :- Downloads are speed on heroku too! 😍

<br>
  
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/TheOnlyMrLucifer/MegaByLucifer)
</details>

<details>
  <summary><b>Deploying on a VPS</b></summary>

<br>



## Variables
- `API_ID` -  Get this value from https://my.telegram.org/apps
- `API_HASH` - Get This Value from https://my.telegram.org/apps
- `TG_BOT_TOKEN` - Make a bot from https://t.me/BotFather and enter the token here.
- `Mega_email` - This is not necessary! Enter your mega email only if you have a mega.nz account with pro/business features. (Used for downloading links with the download engine 'MEGAcmd' which is used in this repository.)
- `Mega_password` - This is not necessary! Enter your mega password only if you have a mega.nz account with pro/business features. (Used for downloading links with the download engine 'MEGAcmd' which is used in this repository.)
- `Bot_username` - Your bot's telegram username. (must enter with '@' in the front of the username.)
- `AUTH_USERS` - Id's of the telegram users, who you want to allow for multitasking - downloading multiple links at once!
- `OWNER_ID` - Your(owner's) telegram id
- `REDIS_URI` - Get This Value from http://redislabs.com/try-free (If you don't know how to obtain these values a complete video tutorial is available here:- https://t.me/botzupdate/5)
- `REDIS_PASS` - Get This Value from http://redislabs.com/try-free (If you don't know how to obtain these values a complete video tutorial is available here:- https://t.me/botzupdate/5)

---

## Bot Commands

<details>
  <summary><b>Normal User Commands</b></summary>

<br>

- `/start` - To check if the bot is alive!
- `/help` - To get the detailed help guide of using the bot!
- `/deletethumbnail` - To delete your saved custom thumbnail!
</details>

<details>
  <summary><b>Admin Commands</b></summary>

<br>

- `/mega_ini` - If you are the bot owner (who deploys the bot) and have a pro/business account; In addition to providing your mega credentials in config variables when deploying the bot, you will have to create a mega.ini file for using with the download engine 'megatools' which is used in this repository. Going through this step is essential if you are willing to avoid quota limits when downloading links!
 
<b>Create a new text file in notepad or from any other method. Copy the code shown below and paste it in your newly created text file. Replace the values with your actual credentials! Then save the file as "mega.ini"</b>

```sh  
[Login]
Username = your-mega-email-without-inverted-commas
Password = your-mega-password-without-inverted-commas

[Network]
# 1MiB/s
SpeedLimit = 0

[UI]
Colors = true
``` 

<b>Note :- In the above code change only the "Username" and the "Password" with your credentials. Keep others exactly as it is and save the file as "mega.ini"</b>
 
Now send your "mega.ini" file to your bot and as a reply to it send the command <code>/mega_ini</code> 
<br>
 
- `/black` - To ban unwanted users from the bot! <br>
(<b>Syntax of sending the commnad to the bot is</b>:- <code>/black</code> <i>userid</i>)<br>

- `/unblack` - To unban banned users from the bot! <br>
(<b>Syntax of sending the commnad to the bot is</b>:- <code>/unblack</code> <i>userid</i>)<br>
 
- `/lisblack` - To get the telegram id list of banned user's from the bot!<br>
 
- `/broadcast` - To broadcast a message to all the users of the bot! <br>
(<b>Syntax of sending the commnad to the bot is</b>:- <code>/broadcast</code> <i>as a reply to the message that you want to broadcast!</i>)<br>

- `/stats` - To get the total number of users who has used your bot!
</details>

---

### Reason for making this open source :-

<b>For the help of any guy like me in this world who is wondering how to make a bot for downloading mega links, or for whoever that is finding a code to download mega links; thought to make this public. 😇❤️</b>

---

## Credits, and Thanks to

* [megous](https://github.com/megous) for [megatools](https://megatools.megous.com)
* [mega.nz](https://mega.nz) for [MEGAcmd](https://github.com/meganz/MEGAcmd)
* [Odwyersoftware](https://github.com/odwyersoftware) for the [Python library](https://github.com/odwyersoftware/mega.py) of [mega.nz-API](https://mega.nz/API) 
* [ProThinkerGang](https://github.com/ProThinkerGang) for the database module code!
* [Anjana](https://github.com/AnjanaMadu) for various helps!
* [Dan](https://github.com/delivrance) for [pyrogram](https://github.com/Pyrogram)

<b>Project written and created by</b> - [XMYSTERIOUSX](https://github.com/XMYSTERlOUSX)

---

#### LICENSE

- GPLv3
