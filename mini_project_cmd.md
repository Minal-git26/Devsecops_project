jenkins & java install 

    sudo apt update
    sudo apt upgrade -y
    sudo apt install fontconfig git default-jre -y
    #Sudo nano bash.sh
    #Give permission to bash.sh (700)
    
    
    sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
      https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
    echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
      https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
      /etc/apt/sources.list.d/jenkins.list > /dev/null
    sudo apt-get update
    sudo apt-get install jenkins -y
    systemctl is-active jenkins
    
    sudo systemctl restart jenkins
    sudo systemctl status  jenkins

install git and docker 

        sudo apt install git docker.io  -y
        sudo systemctl start docker
        sudo systemctl status  docker
  




