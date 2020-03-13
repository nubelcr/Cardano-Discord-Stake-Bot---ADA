To use this bot you'll need to first visit the discord developer page and create an application.
https://discordapp.com/developers/applications/

After you created an application, give it a name and a picture.

Next, open up the file "settings.json" using your preferred text editor.

On the discordapp developer page, click bot on the left hand side, then copy the token under the bots username. and replace the ##PUT_BOTS_APP_TOKEN_HERE text with it.

"token":"##PUT_BOTS_APP_TOKEN_HERE"

Copy your client id from the discord developer page (right below the bots name) and replace the following text with the copied client id:
##BOT_CLIEN_ID_HERE

client":"##BOT_CLIEN_ID_HERE"

replace the text ##PUT*YOUR_DISCORDIDWITH*#XXXXS_AT_THE_END_HERE with your discordname with # sign and 4 numbers between the quotes. You can find this in the bottom left of discord.

"ownerId":"##PUT*YOUR_DISCORDIDWITH*#XXXXS_AT_THE_END_HERE"

Save file and close.

Next navigate to the main folder and open your prefferd CLI.

Type in the following command and press enter.

node bot.js

If you see
[Cron Scheduler] Event 'UpdateEpoch' has been schedule. Timezone:America/New_York|Cron:39 14 \*\*\* then your bot has started.

Now you can proceed to discord and assign your stake pool id

To set the pools id use the following command, but replace the long number with your pool's ID:

!setpoolid 28099aba9ea7c89cdb2a44a4c6640e4137e1939bd75451202c67dd384814dfc9

In the above example, this should set the bot to pull results from the SOBIT stakepool.

Make sure to give bot permissions to post in the channels. Currently the bot is set to auto post to default discord channel. In the future this may changeable.

Available Commands
To see the latest 5 epochs history, just type:
!epoch

To see a specific epoch results use the command as above but enter the epoch # that you want to view.
!epoch #

- Example:
  !epoch 89

If you would like to help support this open-source project you can help in a mutliple of ways.

Help add functionality, suggestions and provide feedback.
Donating Cardano to: DdzFFzCqrhsgeoZkAuLRuR3tFSyYGVcvmgXC8LjBZ6Bptcf6ysUNYU7pxXpKK6agWiy5wtsoB4WV9ZS54VkVxW67HUNz6ZGUP3uAFfMk
