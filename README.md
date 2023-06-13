# CI-CD-for-springboot-application
Using Jenkins CI/CD to automate the deployment of a spring-boot application  

## To run :  
Install Jenkins & configure. If using an EC2 instance, choose a t2.medium at least  
Install Java 17 (requirement to run app) [ https://devopscube.com/install-maven-guide/ ]  
$ sudo yum install java-17-amazon-corretto-devel -y  
$ java --version   	--> to confirm installation of Java 17  
Create new pipeline. Copy & paste this script in the pipeline script field. Save & Build  
A manual approval has been added to the script. Make sure to approve the deployment by clicking 'proceed'  
Check browser at IP:8080  

![PetClinic __](https://github.com/Lily-G1/CI-CD-for-springboot-application/assets/104821662/f8b40144-c724-4f5a-8259-130ac12de66e)

