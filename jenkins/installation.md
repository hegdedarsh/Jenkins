1)Check whether wget is installed

  which wget

2)Switch to root user

   sudo su -
   
3)wget the jenkins repo

wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo


4)Import the jenkins key

rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key

5)Install Jenkins along with git and openjdk

yum install jenkins  java-1.8.0-openjdk-devel git -y


6)Enable jenkins to start on bootup

systemctl enable jenkins

7)Start Jenkins

systemctl start jenkins

8)Check the status of jenkins

systemctl status jenkins


9)Try to check whether you can access jenkins by doing the following

http://Hostname:8080


10)Go to the below path to get the initial admin password

/var/lib/jenkins/secrets/initialAdminPassword

11)You will get the page called "Customize Jenkins"

Click on install Suggested Plugins

12)Once done, create the first admin user,click on Save and Continue

