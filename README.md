# Buttons for SAMMI Solutions

## twitch-command-followage.json

!followage  
Returns self follow age of chatter that sent command

!followage username  
!followage @username  
Returns follow age of target username.

Response:  
username has been following streamername for 1 years 6 months 9 days 3 hours 11 minutes 

If no target user string remains after sanitization of message  
(e.g. chatter typed !followage #@&%) then defaults to self followage.  

Puts a message in chat if timeout with Twitch API  

If not following (or target is broadcaster), chat message is "username not following"  

Gets total years with decimal places between follow date/time to current time  
Calculates from total years a breakdown of years, months, days, hours, minutes.  
Builds a response message only for units above 0. If 0 years, doesn't mention years.  
If followage time is less than a minute, result is "0 minutes" followage.  

## walkons.json

Create source in OBS (image/gif/video/sound) named: walkon-username

Edit Default Variables list of chatters with walk ons

Button will match chatter's message with list and then turn visibility of matching source on for N seconds. 

For Subs only, check trigger option. Only need to add chatter to list once. Don't need to remove from list. 

## twitch-command-sleeper-mods.json  

Mods can chat without badge/role. Then, give themselves mod role when needed.

Store list of approved chat mods in the Default Variables array

Chatter can type !modme and the button will check the list

If approved, the chatter is assigned mod role

If not approved, a chat message will say they are not approved.

Mods can use Twitch's native /unmod username command to unmod themselves.

## Disclaimer

This is an unofficial community project. I am not affiliated with 
SAMMI Solutions.
