# CI-CD-for-springboot-application
Using Jenkins CI/CD to automate the deployment of a spring-boot application  

## To run :  
- Install Jenkins & configure. If using an EC2 instance, choose a t2.medium at least  
- Install Java 17 (requirement to run app). [See here](https://devopscube.com/install-maven-guide/)  
  - $ sudo yum install java-17-amazon-corretto-devel -y  
  - $ java --version   	--> to confirm installation of Java 17  
- The application runs on port 8080, and so does Jenkins. This would cause an error on deployment. You can change the default port for Jenkins through the ffg:  
  - In Jenkins server terminal, open this file: /usr/lib/systemd/system/jenkins.service  
  - Locate "Environment="JENKINS_PORT=8080" and change 8080 to any port you desire. Save file   
  - $ systemctl daemon-reload  
  - $ systemctl restart jenkins.service     --> to reload/restart the Jenkins service  
  - Allow the new port in security group settings  
  - Access Jenkins on browser with new port e.g IP:8081  

- Create new pipeline in Jenkins. Copy & paste the script in the pipeline script field. Save & Build  
- A manual approval has been added to the pipeline. Make sure to approve the deployment by clicking 'proceed'  
- Check browser at IP:8080  

![PetClinic __](https://github.com/Lily-G1/CI-CD-for-springboot-application/assets/104821662/3ef68896-e4dd-4690-abb0-af9b71c74fc9)


