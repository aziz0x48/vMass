# vMass Bot  :hook:  FREE Version 1.2
<p align="center">
<img src="https://raw.githubusercontent.com/c99tn/Randoms/master/n.png?token=GHSAT0AAAAAABVX6V7OVKN5YN5NXLEK7T6MYYHZ5VA" width="850">
</p>  
<p align="center"> 
<a href="#requirements-wrench">Requirements</a>  ◦ 
<a href="#installation-package">Installation</a>  ◦ 
<a href="#usage--rescue_worker_helmet">Usage</a>  ◦ 
<a href="#contact--speech_balloon">Contact</a> 
</p> 
<br>   
<b>vMass Bot</b> automates the exploitation of remote hosts by trying to find environment files (.env) in the target hosts and extract tools and info insde, 
then the bot detects the targets host CMS and tries to auto-exploit and upload shell payload using the vMass vulnerability set <b>( 108 exploits in the current version 1.2, check the full vulnerability list in our <a href="https://t.me/+7wraokmFiCcxOTk0">Telegram Channel</a> )</b>.  

No target list ? No worries, <b>vMass Bot</b> can generate hosts lists from IP ranges, URL list, dotenv low profile dorks and scrapes from (bing, duckduckgo, ..) or you can use IP ranges from various hosting providers for best hit rate while scanning, then generated lists can be checked using the bot to eleminate invalid/dead hosts.
      

Extracted Tools, can be filtered and tested to only keep working ones (test smtp delivery and twilio api balance), the bot can also use wp hosts with phpmyadmin access to perform auto upload (admin takeover) if the CMS Exploits failed, working tools can be delivered right to your telegram channel inbox by settings up your telegram webhook in the Bot. The whole process from generating hosts and scanning to delivering the results to Telegram, can be automated using the AUTOPILOT option (For more information, check vMass Bot <a href="/#">Usage</a>).

# Requirements :wrench:
- Perl v5.x+ ( For Windows, get <a href="https://strawberryperl.com/">Strawberry Perl</a> )
- RDP/VPS ( <b>Optional</b> )

# Installation :package:
1- Clone vMass Bot
``` 
$ git clone https://github.com/c99tn/vMass.git
$ cd vMass
```
2- Install required Perl Modules -- IMPORTANT
Install Modules with Bash Script
```
$ chmod +x install.sh
$ bash install.sh
```
<b>OR</b>  
Install Perl modules manually
```
$ perl -MCPAN -e shell 
cpan[1]> install Net::IP
         install Net::DNS::Resolver
         install LWP::UserAgent
         install HTTP::Request::Common
         install WWW::Mechanize
         install Term::ANSIColor
cpan[1]> quit
```
3- Launch vMass Bot
```
$ perl vMass.pl
```
# Usage  :rescue_worker_helmet:
<p align="center">
<img src="https://raw.githubusercontent.com/c99tn/Randoms/master/zoomed.png?token=GHSAT0AAAAAABVX6V7OMNF66DBGMCXAJ3SSYYIEZLQ" width="800">
</p>  
<p align="center">
<b>vMass FREE Version only includes Features with :green_square:</b>  
</p> 


| Command | Description |
| :---: | --- |
| 1 | :green_square: Generate target hosts from given IP Range, you can use more as many ranges as you like (ex:  100.20.0.0/14 )              |
| 2 | :yellow_square: Generate target hosts from given dorks or using the bot env dorks, you can specify target hosts region, TLDs and search engines |
| 3 | :green_square: Generate target hosts from given Website List, PS: URL Lists must me domain.com format only without www or https          |
| 4 | :green_square: Generate target hosts from provided hosting ip range, range is picked randomly, you can change range before starting      |
| 5 | :green_square: Check the targets hosts to filter Live Running IPS from dead ones.                                                        |
| 6 | :green_square: Scan the target hosts for possible .env files, the bot will test all host directories and saves host if env is found      |
| 7 | :yellow_square: Scan the target hosts for .env and perform auto exploit based on host CMS to upload shell payload (108 exploits)          |
| 8 | :yellow_square: Under Construction...  :ninja:                                                                                            |
| 9 | :green_square: Extract tools from hosts where env file is found based on tool type                                                       |
| 10| :yellow_square: test extracted SMTPs, an email input is required, if the smtp delivers, the smtp info will be in the email body           |
| 11| :yellow_square: test extracted TWILIOs APIs validity and balance                                                                          |
| 12| :yellow_square: try to find phpmyadmin login page path, and perform admin takeover method to upload shell in Wordpress CMS hosts               |
| 13| :yellow_square: Transfer all tools to a private telegram channel, telegram webhook is required                                            |
|1337| :yellow_square: performs all the steps above one after another, you just configure the bot, start it and results will be delivered to your telegram, best use for RDP/VPS and with big target hosts list |
<br>

# Contact :speech_balloon:
Got a Question ?
send me DM on <a href="https://t.me/dpr52">Telegram</a>

# Disclaimer :bangbang:
vMass Bot was created for educational purposes only, Any actions and/or activities done using this bot is solely your responsibility.

## :ringed_planet: Join Our Channel To be Notified of Updates and New Releases :ringed_planet:
 
<br>
<p align="center">
<a href="https://t.me/+7wraokmFiCcxOTk0">
<img src="https://raw.githubusercontent.com/c99tn/Randoms/master/telegram_button_icon_151837.png?token=GHSAT0AAAAAABVX6V7OOUCJTCCDNVAXPHCMYYIHTNA" width="200" height="50">
</a>
</p>

