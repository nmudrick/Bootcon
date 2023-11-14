# Bootcon
Monitoring Minecraft server with Splunk Monitoring!

Commands to Download splunk onto server: 
* Mkdir /opt/splunk
* Cd /opt/splunk 
* Sudo chown ec2-user /opt/splunk 
* Pwd 
* wget -O splunk-9.1.1-64e843ea36b1-Linux-x86_64.tgz "splunk-download-link"
* Tar -xzyC -f “splunk-9.1.1-64e843ea36b1-Linux-x86_64.tgz" 
* Cd bin
* ./splunk status
* ./splunk start 


Commands to Download Minecraft server to your server: 
* sudo rpm --import https://yum.corretto.aws/corretto.key
* sudo curl -L -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo
* sudo yum install -y java-17-amazon-corretto-devel.x86_64
* java —version
* 
* (this was to install java)
*  
* mkdir /opt/minecraft/
* mkdir /opt/minecraft/server/
* cd /opt/minecraft/server
* Sudo chown ec2-user /opt/minecraft/server
* scp -i "Minecraft2.pem" server.jar ec2-user@ec2-54-173-200-161.compute-1.amazonaws.com:/home/ec2-user/minecraft_server     (this is to get the downloaded minecraft server onto remote machine) 
* java -Xmx1G -Xms1G -jar seerver.jar nogui
* Nano eula.txt( change to true)

* Command to run the minecraft server: 
* java -Xmx1G -Xms1G -jar minecraft_server.1.20.2.jar nogui





