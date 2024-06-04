# All below requires you to have allready installed sammi and set it up with your account. if you have not done so allready please follow the instructions in the link below
https://sammi.solutions/docs/getting-started/step-by-step

# KBM  Sammi package install guide:
- Open the JSON files provided with a text editor of any kind.
- Copy the entire file and click paste deck in SAMMI, do this for all modules you would like to add.
- copy kbmBeep.ogg to your Sammi folder
- to update a module simply replace the old one by hitting yes when it says the deck already exsists
- Restart sammi after adding all modules to ensure all settings are loaded

all modules require KBM core to work but all other modules are optional

# KBM Sammi core usage guide:

### using your streaming account as the bot
- To use these scripts with JUST your streaming account simple open up your twitch chat and type !assignchannel (your channels name)

```!assignchannel keyboardmedic```

### using a second bot account as the bot
- To use it with a bot account connect a second account to your Sammi the same way as you add a normal account, then tick “join chat under this name” on the account you want to have function as your bot
- Type in your twitch chat “!assignchannel (your streaming channels name)“
to assign the channel for the bot to output messages to 


without this command the bot will output to its own chat

```!assignchannel keyboardmedic```

### Other commands and features in KBM core
- For a help message in chat use !kbmhelp
- To quickly stop all ongoing commands use !stop
- To see if the bot is actually in your chat use !bot
- To switch between using the “SAMMI:” prefix before every message use
!prefix (on or off)
- To display the current version of the modules that you are running use
!kbmversion
- To display a disclaimer and explanation about keybotmedic written by myself, keyboardmedic use the command !keybotmedic

# KBM autoSO usage guide:

### Using AutoSO:
by default it will automagicly shout out everyone who is on the list on their first message in chat of the session. It has a delay of 1.5 seconds before it shouts out.   
By default the list contains only 2 names: KeyboardMedic and Ibohlution   
By default autoSO outputs “!so username” in chat on a shoutout   
you don’t have to worry about using @ or caps. As long as the spelling is correct it will work

### Adding a name to the list:
To add a new name to the list simply type in twitch chat “!soadd username” 

```!soadd @keyboardmedic OR !soadd Keyboardmedic```


Sammi will output a message in twitchchat saying wether it worked or if the name is already in the list and will shout out the new name on the list
```
	“SAMMI: keyboardmedic added to the SO list.”
OR
	“SAMMI: keyboardmedic is allready in the list”
```

### Removing a name from the list
To remove a name to the list simply type in twitch chat “!soremove username” 

```!soremove @keyboardmedic OR !soremove Keyboardmedic```

Sammi will output a message in twitchchat saying wether it worked or if the name is already in the list
```
	“ SAMMI: keyboardmedic removed from the SO list..”
OR
	“SAMMI: keyboardmedic is not in the list”
```

### Changing the delay for a shoutout:
The change the time the script takes to put a shoutout in chat after the first message of the chatter you can use the command “!sodelay number in ms” to change the delay time

```!sodelay 2000```

### Changing the shoutout message:
To change the message used in the shoutout you can use the command 
“!somessage message you would like to use” You can use the variable “/username/” to target the user that is going to receive the shoutout.

```!somessage big shoutout to /username/! Check them out at twitch.tv//username/```

### Switching between shouting out from the list or shouting out all viewers:
By default the bot will only SO people that are on the list. you can change it to shout out everyone on their first message You can use “!soall on or off”.

```!soall on```

### Adding names to exclude from shoutouts:
To add excluded names to the list who will NOT be shouted out if autoSo is set to shout out all viewers use “!soexclude username”.

```!soexclude streamelements```

### Removing names from the excluded list:
To remove excluded names to the list who will NOT be shouted out if autoSo is set to shout out all viewers use “!soexcluderemove username”.

```!soexcluderemove streamelements```

### Turning sound notifications on or off on first chat of the session:
autoSO can play a beep indicating a new message has been sent in chat, to turn it on or off use “!sonotification on or off”

```!sonotification on```


### Use the build in !so commands:
To use the build in !so command use the command “!souse on or off”.
This allows you to use !so <username> to shout out people in your chat.

```!souse on```

