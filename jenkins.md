# Create Jenkins Server

## Install and Run Jenkins

```bash
  sudo apt update

  sudo apt install fontconfig openjdk-17-jre

  java -version

  sudo apt update 

  sudo wget -O /usr/share/keyrings/jenkins-keyring.asc https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
    
  echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]"  https://pkg.jenkins.io/debian-stable binary/ | sudo tee  /etc/apt/sources.list.d/jenkins.list > /dev/null
    
  sudo apt update

  sudo apt install jenkins -y

  sudo systemctl start jenkins

  sudo systemctl enable jenkins

  sudo systemctl status jenkins

  sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```
![Jenkins](images/jenkins-install-1.png)
![Jenkins](images/jenkins-install-2.png)
![Jenkins](images/jenkins-install-3.png)

## Create a Freestyle Job
![Jenkins](images/freestyle-test.png)

## Create a Pipeline Job
![Jenkins](images/pipeline-test.png)
![Jenkins](images/webview.png)