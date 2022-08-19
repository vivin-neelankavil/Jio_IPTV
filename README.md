<h1 align='center'>Jɪᴏ IPTV Server</h1>

<!-- DO NOT EDIT FILE AND ADD YOU NAME HERE AND PUBLISH -->
<!-- © 2021-22 TechieSneh -->

<h4 align='center'>A Jio IPTV server based on Apache and PHP than can be run on Android TV and Android things to stream Jio IPTV channels</h4>
<h6 align='center'>Login with your own Jio credentials (username & password) to stream channels using this script</h6>
<br>

<h2>Features</h2>
&ensp; - HQ Streaming Free of Cost<br>
&ensp; - Will Works In 250, 400, 600, 800, 1200(FEW NOT SUPPORT) in this Given Qualities<br>
&ensp; - Web Play Supports<br>
&ensp; - Works on Mobile, AndroidTV or PC Browser Perfect<br>
&ensp; - Search channels by Channels, Genre, Language<br>
&ensp; - Themes support fort the portal<br>

<br>

<h2>Screenshots</h2>

<table>
  <tr>
    <td><img src="screenshots/main/main.png" width="400" height="200"></td>
    <td><img src="screenshots/main/play.png" width="400" height="200"></td>
  </tr>
</table>

<br>

<h2>How To Use</h2>
I am just concentrating on configuring Android TV's in this document to not confuse the users reading this
BTW you need atleast 2Mbps internet bandwidth alocatted just for Android TV for smooth and HD viewing experience

Steps

1. Install the following android apps from google play store
  a. 'KSWEB: web developer kit', the author of this script recommends using  paid/PRO version
  b. Tivimate or OTT Navigator Player, I recommend using the paid version<br>

2. Download the [JioTV zip](https://github.com/mitthu786/TS-JioTV/blob/main/tsjiotv.zip?raw=true) file<br>
  a. Extract the 'tsjiotv' folder inside the tsjiotv.zip and copy it to 'htdocs' directory <br>
  As per my 'Airtel xstream Android TV Box' the 'htdocs' location looks like this
  ```py
/mnt/sdcard/htdocs
```
  After you have pasted the 'tsjiotv' folder, the directory structure of the 'htdocs' directory should look like this 
```py
/mnt/sdcard/htdocs/tsjiotv/
```

3. Configure the KSWEB Pro
  a. Open KSWEB Pro and disable all the service except Apache and PHP
  b. Goto 'Apache' section and edit the configuration file to run the Apache server to run on port 8080
  c. Goto 'Setting' section and enable 'Auto start', 'Start minimized' and 'Turn off battery saving' (you may need to follow few more steps to turn off battery saving in Android settings)
  d. Goto 'Status' section and note down the private ip address of your 'Android TV' that looks somethings like this '192.168.x.x'

4. Login to JioTV server with your Jio credentials, just for the first time
  a. Using the 'Android TV' internet browser 
     ```py
     http://localhost:8080/tsjiotv/login.php
     ```
  b. Using your mobile, iPad or PC's internet browser
    Your JioTV server ip same as the 'Android TV' private ip we noted down earlier
    ```py
     http://<your_private_ip>:8080/tsjiotv/login.php
    ```

5. Open Tivimate or OTT Navigator Player and configure the IPTV playlist<br>
  a. Select local playlist option and choose the 'localplaylist.m3u' file from the htdocs/tsjiotv directory <br>
  b. in case your IPTV video is lagging/buffering or you don't have the required internet bandwidth to stream smoothly, then choose the default required resolution from one the playlist at htdocs/tsjiotv directory.

Hurrah !! Now Play & Enjoy with your Jio Channels .</b><br>


<!-- DO NOT EDIT FILE AND ADD YOU NAME HERE AND PUBLISH -->
<!-- © 2021-22 TechieSneh -->
<br>

<h2>Disclaimer</h2>
&ensp; - This is Just For Educational Purpose

<h3>Get in touch with the original author of this script below (I am just a user who looks to document & guide other user to configure this server well) : </h3>
&ensp; • For any Support Join Our Channel [Techie Sneh Official](https://telegram.me/techiesneh_official)<br>
&ensp; • For Any Query Contact at [ProtonMail](mailto:techiesneh@protonmail.com)

<br>

---
<h4 align='center'>© 2021-22 Techie Sneh</h4>

<!-- DO NOT REMOVE THIS CREDIT -->
