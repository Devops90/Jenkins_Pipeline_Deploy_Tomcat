# Jenkins_Pipeline_Deploy_Tomcat
jenkins pipeline script to deploy war file into tomcat servr
- go to pipeline syntax click on ssh agent gitve username and privatekey(pem file) generate pipeline script
- if we get host key verification fail the we will add "-o StrictHostKeyChecking=no"
- scp syntax: scp sourcefilelocation username@ipaddress:desinationfolder location 
- if we get permission denaied when deploy into tomcat server webapps folder then we will change the webapps folder owner permission
- chown ec2-user:ec2-user /opt/apache-tomcat-8.5.57/webapps 
