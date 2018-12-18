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

![jenkins4](https://user-images.githubusercontent.com/20787443/50155702-b11faf00-02c4-11e9-8de0-e83a0ddce155.png)

5)Install Jenkins along with git and openjdk

yum install jenkins  java-1.8.0-openjdk-devel git -y

![jenkins5](https://user-images.githubusercontent.com/20787443/50155712-b67cf980-02c4-11e9-9445-bd1fceffac9a.png)

6)Enable jenkins to start on bootup

systemctl enable jenkins

![jenkins6](https://user-images.githubusercontent.com/20787443/50155717-bb41ad80-02c4-11e9-91cc-883b5a247b1b.png)

7)Start Jenkins

systemctl start jenkins

![jenkins7](https://user-images.githubusercontent.com/20787443/50155724-c0066180-02c4-11e9-996f-fcbc22bc7a6e.png)

8)Check the status of jenkins

systemctl status jenkins

![jenkins8](https://user-images.githubusercontent.com/20787443/50155729-c4cb1580-02c4-11e9-8c79-7f49f47dfbc8.png)

9)Try to check whether you can access jenkins by doing the following

http://Hostname:8080

![jenkins9](https://user-images.githubusercontent.com/20787443/50155734-ca286000-02c4-11e9-9861-f28573f1e838.png)


10)Go to the below path to get the initial admin password

/var/lib/jenkins/secrets/initialAdminPassword


![jenkins10](https://user-images.githubusercontent.com/20787443/50155743-ceed1400-02c4-11e9-9c6d-35261740bb64.png)

11)You will get the page called "Customize Jenkins"

Click on install Suggested Plugins

12)Once done, create the first admin user,click on Save and Continue


