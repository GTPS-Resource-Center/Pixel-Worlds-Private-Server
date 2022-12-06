###### This is a private server for PIXEL WORLDS and is currently set to the proper version at the time of uploading.
###### If the version no longer matches when you try to run a build then follow the steps below on 
###### how to update your version to the proper one.

### If You're lazy or don't know how to use Visual Studio then you can use the pre-built version (Release.zip) which is set to the Current version 94.

### STEPS TO SETUP
----------------------
#### 1.) Download & Install Visual Studio. (If you download 2019 PRO then you can use the activation key provided)
## Visual Studio 2019 Pro License Key: NYWVH-HT4XC-R2WYW-9Y3CM-X4V3Y
#### 2.) Open the .sln with Visual Studio.
#### 3.) Click Build in the tab, then Build Solution.. OR do ctrl+shift+B.
#### 4.) Once built, Goto the folder where the exe is : (PixelWorldsServer2/bin/Debug/netcoreapp3.1/)
#### and COPY EVERYTHING in the folder.

#### 5.) Make a new folder on your desktop (or where you want) and paste the contents into it..
#### 6.) Set your Firewall to allow incoming connections on port 80 & 10001 on both UDP & TCP (same as gtps method)
#### 7.) Copy the "player.dat" and "items.txt" to your created folder where the exe is before running.
#### 8.) Now the server can be started.

### HOW TO UPDATE VERSION IF GET AN ERROR
--------------------------------------------
#### While the project is open in Visual studio Goto the "PWServer.cs" file located in "Networking/Server"
#### and increase the version number on LINE 21 by ONE then rebuild and check... keep doing this until it works
#### and you will have found the new version number.

### TO PLAY ON SAME PC AS SERVER YOU NEED TO ADD THE FOLLOWING TO YOUR HOSTS FILE
----------------------------------------------------------------------------------------------------------------------
##### 127.0.0.1 prod.gamev81.portalworldsgame.com
##### 127.0.0.1 prod.gamev82.portalworldsgame.com
##### 127.0.0.1 prod.gamev83.portalworldsgame.com
##### 127.0.0.1 prod.gamev84.portalworldsgame.com
##### 127.0.0.1 prod.gamev94.portalworldsgame.com

#### if someone from Another pc wants to connect they need t0 switch "127.0.0.1" to the actual ip.

#### if version is higher than 94 then add more lines with leading numbers... example: if 97 then add
##### 127.0.0.1 prod.gamev95.portalworldsgame.com
##### 127.0.0.1 prod.gamev96.portalworldsgame.com
##### 127.0.0.1 prod.gamev97.portalworldsgame.com

### How to find Hosts File?
-----------------------------
#### Open "File Explorer" and click "This PC or My Computer" then Open "WINDOWS" folder and Find "System32"
#### and open it. While in "System32" folder search in the top right for "hosts" and wait till it shows...
#### Right click "hosts" and open with notepad or notepad++ then you can add the new host data for your server.

### Private Server Commands
--------------------------------
PLAYER COMMANDS
#### /spin
#### /pay
#### /find
#### /clearinv
THESE GET ENTERED INTO THE GAME CHAT!

SERVER ADMIN COMMANDS (CONSOLE):
#### /help
#### /stop
#### /getinfo (name)
#### /setvip (userid)
#### /setmod (userid)
#### /setadmin (userid)
#### /givegems (userid) (amount)
THESE GET ENTERED INTO THE CMD WINDOW NOT THE GAME CHAT!

### How to Edit Shop
-----------------------
#### While the project is open in Visual Studio, Goto the Shop.cs File in "Database" Folder.
#### You can change/add/remove items there with the line below

AddShopOffer("nameNOSPACES", priceingems, itemid);
