# Reaction Role Class Instructions:
The following are instructions for how Admins/Mods can create classes that are joinable with Zira reaction roles. This can be done with other reaction role bots but Zira will be used for this tutorial.

### Enable developer mode:
   * Click the settings icon on the bottom left of the Discord desktop app </br>
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/1.PNG)
   * Click "Advanced" then turn on developer mode.
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/2.PNG)

### Creating Roles
   * The first step will be creating the roles for the classes you want to add
   * Go to the server, click the servers name in the upper left, then click "Server Settings"
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/3.PNG)
   * Click "Roles" and then click "Add a Role"
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/4.PNG)
   * Name the role, I suggest naming them consistently so the next steps are easier.
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/5.PNG)
   * Click "Save" and repeat for as many classes as you need to add

### Creating the Reaction Role message
   * This step may be unneeded if your server already has messages with roles attached.
   * I suggest typing something out like this to make it clear for people how to add themselves to classes
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/6.PNG)

### Setting the Channel ID and Message ID with Zira
   * Right click the channel the message from above is in and click copy ID
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/7.PNG)
   * Go to a chat (preferably a private chat with you and Zira so you don't spam others with notifications)
   * Type `z/channel 123456789` replacing 123456789 with the channel ID you just copied
   * Go to the message you want to add reactions to and right click, click "Copy ID"
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/8.PNG)
   * Go back to the channel you typed the last Zira command
   * Type `z/message 12345678` replacing 123456789 with the message ID you just copied
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/9.PNG)

### Adding the reactions to the message with Zira
   * **This process will need to be completed for every class/role you are adding**
   * In the same chat you typed the last Zira commands:
   * Type `z/normal :emoji: @rolename`
      * Where `:emoji:` is an emoji in Discord (You can also use the emoji selector on the right side of the chat bar)
      * And where `@rolename` is the role you created in the first step
   * Ex: `z/normal :one: @MECH103`
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/10.PNG)
   * If it worked Zira will confirm and a reaction will show up on the message
![RRInstructions](https://raw.githubusercontent.com/TrevorSLong/CamTheRam-Discord/main/ClassReactionRoleInstructions/11.PNG)
   * If everything worked, continue this process changing the `:emoji:` and the `@rolename` until you've made all the reactions you need.