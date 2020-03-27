### Jenkins 👴

## What is a CI/CD pipeline?
- A CI/CD pipeline helps users automate steps in their software delivery process, such as initiating code builds, running automated tests, and deploying to a staging or production environment.


## Continuous Integration - CI:
Implementing Continuous Integration (CI) can reduce errors in code, shorten development cycle, where teams can build, test, and update their code within minutes, increasing quality and reducing time to production.


## What is automation server?

Automation Server: is an integrated solution that automates provisioning, patching, and configuration of operating systems, storage resources and application components across physical, virtual and public cloud systems.


## What to Use Jenkins for and When to Use It??

Jenkins is the leading open-source automation server. Built with Java,  which can be used to automate all sorts of tasks such as building, testing, and deploying software. Jenkins is commonly used for:

1. Building projects.
2. Running tests to detect bugs and other issues as soon as they are introduced.
3. Deployment.

* Execute repetitive tasks, save time, and optimise user development process with Jenkins.

## Create Virtual Machine and Install Java:
- Create Virtual Machine (Vagrant init, Vagrant up)
- Install Java
    'sudo apt install openjdk-8-jdk'

- Check the java version installed
    'java -version'
- Choose the default java to use (optional)
    'sudo update-alternatives --config java'

## Install Jenkins
1. First need to add the package key to  Ubuntu packaging system,

```
wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -

```

2.  Add the package repository to the source list so it gets updated when typing apt-get update and install Jenkins.

```
sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list

```
```
sudo apt-get update && sudo apt-get install jenkins

```


3. Unlock Jenkins
Now can open the browser of local host machine and visit localhost:8080. Should look like Welcome to Jenkins but it is ask for password.

- copy the link show, open the jenkins machine and from the terminal

```
sudo su
cat /var/lib/jenkins/secrets/initialAdminPassword

```
f99bbdf443534aa8a70de5bf04606060
copy the password and unlock jenkins.

*CONGRATS! JENKINS IS SUCCESSFULLY INSTALLED!!*


## Setup recommended plugins
On the next screen Jenkins will ask to setup default plugins or choose from a list of plugins. Setup the defaults to start.

## Jenkins User dashboard
After it finishes wait until it loads.
