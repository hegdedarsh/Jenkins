Install Maven using the following command

sudo yum install maven -y


![maven_install_1](https://user-images.githubusercontent.com/20787443/50431077-0aaa5e00-0903-11e9-98bc-530d5a2f8353.PNG)

To check the version,once ,maven is installed.

mvn -version 

![maven_version_2](https://user-images.githubusercontent.com/20787443/50431080-10a03f00-0903-11e9-91bb-300ff68fb41a.PNG)

Set Java classpath .

To find where is your java present , run the below command.

$(dirname $(dirname $(readlink -f $(which javac))))


When you check the maven version,you will see that the path is already defined, hence use it.

![maven_java_3](https://user-images.githubusercontent.com/20787443/50434155-5961f300-0917-11e9-8540-242fa4fb1b2a.PNG)


To setup Jenkins global configuration, click on Manage Jenkins>> Global Tools Configuration
![image](https://user-images.githubusercontent.com/20787443/50434298-d4c3a480-0917-11e9-9832-ca336b1425de.png) 


![jdk_1png](https://user-images.githubusercontent.com/20787443/50437078-5ff66780-0923-11e9-880e-dae56daeea10.PNG)

Based on the maven version command we executed above, we can see the MAVEN_HOME path, use it.

![maven_path_1](https://user-images.githubusercontent.com/20787443/50437079-5ff66780-0923-11e9-99fb-4b5357f12f71.PNG)

 Execute the below command .Based on this you will get the GIT_HOME path
 
 which git
 
 
 
![git_1_path](https://user-images.githubusercontent.com/20787443/50437125-8916f800-0923-11e9-8862-d27c9bc14f6d.PNG)

Once this is done, click save.

Create new job and name it Maven-Project.Make sure you select Git and provide the url you need to package which should contain your artifacts and pom.xml file.
![image_1](https://user-images.githubusercontent.com/20787443/50461800-f9715800-09bb-11e9-8400-770c9e5602cb.PNG)

In the build tab, click on invoke top-level maven targets, and provide the goals 

![image_2](https://user-images.githubusercontent.com/20787443/50461802-fb3b1b80-09bb-11e9-97b5-a17f9c51c4e7.PNG)

Once this is done, save it and run the job and check for the output.It should be success.
![image_3](https://user-images.githubusercontent.com/20787443/50461803-fc6c4880-09bb-11e9-9aca-813836fe7d7f.PNG)
