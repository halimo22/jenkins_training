- What is the packages is a prerequisite for installing Jenkins ?
java 
- Run this command and tell me the ssh port: curl -Lv http://localhost:8085/login 2>&1 | grep -i 'x-ssh-endpoint'
8080

- What are jenkins plugins?

	A. Plugins are used to configure the security settings in Jenkins.
	B. Plugins are the primary means of enhancing the functionality of a Jenkins environment to suit organization or user specific needs.
	C. Plugins are used to create jobs in Jenkins.
	D. Plugins are the tools to setup CI/CD pipelines in Jenkins.

B
- Can we install the .hpi plugin file from Jenkins web UI?
Yes
- Make sure that Git and Github plugins are installed if it's not kindly install them
Done
- Install Jenkins as normal service or as docker container (bouns install it using ansible)
Done
- Under what location Jenkins store its data primarily?
/var/lib/jenkins
- Install and configure thinbackup plugin and make sure that the default dir for backup is: /var/lib/jenkins/jenkins_backup
Done
- Create a Jenkins user as per the details provided below.

	A. Username: jenkins
	B. Password: jenk!n$
	C. Full Name: Orange DevOps

![alt text](image.png)
- Install the Role-based Authorization Strategy plugin and enable the Role-Based Strategy authorization in Jenkins security settings.
![alt text](image-1.png)

- Install the Role-based Authorization Strategy plugin and enable the Role-Based Strategy authorization in Jenkins security settings.
![alt text](image-2.png)
- Create a role named developers and make sure it has overall Read permissions alone. Also assign role called developers to the user called jenkins.
![alt text](image-3.png)
![alt text](image-4.png)
- First, install the Matrix Authorization Strategy plugin and using the Project-based Matrix Authorization Strategy assign some permissions that would allow jenkins to build the mytest job.

![alt text](image-5.png)
	Once this is done, build this job through user jenkins.
	Note: You should use jenkins's credentials from the previous question.
	
		Username: jenkins
		Password: jenk!n$
![alt text](image-6.png)
- Install Pipeline Jenkins plugin?
![alt text](image-7.png)
- Create a pipeline job named hello-world, it should just echo the Hello World string.
![alt text](image-8.png)
- Install SSH Build Agents Jenkins plugin.
![alt text](image-9.png)
- Create a simple Jenkins job that prints "Hello, World!" in the console output.
	Set up a basic Freestyle job with a shell command to print a message.
![alt text](image-8.png)
- Configure a Jenkins job to pull code from a public GitHub repository.
	Use the Git plugin to connect to the repository and check out the latest code.
![alt text](image-10.png)
- Set up a Jenkins job that triggers every 5 minutes using the "Build periodically" option.
	Use the cron syntax to configure the trigger.
![alt text](image-11.png)
- Install a Jenkins plugin from the Plugin Manager.
	Pick any plugin (Docker) and verify that it's successfully installed.
![alt text](image-12.png)
- Configure a Jenkins job to send email notifications when a build fails.
	Set up the Email Extension Plugin and define an email recipient list.
![alt text](image-13.png)
- Create a Jenkins pipeline with two stages:
	Stage 1: Pull code from GitHub(repo from your choise)
	Stage 2: Run a simple shell script that lists all files in the workspace.
![alt text](image-14.png)
- Set up a Jenkins job to archive log files generated by the build.
	Use the "Archive the artifacts" post-build action to store the logs.
![alt text](image-15.png)
- Set up a Jenkins job to clean up old builds (e.g., only keep the last 5 builds).
	Configure the job to discard old builds using the "Discard Old Builds" option.
![alt text](image-16.png)
- Create a Jenkins job that takes user input for a name and prints a greeting message in the console output (e.g., "Hello, [Name]!" ).
	Use the "This build is parameterized" option and add a string parameter.
![alt text](image-17.png)
![alt text](image-18.png)
- Set up a Jenkins job to build a Java project using the javac command.
	Ensure the job compiles a basic Java file and outputs the result.
![alt text](image-19.png)
- Create a Jenkins job that runs a script to check for disk space usage on the Jenkins server.
	Use a simple shell script in the build step to check the disk space (df -h on Linux).
![alt text](image-20.png)
- Create a Jenkins job that executes a Python script from the repository search for a repo or create one.
	Ensure the job pulls the script from GitHub and runs it.
![alt text](image-21.png)
- Configure a Jenkins job that runs on an agent (slave) node with specific labels ("linux").
	Set up a node with a label and configure the job to run only on that node.
