We are now at a landing page, currently there are no jobs created.

![create_new_job_1](https://user-images.githubusercontent.com/20787443/50428509-3cb3c400-08f3-11e9-9ad3-5333639216a9.PNG)





Now click on create new job and write a new job name.In my case its test. And now select a freestyle project.

![image](https://user-images.githubusercontent.com/20787443/50428565-acc24a00-08f3-11e9-8daa-a893bb14d75a.png)

Provide a description for the job.

![create_new_job_3](https://user-images.githubusercontent.com/20787443/50428700-a2ed1680-08f4-11e9-903a-76b69460047f.PNG)

Now click on discard old builds.Build jobs consume a lot of disk space and memory especially if you are storing artifacts.This option will help you in limiting the the number of builds you record in the build history.You can either tell Jenkins to only keep recent
builds or to keep no more than a specified number of builds.

![create_new_job_4](https://user-images.githubusercontent.com/20787443/50428745-e3e52b00-08f4-11e9-9dee-d10b13cc8d88.PNG)

The first section is SCM pr Source Control Management, which defines the source of the code to build the job.Currently we could see that it has SVN and Github plugins installed as part of the Jenkins Default Plugins.For this job, we are selecting None.

![create_new_job_5png](https://user-images.githubusercontent.com/20787443/50429117-3fb0b380-08f7-11e9-81a5-e13a9e59c6cb.PNG)

For this job, we are going to trigger the build manually, hence go to Build section and click on Execute Shell, you can also execute Windows Batch Command if you are on Windows. But I am going to select as I am on Linux

![create_new_job_6](https://user-images.githubusercontent.com/20787443/50429218-09bfff00-08f8-11e9-913a-0b7155578f93.PNG)


Currently we are going to write a basic echo statement.

![create_new_job_8](https://user-images.githubusercontent.com/20787443/50429683-ddf24880-08fa-11e9-9264-97e9f1a7cb86.PNG)


![create_new_job_9](https://user-images.githubusercontent.com/20787443/50429928-ebf49900-08fb-11e9-8d56-a26d12c08cf3.PNG)


![create_new_job_10](https://user-images.githubusercontent.com/20787443/50429932-eeef8980-08fb-11e9-807b-c08d828f6b3a.PNG)
