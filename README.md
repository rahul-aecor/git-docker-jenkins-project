# git-docker-jenkins-project
## Required Installation
- apt install git
- apt  install docker.io
- sudo apt install openjdk-11-jre
- curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee   /usr/share/keyrings/jenkins-keyring.asc > /dev/null
- echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]   https://pkg.jenkins.io/debian-stable binary/ | sudo tee   /etc/apt/sources.list.d/jenkins.list >     /dev/null
- sudo apt-get update
- sudo apt-get install jenkins
- mkdir /home/ubuntu/project
- git clone https://github.com/rahul-aecor/git-docker-jenkins-project.git
- sudo usermod -a -G docker $USER
- sudo usermod -a -G docker jenkins
- sudo chmod -R 777 /var/run/docker.sock
- sudo apt install nodejs
- sudo apt install npm
- npm install
- node app.js

