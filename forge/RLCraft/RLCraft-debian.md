Debian Server 11 RLCraft install

apt update

apt install cockpit

apt install ufw

systemctl restart cockpit.socket

systemctl status cockpit.socket

sudo ufw allow 9090
sudo ufw allow 80

sudo ufw enable

sudo ufw status

Add line to apt etc/apt/sources.list "deb http://deb.debian.org/debian stretch main contrib non-free"

apt update

apt install openjdk-8-jre

wget https://maven.minecraftforge.net/net/minecraftforge/forge/1.12.2-14.23.5.2860/forge-1.12.2-14.23.5.2860-installer.jar

java -jar <forge-file> --installServer

wget https://maven.minecraftforge.net/net/minecraftforge/forge/1.12.2-14.23.5.2860/forge-1.12.2-14.23.5.2860-universal.jar

wget https://media.forgecdn.net/files/3655/676/RLCraft+Server+Pack+1.12.2+-+Release+v2.9.1c.zip

unzip <RL-Craft-Server-Pack-x.x.x>

nano start.sh

~
~ java -Xms<MIN-MEM>G -Xmx<MAX-MEX>G -jar <universal.jar>
~

chmod +x start.sh

./start.sh
