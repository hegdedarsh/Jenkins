1)Check whether wget is installed

  which wget
  
  ![jenkins1](https://user-images.githubusercontent.com/20787443/50155536-38205780-02c4-11e9-945c-a883de09e6bc.png)

2)Switch to root user

   sudo su -
   
   ![jenkins2](https://user-images.githubusercontent.com/20787443/50155691-a6fdb080-02c4-11e9-9c76-f3460d5b2076.png)
   
3)wget the jenkins repo

wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo

![jenkins3](https://user-images.githubusercontent.com/20787443/50155698-ac5afb00-02c4-11e9-9b84-89630f1cd74e.png)

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


