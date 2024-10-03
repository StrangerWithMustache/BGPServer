# BGPServer
---
### Using Centos.7.9.2009:  
  * Can be build through DockerFile given in "Centos.7.9.2009.DockerFile" directory.
  * 1 issue observed is that unable to start frr during build. Workaround is after image is created, start manually using below command and create another image.  
  * command: systemctl enable frr && systemctl start frr  
  * Can be use already created image: mozegunner/bgpserver:centos.7.9.2009  

### Using Ubuntu.20.04:
  * Can be build through DockerFile given in "Ubuntu.20.04.DockerFile" directory.
  * FRR service will not be started when deployed. Need to start manually below command.
    > '/etc/init.d/frr start'  
  * Can be use already created image: mozegunner/bgpserver:ubuntu.20.04  
  
