#### Give Sudo previleges to the user.
```
sudo useradd -s /bin/bash -d /opt/stack -m <username> 
```
```
$ echo "<username> ALL=(ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/<username>
$ sudo su - <username>
```


####
