# Cam the Ram Discord Bot
This is a Python Discord bot designed to help moderate and enhance Colorado State University related servers. This bot is in no way affiliated with Colorado State University. This bot is essentially a reskin of [Robo Rick](https://github.com/TrevorSLong/Robo-Rick) (another bot I created). If you would like to add Cam the Ram to your server click [here](https://discord.com/api/oauth2/authorize?client_id=876863853940592661&permissions=8&scope=applications.commands%20bot).

# Bot events:
#### Welcome message
   * Welcomes new members into the server by name with a random welcome message related to CSU.     <br />
#### Welcome DM
   * Welcomes new members into the server by sending them a DM     <br />
#### Chat response
   * Responds to "cam" with the CSU Fight Song     <br />
#### Changes bot status
   * Cam the Ram's status is "Watching MECH324 Lecture"     <br />
#### Join server message
   * Cam the Ram sends a message in the default channel when he joins the server for the first time introducing himself     <br />
# Slash Commands:
   * Slash commands were introduced to Discord 3/24/21, they much more user-friendly because they suggest and auto-fill based on whether the expected value is a string, user, channel, etc. Below is a list of all of the slash commands:
#### Ping
   * Responds to `/ping` with "Pong" and the server latency
#### UpdateChannel
   * Changed the channel Cam the Ram sends updates to (Welcome messages, leave messages, etc.)
   * Hitting tab will autofill the command and bring up a list of channels on your server. If it doesn't see the channel in the UI just type it out.
   * Note: command and result are using a different channel
#### AdminChannel
   * Changed the channel Cam the Ram sends admin updates to (Kicking, banning, temp banning, etc.)
   * Hitting tab will autofill the command and bring up a list of channels on your server. If it doesn't see the channel in the UI just type it out.
   * Note: command and result are using a different channel
#### Announcements
   * Allows a user with `Manage Server` ability to send an announcement to any channel in the server. Both a message and channel to send to are required.
   * After typing the command hit TAB to autofill the message parameter, then type your message and hit tab. It will then open a list of channels to send the announcement to.
#### Kick
   * `/kick member:` **@User** `reason:` **REQUIRED REASON, THE USER WILL SEE THIS REASON**
   * Kicks the user from the server, informs them of the reason. Also informs the admin channel that the person was kicked and the reason.
#### Ban
   * `/ban member:` **@User** `reason:` **REQUIRED REASON, THE USER WILL SEE THIS REASON**
   * Bans the user from the server, informs them of the reason. Also informs the admin channel that the person was kicked and the reason.
#### TempBan
   * `/tempban member:` **@User** `reason:` **REQUIRED REASON, THE USER WILL SEE THIS REASON** duration: **How long in days**
   * Temporarily bans the user from the server, informs them of the reason. Also informs the admin channel that the person was kicked and the reason.
#### UnBan
   * **Careful with the syntax here**
   * `/unban member1234: Username#1234`
   * This command will not autofill the user, you need to type the username and number
# Traditional ($) Commands:
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