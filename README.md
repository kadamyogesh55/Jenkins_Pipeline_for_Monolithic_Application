# Jenkins_Pipeline_for_Monolithic_Application

In this project I have deployed simple java based application into Tomcat server using Jenkins pipeline. Below tools are integrated with this pipeline:
- Git: Application code repository
- SonarQube: Static Code Analysis
- Maven: To build code into package and create artifact
- Nexus: Backup repository for release candidate and artifact
- Tomcat: Deployments server for realease candidate or artifact

## Steps
1.Create total 4 EC2 instances of Amazon Linux 2 with t2.medium

2.On 1st server: (Jenkins)
- Install jenkins (with java 17)
- Install Git
- Install maven (with java 11)
- Configure jenkins

3.On 2nd Server: (SonarQube)
- Install sonarqube with java 11
- Configure sonarqube

4.On 3rd server: (Nexus)
- Install nexus with java 11
- Configure nexus

5.On 4th Sever: (Tomcat)
- Install tomcat with java 11
- configure tomcat
- **tomup** and **tomdown** soft link for starting and stoping tomcat server

6.Add jenkins user to in tomcat server and give sudo privileges to jenkins user

7.Configure passwordless authentication from jenkins to tomcat server

8.On Github modify pom.xml for SonarQube and Nexus 



## Jenkins Pipeline
Configure sonarqube
4.On 3rd server: (Nexus)

Install nexus with java 11
Configure nexus
5.On 4th Sever: (Tomcat)

Install tomcat with java 11
configure tomcat
tomup and tomdown soft link for starting and stoping tomcat server
6.Add jenkins user to in tomcat server and give sudo privileges to jenkins user

7.Configure passwordless authentication from jenkins to tomcat server

8.On Github modify pom.xml for SonarQube and Nexus

## Jenkins Pipeline
![image](https://github.com/user-attachments/assets/ccd24ec5-d112-4c35-93dc-9626776dd360)
## SonarQube Static Code Analysis
![image](https://github.com/user-attachments/assets/2b935b0d-ab9e-4f63-a629-dfce7ded3235)
## Nexus Artifact Upload
![image](https://github.com/user-attachments/assets/2bf1c0b4-95f2-498e-a50c-ad69dc459c77)
## Deployment in Tomcat Server
![image](https://github.com/user-attachments/assets/d87e97ff-7241-4523-b688-9ed0fb271404)
## Web Application
![image](https://github.com/user-attachments/assets/2c65936b-f4fc-44f3-b1e1-da8e579b82df)




