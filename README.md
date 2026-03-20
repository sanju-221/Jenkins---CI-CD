Jenkins

Jenkins is a CI/CD open source tool which used to automate the building, testing, and deployment of software projects.

It enables DevOps teams to implement Continuous Integration (CI) and Continuous Delivery (CD) pipelines, accelerating development by automating repetitive tasks.

Jenkins is a Java based application so it requires Java to run

Refer: https://www.jenkins.io/doc/book/installing/linux/

Java installation:
```
sudo apt update
sudo apt install fontconfig openjdk-21-jre
java -version
```

Jenkins - Long Term Support release:
```
sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2026.key
echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt update
sudo apt install jenkins
```
To access the Jenkins GUI enable port 8080 in the security group.
