# BGPServer
Using Centos.7.9.2009:  
  Can be build through DockerFile given in "Centos.7.9.2009.DockerFile" directory.  
  1 issue observed is that unable to start frr during build. Workaround is after image is created, start manually using below command and create another image.  
  command: systemctl enable frr && systemctl start frr  
  Or use already created image: mozegunner/bgpserver:centos.7.9.2009  
  
