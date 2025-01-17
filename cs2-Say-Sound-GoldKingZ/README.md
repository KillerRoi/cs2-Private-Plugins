
## .:[ Price ]:. [(Payment Rules)](https://github.com/oqyh/cs2-Private-Plugins/blob/8040379022008134dde7d34cf08f7a611c750862/README.md?plain=1#L7)
```diff
+ PRICE 10$ + FREE Multiple Servers [Lifetime ( One Time Payment )] 
```

# [CS2] Say-Sound-GoldKingZ (1.0.2)  

### Let Players Convert Chat/Radio To Say Sound With Radius

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/GWZRZuL20QA/0.jpg)](https://www.youtube.com/watch?v=GWZRZuL20QA)


## .:[ Dependencies ]:.

[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Say-Sound-GoldKingZ\config\config.json                                         

```json

{

  //Key To Active Plugin
  "KEY": "",

  //Allow Dead Players To Toggle Say Sound?
  "AllowDeadPlayersToSaySound": false,

  //Hide Default Radio Message If Toggle Say Sound By Radio?
  "HideDefaultRadioAfterSaySound": true,

  //Hide Default Chat Message If Toggle Say Sound By Chat?
  "HideDefaultChatAfterSaySound": true,

  //Override Plugins Controls Chat Hook
  "Override_These_Plugins": "CS2-Tags,Plugin2,Plugin3",
}

```


## .:[ Configuration Say Sound ]:.

> [!CAUTION]
> SaySound Config Located In ..\addons\counterstrikesharp\plugins\Say-Sound-GoldKingZ\config\SaySound_Settings.json               
                          
```json
{
  "clap": //This Will Be Hooked To Lang  "saysound.chat.clap" 
	{
	  "SOUND_NAME": "Clapping", //Sound Name To Use In Lang {1} If Needed
	  "MAKE_SOUND_3D": true, //true = Sound will Play As 3d With Ridus || false = Will Play Locally Direct To Players

	  "ONLY_FOR_FLAGS": "@css/admin,#css/root", //Only These Flags Have Access To This Say Sound (Empty OR Not Using It = Anyone Can Use It)

	  "HOOK_RADIO": "cheer", //Hook Radio cheer
	  "TOGGLE_SOUND_IN_CHAT": "clap,claping,clapping", //Toggle This Sound By Chat
	  
	  "PRINT_IN_CHAT": true, //Make Print Ingame Chat "saysound.chat.clap"?
	  
	  "GIVE_COOLDOWN_AFTER_THIS_INSECS": 5, //Give Cooldown After This X Secs
	  
	  "SOUNDPATH_1": "", //Sound Path You Can Add As Many As You Like Its Random Play
	  "SOUNDPATH_2": "",
	  "SOUNDPATH_3": ""
	}
}

```

## .:[ Language ]:.
```json
{
	//==========================
	//        Colors
	//==========================
	//{Yellow} {Gold} {Silver} {Blue} {DarkBlue} {BlueGrey} {Magenta} {LightRed}
	//{LightBlue} {Olive} {Lime} {Red} {Purple} {Grey}
	//{Default} {White} {Darkred} {Green} {LightYellow}
	//==========================
	//        Other
	//==========================
	//{nextline} = Print On Next Line
	//==========================
	
	"player.not.allowed": "{green}[SaySound] {grey}You Are Not Allowed, This For {lime}VIPS Only", //make it empty string "" message will not show
	"player.cooldown": "{green}[SaySound] {grey}You Need To Wait {darkred}{0} Secs {grey}Cooldown", //make it empty string "" message will not show
	
	//==========================
	//{0} = Player Name Who Say Sound
	//{1} = SOUND_NAME 
	//==========================
	"saysound.chat.clap": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.cry": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.fart": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.gg": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.haha": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.handsome": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.lightweight": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.mama": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.nicework": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.rizz": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.stop": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.suka": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.whistle": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.wtf": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}",
	"saysound.chat.yeah": "{green}[SaySound] {purple}{0} {grey}: {yellow}{1}"
}
```

## .:[ Change Log ]:.
```
(1.0.2)
-Added AllowDeadPlayersToSaySound

(1.0.1)
-Fix Some Bugs
-Added gkz_plugins To check status of gkz plugins
-Added MAKE_SOUND_3D
-Added Override_These_Plugins

(1.0.0)
-Initial Release
```
