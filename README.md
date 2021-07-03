# Deploy-app-with-ansible-docker
Creating infrastructure with ansible and docker deploying a simple app web and monitoring it.
In a single playbook, you will install the docker, download default images, configure the environment and resources so that a web application is presented and the docker environment monitored.
In these projects a standalone server with CentOS 8 installed and ansible was used.
The tools used are in addition to those already mentioned, Prometheus for monitoring the environment. 

The files are organized in the /srv directory for best use. The main file is "iac.yml", as the following tree image:

![image](https://user-images.githubusercontent.com/23237395/124341031-e8f35700-db8f-11eb-83ec-d41dfefc8d9a.png)


 From the /srv directory, just run the command: ansible-playbook iac.yml and the structure will be created.
 ![image](https://user-images.githubusercontent.com/23237395/124341129-b007b200-db90-11eb-9620-8e3eda5c56b1.png)


To access the application, just put the ip of the virtual machine in the browser and the web application message "Hello World" will be displayed. The application is configured to access the default port, port 80.

To access the monitoring, open the browser and enter the ip of the virtual machine along with the port and it will be 9090 and prometheus will open. Example: <IP host>:9090.

![image](https://user-images.githubusercontent.com/23237395/124340975-931eaf00-db8f-11eb-97d0-ed8a69977942.png)

 Monitoring
 ![image](https://user-images.githubusercontent.com/23237395/124341004-ba757c00-db8f-11eb-9c8d-5b54010e4852.png)

  
 
 
