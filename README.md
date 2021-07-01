# AWS
Ultimate AWS Certified Solutions Architect Associate 2021

ec2-user-data.sh
#!/bin/bash
# Use this for your user data(script from top to bottom)
# install httpd (Linux 2 version)
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable htttpd
echo "<h1>Hello World from $(hostname -f)</h1>" > /var/www/html/index.html