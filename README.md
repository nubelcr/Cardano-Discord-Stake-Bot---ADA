## Support

This project was made with love by TheChemist. If you would like to help support this open-source project you can help in a mutliple of ways.

Help add functionality, suggestions and provide feedback as well as donating ADA to the following address or joining my Stake pool!

Donate Cardano to:
```bash
addr1q822nxjuu89qf4p29r9gkk72ewvxh9l6sc6ctgcdf2us5fre3z6p6zd8x49z9ccrmz07fk0prd9e8nqzgvc7mwy2u4zsh87dwf
```


## Install instructions

1) To use this bot you'll need to first visit the discord developer page and create an application.
```bash 
https://discordapp.com/developers/applications/
```
After you created an application, give it a name and a picture.

2) Next, open file "settings.json", located in the data folder using your preferred text editor.

3) On the discordapp developer page, click "Bot" on the left hand side, then copy the token located under the bots username. Replace the ##PUT_BOTS_APP_TOKEN_HERE text with copied token.

```bash 
"token":"##PUT_BOTS_APP_TOKEN_HERE"
```

4) Copy your client id from the discord developer page (right below the bots username) and replace the following text with the copied client id:
##BOT_CLIEN_ID_HERE
```bash
client":"##BOT_CLIEN_ID_HERE"
```
5) replace the text ##PUT*YOUR_DISCORDIDWITH*#XXXXS_AT_THE_END_HERE with your discordname with # sign and 4 numbers between the quotes. You can find this in the bottom left of discord.

```bash
"ownerId":"##PUT*YOUR_DISCORDIDWITH*#XXXXS_AT_THE_END_HERE"
```

6) Save file and close.


7) Next navigate to the main folder and open your prefferd CLI.


8) Type in the following command and press enter. Note this requires node.js to be installed. |

```bash
node bot.js
```

If you see

```bash
[Cron Scheduler] Event 'UpdateEpoch' has been schedule. Timezone:America/New_York|Cron:39 14 \*\*\*
```
then your bot has started.


10) Now you can proceed to discord and assign your stake pool id

To set the pools id use the following command, but replace the long number with your pool's ID:

```bash
!setpoolid 28099aba9ea7c89cdb2a44a4c6640e4137e1939bd75451202c67dd384814dfc9
```

In the above example, this should set the bot to pull results from the SOBIT stakepool.

Make sure to give bot permissions to post in the channels. Currently the bot is set to auto post to default discord channel. In the future this may changeable.

That's it! Time to enter commands and test out the stakebot!


## Available Commands

To see the latest 5 epochs history, just type:

```bash
!epoch
```
To see a specific epoch results use the command as above but enter the epoch # that you want to view.
!epoch #

```bash
Example:
  !epoch 89
```

## Future API updates

Should the API from PoolTools ever change, you can easily modify and update the bot yourself by visiting the commands.json file located in the data folder. update inside the parenthesis with the correct URL but DO NOT DELETE ${serverVars(\"PoolID\")} or you are guaranteed to have a bad time mkay?

```bash
"url":"https://pooltool.s3-us-west-2.amazonaws.com/8e4d2a3/pools/${serverVars(\"PoolID\")}/epochstats.json"
```