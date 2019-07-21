# nd9991_project_2

**To create the stack** Log on to Amazon AWS Console, locate the CloudFormation page. Click on **Create stack** then upload **nd9991-stack.yml** template file and enter the following under **Specify stack details**

- Stack name
- EnvironmentName
- KeyName


## Bastion Host:

Modify **SecurityGroupWeb**'s inbound rules as troubleshooting requires. For example,
allow **ICMP** inbound from 10.100.0.0/16 to allow PING, and allow **SSH** inbound from only 10.100.0.0/16 
to allow SSH into Private instances

Note. **KeyName** maybe removed from **WebServerLaunchCongi** and relaunch the stack for more security.