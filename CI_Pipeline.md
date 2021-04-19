**Continous Integration Pipeline For Tooling Website on AWS**


Network Information

- Jenkins  172.31.32.87(Ubuntu 20.04 on AWS)

- NFS    172.31.36.217(Red Hat AMI)

- Web Server 1  172.31.36.79(Red Hat AMI)

- Web Server 2 172.31.41.116(Red Hat AMI)




**Install Jenkins server**


```sudo apt update```

```sudo apt install default-jdk-headless```




```wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -```

```sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \ /etc/apt/sources.list.d/jenkins.list'```


From my browser i opened http://18.133.196.30:8080
and inputed the password

![](https://github.com/drazen-dee28/Continous-Integration-Pipeline-For-Tooling-Website/blob/main/img/unlockjenk.png)



```sudo apt update```

```sudo apt-get install jenkins```

**Configure Jenkins to retrieve source codes from GitHub using Webhooks**

I enabled webhooks in my GitHub repository settings

![](https://github.com/drazen-dee28/Continous-Integration-Pipeline-For-Tooling-Website/blob/main/img/webhook.jpg)






CREDITS