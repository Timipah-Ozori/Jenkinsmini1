## Project Purpose:
The purpose of this project is to set up an Instance on AWS to Install and set up jenkins.

Project Objective: 

1. Deploy a jenkins server on AWS using EC2 instance
2. Install Java, Jenkins and other packages
3. Ensure successful connection to jenkins via the web browser and create admin user.

## Project Requirements
1. Compute: AWS EC2 instance for hosting Jenkins
2. Networking: Creating inbound rules for SSH connection on port 22 to run installations and Custom TCP port on 8080 to connect throught the web browser



Step 1:

Installing and configuring jenkins on AWS EC2 Instance
 

## Create instance on AWS called Jenkins Server, with a public IP address and granted SSH access to connect to the instance to install java, jenkins on the command line. 

![](./img/1.%20Jenkins%20server.png) 


Step 2. Granted SSH access to connect to the instance 

![](./img/6.sg%20ssh.png)

Step 3. Java installation 

`sudo apt update`

`sudo apt install openjdk-11-jdk`


![](./img/2.%20Jenkins%20install.png)



![](./img/3.%20Jenkins%20install.png)


## Step 4. Jenkins Installation 

   `` wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
    sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
    sudo apt update
    sudo apt-get install jenkins``

### Start Jenkins Service 

`sudo systemctl status jenkins`

## Jenkins installed and is running 

![](./img/5.%20Jenkins%20installed.png)


# Security Group allow access to port 8080 for jenkins UI 

![](./img/6.%20sg.png)



# Admin Overview 

![](./img/6.%20Jenkins%20admin.png)


##  Installed suggested plugins and Created First Admin user 


# Connect to Jenkins interface

http://13.60.60.184:8080 - IP address of the instance and port 


## Jenkins is running and accessible via the web UI


![](./img/6.%20Jenkins%20admin%20created.png)

