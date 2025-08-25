# Postal2-LinuxFix
1|Install the game on linux from steam
2|Set the compatibility tool to "proton hotfix"
3|Have the 5025 Beta update enbaled
4|Install 'Nicks coop [5025]' and 'Nicks coop API' from the workshop for Postal 2
5|Start the game, go into single player and save the game. Exit out of the game completly

Now Browse where the game is installed and follow these instructions but for linux

cd 'D:\SteamLibrary\steamapps\common\POSTAL2Complete'
mkdir WorkshopContent
cd WorkshopContent
wget https://github.com/D4rkMoons/Postal2-LinuxFix/raw/refs/heads/main/1756094907338.tar.gz
untar 1756094907338.tar.gz

BAsicly we used that fix from the forum that specify to replace Postal2.ini
cd ~/.lgp/postal2/System && wget https://gist.githubusercontent.com/Koncord/5ea0d1daec8f1c6185eb72d4ad09eca0/raw/366bc04ff39dea8ef6f02aa89a0e83208f49e8be/Postal2.ini

but we used that fix and replaced Nicks Coop/Postal2.ini proton://[/steamapps/common/POSTAL2Complete/WorkshopConten/737631813/Postal2CoOp.ini] | SteamRuntimeLinux://[/steamapps/common/POSTAL2Complete/WorkshopConten/737631813/Postal2CoOp_Linux.ini]
What we had to modify in the file ( was the line '19' the ConfigVer=5020 -> ConfigVer=5025 -> ConfigVer=5100
LN19|    [ConfigVer] ConfigVer=5020
->>>     [ConfigVer] ConfigVer=5100
