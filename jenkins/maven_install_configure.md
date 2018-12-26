Install Maven using the following command

sudo yum install maven -y


![maven_install_1](https://user-images.githubusercontent.com/20787443/50431077-0aaa5e00-0903-11e9-98bc-530d5a2f8353.PNG)

To check the version,once ,maven is installed.

mvn -version 

![maven_version_2](https://user-images.githubusercontent.com/20787443/50431080-10a03f00-0903-11e9-91bb-300ff68fb41a.PNG)

Set Java classpath .

To find where is your java present , run the below command.

$(dirname $(dirname $(readlink -f $(which javac))))


![maven_java_3](https://user-images.githubusercontent.com/20787443/50434155-5961f300-0917-11e9-8540-242fa4fb1b2a.PNG)


To setup Jenkins global configuration, click on Manage Jenkins>> Global Tools Configuration
![image](https://user-images.githubusercontent.com/20787443/50434298-d4c3a480-0917-11e9-9832-ca336b1425de.png) 


![jdk_1png](https://user-images.githubusercontent.com/20787443/50437078-5ff66780-0923-11e9-880e-dae56daeea10.PNG)