### Use the build in follower notification:
To use the build in follower notification use the command “!sofollower on or off”. This will send a thank you message in chat when a new viewer follows.

```!sofollower on```

### resetting autoso to default settings:
In the event of something going wrong, you can reset the list to its default state by using “!soreset”
WARNING this will clear all saved settings and names in the list

### Other commands and features in autoSo:
- ”!help kbmautoso” will display a help message in chat

# KBM raidSo usage guide:
This script wil automagicly shoutout a channel that raids you for X amount of times.   
By default raidSo will also shoutout a raid 3 times total, 1 time after 1.5 second, another one 60 seconds later and one last time 2 minutes after the raid   
By default raidSo outputs “!so username” in chat on a shoutout   

### Changing the amount of times the shoutout repeats:
To change the amount of times you want to repeat the shoutout after a raid use the command “!raidrep number of times you want to repeat”. Note that a number of 1 will repeat twice and 0 will not repeat

```!raidrep 2```

### Changing the delay of the first shoutout:
To change the delay until the first shoutout is given use the command “!raidintdelay number in ms”.

```!raidintdelay 2000```

### Changing the delay between repeated shoutouts:
To change the delay between the repeated shoutouts use the command “!raidrepeatdelay number in ms”.

```!raidrepeatdelay 60000```

### Changing the raid shoutout message:
To change the message displayed on the shoutout use the command “!raidmessage message you would like to use” . You can use the variable “/username/” to target the user that has raided your channel.

```!raidmessage big shoutout to /username/ for the raid! Check them out at twitch.tv//username/```

### Turning sound notifications on or off on a raid:
autoSO can play a beep indicating a raid has arrived, to turn it on or off use “!raidnotify on or off”

```!raidnotify on```

### Other commands and features in RaidSo:
- ”!kbmhelp raidso” will display a help message in chat

# KBM convert time usage guide:
convert time allows you to convert a time from one timezone to another in chat. it will accept 2 formats of timezone:
- europe/amsterdam
- utc

it can do 2 formats of time notation

- 09:00
- 9am

to convert use "!convert time timezone_to_convert_from timezone_to_convert_to"

```!convert 15:00pm est utc```

# KBM randomimage usage guide:
Shows a random image from a list of images in a html file and auto shows and hides an obs source to provide a smooth transition.

Use ```!randomimage``` to show the image and ```!hideimage``` to hide the image if you have not set a hide timer

## Initial setup:
- make sure sammi is connected to obs trough the websocket (check Sammi documentation on how to do this)
- load the deck into Sammi from the json file as described above and restart Sammi to allow it to create the necessary files
- put all the images you want to use in the folder called "kbmrandomimage" in your Sammi folder
- open the file "listofimages.txt" in the "kbmrandomimage" folder, delete the line marked as "delete this line" and add all the names of the files you want the script to use, one line for one file. for example:
```
picture1.jpg
picture2.png
picture3.jpg
```
- create a new scene in OBS and name it "kbmrandomimage"
- create a new browser source in the scene you just created and name it "kbmrandomimagesource" and point it at the local html file you created earlier called "randomimage.html". Make sure to tick refresh source when it becomes visible
- if you want the image to be centered on screen add the following css code to the "costum css" section in the browser source options
```
body {
  display: flex;
  justify-content: center;
}

img {
  display: flex;
  margin: auto;
}
```
- nest this scene in the scene you want to display it to use it in exsisting scenes

## changing the time the image is visible:
To change the time the image is visible on screen use the command "!rihidetime time in seconds"

```!rihidetime 20```

## changing the cooldown for the !randomimage command:
To change the cooldown for the !randomimage command use the command "!ricooldown time in seconds"

```!ricooldown 60```

## changing the activation from a command to a channel point redeem:
To change the activation method from a command to a channel point redeem:
- open the deck in Sammi by double clicking the deck named "KBM random image"
- with the deck open right click on !randomimage and select "Edit triggers"
- set both Twitch chat message options to broadcaster with the tickbox marked broadcaster
- click the plus below the exsisiting triggers and select "Twitch channel point redemption"
- Select your channel point redeem in the dropdown menu (might have to hit "Load from twitch api").
- Save and test your redeem.