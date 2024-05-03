# Playbook2024
DevOps Simplified tasks
# Installing Maven in aws ec2
*1. Install Apache Maven on your EC2 instance. First, enter the following to add a repository with a Maven package*
   sudo wget https://repos.fedorapeople.org/repos/dchen/apache-maven/epel-apache-maven.repo -O /etc/yum.repos.d/epel-apache-maven.repo
*2. Enter the following to set the version number for the packages.*
sudo sed -i s/\$releasever/6/g /etc/yum.repos.d/epel-apache-maven.repo
*3. Then you can use yum to install Maven.*
sudo yum install -y apache-maven
