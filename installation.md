# Jenkins Installation on Google Compute Engine


## Pre-requisite:

* Ubuntu-based VM, e.g Ubuntu 22.04 LTS x86-64
* Java 11

## Installation Step:

1. SSH to your VM
2. Run this script
```
sudo apt install openjdk-11-jdk-headless -y 
wget https://get.jenkins.io/war-stable/2.375.1/jenkins.war

#run jenkins.war using custom port 9090 and bring to background process 
nohup java -jar jenkins.war --httpPort=9090
```

Open http://your-external-ip:9090 from your browser, and continue your setup
