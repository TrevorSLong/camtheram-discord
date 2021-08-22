# Cam the Ram Discord Bot
This is a Python Discord bot designed to help moderate and enhance Colorado State University related servers. This bot is in no way affiliated with Colorado State University. This bot is essentially a reskin of [Robo Rick](https://github.com/TrevorSLong/Robo-Rick) (another bot I created). If you would like to add Cam the Ram to your server click [here](https://discord.com/api/oauth2/authorize?client_id=876863853940592661&permissions=8&scope=applications.commands%20bot).

# Bot events:
#### Welcome message
   * Welcomes new members into the server by name with a random welcome message related to CSU.     <br />
![WelcomeMessageImage](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/welcomemessages.PNG)
#### Welcome DM
   * Welcomes new members into the server by sending them a DM     <br />
![WelcomeDMImage](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/welcomedm.PNG)
#### Chat response
   * Responds to "cam" with the CSU Fight Song     <br />
![CamImage](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/cam.PNG)
#### Changes bot status
   * Cam the Ram's status is "Watching MECH324 Lecture"     <br />
![BotStatus](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/botstatus.PNG)
#### Join server message
   * Cam the Ram sends a message in the default channel when he joins the server for the first time introducing himself     <br />
![JoinMessage](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/joinmessage.PNG)
#### Changes usernames containing bad language when joining a server
   * Cam the Ram change a username that contains swear words to "CSU Ram"
   * The author of the message and the admin channel will get an update explaining what happened.
![ChangeNick](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/changenick.PNG)
![ChangeNick2](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/changenick2.PNG)
#### Removes messages with excessive capital letters
   * Cam the Ram will remove messages that are sent with more then 50% capital letters
   * The author of the message and the admin channel will get an update explaining what happened.
![ExcessiveCaps](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/capitals.PNG)
#### Removes messages with swear words
   * Cam the Ram will remove messages that are sent with a swear word inside
   * The author of the message and the admin channel will get an update explaining what happened.
![SwearWords](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/swearwords.PNG)
# Slash Commands:
   * Slash commands were introduced to Discord 3/24/21, they much more user-friendly because they suggest and auto-fill based on whether the expected value is a string, user, channel, etc. Below is a list of all of the slash commands:
![SlashCommand](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/slashcommand.PNG)
#### Ping
   * Responds to `/ping` with "Pong" and the server latency
![Ping](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/ping.PNG)
#### UpdateChannel
   * Changed the channel Cam the Ram sends updates to (Welcome messages, leave messages, etc.)
   * Hitting tab will autofill the command and bring up a list of channels on your server. If it doesn't see the channel in the UI just type it out.
   * Note: command and result are using a different channel
![UpdateChannel](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/updatechannel.PNG)
#### AdminChannel
   * Changed the channel Cam the Ram sends admin updates to (Kicking, banning, temp banning, etc.)
   * Hitting tab will autofill the command and bring up a list of channels on your server. If it doesn't see the channel in the UI just type it out.
   * Note: command and result are using a different channel
![AdminChannel](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/adminchannel.PNG)
#### Announcements
   * Allows a user with `Manage Server` ability to send an announcement to any channel in the server. Both a message and channel to send to are required.
   * After typing the command hit TAB to autofill the message parameter, then type your message and hit tab. It will then open a list of channels to send the announcement to.
![Announce1](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/announce1.PNG)
![Announce2](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/announce2.PNG)
#### Kick
   * `/kick member:` **@User** `reason:` **REQUIRED REASON, THE USER WILL SEE THIS REASON**
   * Kicks the user from the server, informs them of the reason. Also informs the admin channel that the person was kicked and the reason.
![Kick1](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/kick1.PNG)
![kick2](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/kick2.PNG)
#### Ban
   * `/ban member:` **@User** `reason:` **REQUIRED REASON, THE USER WILL SEE THIS REASON**
   * Bans the user from the server, informs them of the reason. Also informs the admin channel that the person was kicked and the reason.
![Ban](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/ban.PNG)
#### TempBan
   * `/tempban member:` **@User** `reason:` **REQUIRED REASON, THE USER WILL SEE THIS REASON** duration: **How long in days**
   * Temporarily bans the user from the server, informs them of the reason. Also informs the admin channel that the person was kicked and the reason.
![Announce2](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/tempban.PNG)
#### UnBan
   * **Careful with the syntax here**
   * `/unban member1234: Username#1234`
   * This command will not autofill the user, you need to type the username and number
![Unban](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/Screenshots/unban.PNG)
# Traditional ($) Commands:
I won't include any screenshots here, but the commands are exactly the same as [Robo Rick](https://github.com/TrevorSLong/Robo-Rick) so go there and read that documentation if needed.
#### Ping
   * Responds to $ping with "pong" and the bot server latency     <br />
#### UpdateChannel
   * Use $updatechannel to change the channel Cam the Ram sends all public updates
   * The channel will be changed to the channel that you send the command in
   * By default this channel will be the top text channel in the server
   * To change this permission, the user must have the "Manage Channel" permission in the Discord server     <br />
   * $checkupdatechannel can be used to check which channel in your server is set to the update channel     <br />
#### AdminChannel
   * Use $adminchannel to change the channel Cam the Ram sends all admin updates
   * The channel will be changed to the channel that you send the command in
   * By default this channel will be the top text channel in the server
   * To change this permission, the user must have the "Manage Channel" permission in the Discord server     <br />
   * $checkadminchannel can be used to check which channel in your server is set to the admin update channel     <br />
#### Announcements
   * $announce _____ will send an announcement in the updates channel in your server. To change the channel it is sent in use $updatechannel    
   * You will need the permission 'Manage Channel' to use this command
   * Announcements can be sent to a specific channel by adding the channel ID as an optional arguement
   * Example: $announce 123456789 This announcement was sent to a specific channel instead of the update channel     <br />
#### Kick
   * $kick __ __ kicks a member for a either a specified or unspecified reason
   * Sends an update in Admin channel and sends the reason in a DM to the member who was kicked
   * Example: `$kick @User#1234 because they were spamming unrelated messages in school chats ` 
#### Ban
   * $ban __ __ bans a member for a either a specified or unspecified reason
   * Sends an update in Admin channel and sends the reason in a DM to the member who was banned
   * Example: `$ban @User#1234 because they don't go to CSU and are spamming chats` 
   * If a reason is specified:
#### Unban
   * $unban unbans a user that was previously banned
   * Example: `$unban User#1234 because they were mistakenly banned` 
   * **Important**: in ban and kick use @User#1234 after the command but here use User#1234 with no @ (it will not autofill the user)
      * In the admin channel     <br />
#### Tempban
   * `$tempban User#1234 days reason` bans a user for a certain number of days for a reason and then unbans them
   * Example: `$tempban @User#1234 because they are spamming general chat` 
   * **Important**: This command is not perfect, if Cam the Ram is restarted or updated while a temporary ban is in place he will forget the ban and will not execute the unban. This is a known issue and is in the pipeline to be fixed.

#### Error handling
   * Sends an error if a member tries to use a command they do not have access to       <br />  
#### Help
   * $help is here! Type this to get a less detailed summary of what is above.       <br /> 

# Git Command
`git clone https://github.com/TrevorSLong/CamTheRam-Discord`
*  Clones entire repository
*  add `~/FOLDER/SUBFOLDER` after PROGRAM.m to clone to specific folder
   * Ex: `git clone https://github.com/TrevorSLong/CamTheRam-Discord ~/CamTheRam-Discord`
   * to clone repository to a folder in home named CamTheRam-Discord
