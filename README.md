# CONTINOUS INTEGRATION WITH JENKINS


##Services used:

- Git & github

- Jenkins

- Java code plus Maven for building

- Checkstyle for code analysis

- Slack for notification

- Email notification

- Nexus as the repository to store artifact

- Sonarqube  for continuous inspection of code quality
and as well using the scanner to scan my code and publish the code in Sonarqube dashboard

- AWS EC2 server was used

.............................................................................................

### OBJECTIVE

- Fault isolation

- Short MTTR

- Faster turn around time to code changes

- Less disruption

................................................................................................
### FLOW OF EXECUTION


1. Login to AWS console

2. create key pair


3. create SG for jenkins, Nexus, Sonarqube


4. create EC2 instances with userdata  and it will provision jenkins, Nexus, Sonarkqube


5. Post installation


6. Jenkins setup and plugin


7. Nexus setup and repo setup


8. Sonarqube login test


9. Create a github repo and migrate code


10. Build job with Nexus integration


11. Github Webhook


12. Sonarqube server integration stage


13. Slack artifact upload stage


14. Slack Notification integration with Jenkins


