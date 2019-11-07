https://github.com/TrinityCore/TrinityCore <br>
https://github.com/OpenGamePanel/OGP-Website <br>
https://github.com/OpenGamePanel/OGP-Agent-Linux <br>

Assuming you already have Opengamepanel and Trinitycore installed.

1. Copy the XML files to {path to your OGP web root}/modules/config_games/server_configs/ and give ownership to your webserver user 
by using: "chown www-data:www-data {path to your OGP web root}/modules/config_games/server_configs/trinity*"
2. Go to administration -> Game/Mod config and click Update Configs

Installing the authserver

3. In OGP go to administration -> gameservers.
4. Select new gameserver.
5. Select the server where the gameserver is supposed to be hosted.
6. Select Gametype "Trinitycore authserver" and adjust the other settings to your needs.
7. Change Homepath to the path to your trinitycore installation directory (eg. /home/ogpbot/Trinitycore335)
and click Change Home.
8. Set your IP/Port (default Port is 3724) and click set IP.
9. Click back to game monitor and start your authserver.

Installing the worldserver

10. Go to administration -> gameservers again.
11. Select new gameserver.
12. Select the server where the gameserver is supposed to be hosted.
13. Select gametype "Trinitycore worldserver" and adjust the other settings to your needs.
14. Change homepath to the path to your trinitycore installation root directory (eg. /home/ogpbot/Trinitycore335)
and click change home (you can ignore the massage which informs you that this home is already chosen).
15. Set your IP/Port (default Port is 8085) and click set IP.
16. Click Back to game monitor and start your wordserver.

You now can use Opengamepanel to manage your Trinitycore server.
To access the console, just go to your worldserver and click on log viewer.
You can also execute commands from there.

⚠️
Keep in mind that OGP will set the ownership of your Trinitycore directory and all files contained to your OGP-agent user.
You can revert this by using: chown -R youruser:yourgroup /path/to/your/trinity/install/
