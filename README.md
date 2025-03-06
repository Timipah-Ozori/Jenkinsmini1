Project Hightlighs 

## Gettings started with Jenkins 

Created an instance on AWS called Jenkins Server, with a public Ip address and granted SSH access to connect to the instance 

![](./img/1.%20Jenkins%20server.png) 

## Jenkins Installation 

`sudo apt update`

`sudo apt install openjdk-11-jdk`


![](./img/2.%20Jenkins%20install.png)



![](./img/3.%20Jenkins%20install.png)

   `` wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
    sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
    sudo apt update
    sudo apt-get install jenkins``



`sudo systemctl status jenkins`

## Jenkins is running 

![](./img/5.%20Jenkins%20installed.png)


# Security Group premission 

![](./img/6.%20sg.png)



# Admin Overview 

![](./img/6.%20Jenkins%20admin.png)


##  Installed suggested plugins and Created First admin user 




# Connect to Jenkins interface 

http://13.60.60.184:8080 - Ip address of the instance and port 

![](./img/6.%20Jenkins%20admin%20created.png)

