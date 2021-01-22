**Continous Integration Pipeline For Tooling Website**


Prerequisite

An NFS server with exports for mnt/opt

Network Information

- Jenkins  192.168.1.109

- NFS    192.168.1.143

- Web Server 1  192.168.1.223 


I will be building a Jenkins CI pipeline for a tooling website.




I Mounted /var/lib/ to store data on NFS
```sudo mount 192.168.1.143:/mnt/logs /var/log/apache2```

- After mounting to make sure the mount persists, i added the follwing to the /etc/fstab configuration

```192.168.1.116:/mnt/opt  /var/lib	 nfs  defaults   0 0```



- Set up the Jenkins server

I created a Jenkins server on Ubuntu 20.04