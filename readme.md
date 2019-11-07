Assuming you already have Opengamepanel and Trinitycore installed.

1. Copy the XML files to {path to your OGP web root}/modules/config_games/server_configs/ and give ownership to your webserver user 
by using: "chown www-data:www-data {path to your OGP web root}/modules/config_games/server_configs/trinity*"
2. In OGP go to Gameservers.
3. Select new Gameserver.
4. Select the Server where the Gameserver is supposed to be hosted.
5. Select Gametype "Trinitycore authserver" and adjust the other settings to your needs.
6. Change Homepath to the path to your trinitycore installation directory (eg. /home/ogpbot/Trinitycore335)
and click Change Home.
7. Set your IP/Port (default Port is 3724) and click set IP.
8. Click Back to Game Monitor and start your authserver.
9. Go to Gameservers again.
3. Select new Gameserver.
4. Select the Server where the Gameserver is supposed to be hosted.
5. Select Gametype "Trinitycore worldserver" and adjust the other settings to your needs.
6. Change Homepath to the path to your trinitycore installation root directory (eg. /home/ogpbot/Trinitycore335)
and click Change Home (you can ignore the massage which informs you that this home is already chosen).
7. Set your IP/Port (default Port is 8085) and click set IP.
8. Click Back to Game Monitor and start your wordserver.

You now can use Opengamepanel to manage your Trinitycore server.
To access the Console, just go to your worldserver and click on Log Viewer.

Keep in mind that OGP will set the ownership of your Trinitycore directory and all files contained to your OGP-Agent User.
