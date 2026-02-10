java install 

    sudo apt update
    sudo apt install openjdk-11-jdk -y
    java -version
    which java  #/usr/bin/java

jenkins intsall

     sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc \
      https://pkg.jenkins.io/debian-stable/jenkins.io-2026.key
    echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" \
      https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
      /etc/apt/sources.list.d/jenkins.list > /dev/null
    sudo apt update
    sudo apt install jenkins   

        sudo systemctl enable jenkins
        sudo systemctl status jenkins
