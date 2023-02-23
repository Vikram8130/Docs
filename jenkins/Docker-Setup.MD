## Install Docker
```sh
yum install docker
systemctl start docker
systemctl enable docker
chkconfig docker on -> to make sure docker remains online during the boot time.
```

## provide permissions to jenkins user in jenkins server to access docker
```sh
  sudo groupadd docker
  sudo usermod -aG docker jenkins -> adding jenkins inside the docker group 
  sudo chmod 777 /var/run/docker.sock
```
## Add Jenkins user into sudoers file to get sudo access
```sh
   vi /etc/sudoers
   jenkins ALL=(ALL) NOPASSWD: ALL
```   
   

