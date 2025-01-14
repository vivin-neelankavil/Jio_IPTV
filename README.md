<!-- DO NOT EDIT FILE AND ADD YOU NAME HERE AND PUBLISH -->
<!-- © 2021-22 TechieSneh -->

<h1 align='center'>Jɪᴏ IPTV Server</h1>
<h4 align='center'>A Jio IPTV server based on Apache and PHP server than can be run on Android TV, Android set top box and other android things to stream Jio IPTV channels</h4>
<br>
<h2>Description</h2>
Why need to pay for monthly TV subscription to Airtel, DishTV, Tata Sky or even Jio when you can get around 945 TV channels by already using an Jio postpaid or prepaid mobile subscription and have an internet connection at home? <br>
Kudos to the author  <a href="https://github.com/mitthu786">mitthu786</a> for developing this script, I am just a better documenter<br>
Please do star <a href="https://github.com/mitthu786">mitthu786</a> and my repository<br>

<h2>Features</h2>
&ensp; - Supports streaming IPTV in Auto, 250p, 400p, 600p, 800p, 1200p<br>
&ensp; - Remote/LAN player and IPTV clients support<br>
&ensp; - Works on mobile, Android TV or PC internet browser<br>
&ensp; - Search channels by Channels, Genre and Language<br>
&ensp; - Themes support for the remote/LAN player<br>


<h2>Disclaimer</h2>
&ensp; - This is Just For Educational Purpose <br>
&ensp; - The TV channels are not streamed for free, you must have an active Jio postpaid/prepaid subscription that comes with a 'JioTV' app access in order for the IPTV script to work <br>
&ensp; - I am not the author of this script, so I don't know if this script injects or collects information from us, use at your own risk.

<h2>How To Use</h2>
I am just concentrating on configuring Android TV and Android set top box in this document to not confuse the users reading this <br>
BTW you need atleast 2Mbps internet bandwidth allocatted just for your Android TV for a smooth and HD streaming experience.<br>
<br>
Steps

1. Install the following android apps from any android play store(be it aptoide or mod market)<br>
  a. <a href="https://play.google.com/store/apps/details?id=ru.kslabs.ksweb">'KSWEB: web developer kit'</a>, the author of this script recommends using paid/PRO version<br>
  b. <a href="https://play.google.com/store/apps/details?id=ar.tvplayer.tv">Tivimate</a> or <a href="https://play.google.com/store/apps/details?id=studio.scillarium.ottnavigator">OTT Navigator Player</a>, I recommend using the paid version of <a href="https://play.google.com/store/apps/details?id=by.stari4ek.tvirl">TVirl</a> as this it has the closest/similar interface of using ideal TV setup box<br>

2. Download the [JioTV zip](https://github.com/mitthu786/TS-JioTV/blob/main/tsjiotv.zip?raw=true) file<br>
  a. Extract the 'tsjiotv' folder inside the tsjiotv.zip and copy it to 'htdocs' directory <br>
  As per my 'Airtel xstream Android TV Box' the 'htdocs' location looks like this

    ```py
    /mnt/sdcard/htdocs
    ```

  &ensp; &ensp;   After you have pasted the 'tsjiotv' folder, the directory structure of the 'htdocs' directory should look like this
    
    /mnt/sdcard/htdocs/tsjiotv/
  
3. Configure the 'KSWEB Pro' <br>
  a. Connect a wired/wireless mouse (optionally a keyboard) to your Android TV / setup box and follow the below steps by using a mouse<br>
  b. Open 'KSWEB Pro', turn OFF the KSWEB PRO server by using the toggle switch and goto each service sections that is displayed above of your TV screen and disable all the services except Apache and PHP <br>
  c. Goto 'Apache' section and click on that path displayed and select 'Edit Host Config file' and change the port mentioned in the 12th line as '8080', click save and exit <br>
  d. Goto 'Setting' section and enable 'Auto start', 'Start minimized' and 'Turn off battery saving' (you may need to follow few more steps to turn off battery saving in Android settings) <br>
  e. Goto 'Status' section, turn ON the KSWEB PRO server by using the toggle switch and note down the private ip address of your 'Android TV' that looks somethings like this '192.168.x.x' <br>

https://user-images.githubusercontent.com/2281995/185786113-aac4f71f-d4dd-41e9-9918-ce39112a5b69.mp4



4. Login to JioTV server with your Jio credentials, just for the first time <br>
  a. Using the 'Android TV' internet browser, type in the below URL in the address bar and continue with the login process <br>

     ```py
     http://localhost:8080/tsjiotv/login.php
     ```

  &ensp; &ensp; b. Using your mobile, iPad or PC's internet browser that is connected to same WiFi/LAN network as Android TV <br>
  &ensp; &ensp;   Your JioTV server IP is same as the 'Android TV' private IP we noted down earlier, type in the below URL (replaced with your private IP) in the address bar and continue with the login process  <br>

     http://<your_private_ip>:8080/tsjiotv/login.php

5. Open Tivimate or OTT Navigator Player and configure the IPTV playlist<br>
  a. Select local playlist option and choose the 'localplaylist.m3u' file from the htdocs/tsjiotv directory <br>
  b. in case your IPTV video is lagging/buffering or you don't have the required internet bandwidth to stream smoothly, then choose the default required resolution from one the playlist at htdocs/tsjiotv directory.<br>
  c. Optionally, you can configure to auto start Tivimate or OTT Navigator on Android TV boot (or waking from sleep) and start playing TV channels automatically as any TV or set top box would do. <br>

Hurrah !! Now enjoy streaming TV Channels on your Android TV.<br>

<h2>Screenshots</h2>

<table>
  <tr>
    <td><img src="screenshots/remote_portal.png" width="400" height="200"></td>
    <td><img src="screenshots/video_player.png" width="400" height="200"></td>
  </tr>
  <tr>
    <td><img src="screenshots/Android_home_screen_showing_Tivimate_and_KSWEB.png" width="400" height="200"></td>
    <td><img src="screenshots/TiviMate_channel_group.png" width="400" height="200"></td>
  </tr>  
  <tr>
    <td><img src="screenshots/Channel_EPG.png" width="400" height="200"></td>
    <td><img src="screenshots/Fullscreen_view_of_channel.png" width="400" height="200"></td>
  </tr>
</table>

<br>
