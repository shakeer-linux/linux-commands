#### Give Sudo previleges to the user.
```
sudo useradd -s /bin/bash -d /opt/stack -m <username> 
```
```
$ echo "<username> ALL=(ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/<username>
$ sudo su - <username>
```


#### List all tags for a Docker image on a remote registry?
```
root@ubuntu:~/k8s4/Prometheus-Monitoring-with-k8_bkp_working# wget -q https://registry.hub.docker.com/v1/repositories/prom/prometheus/tags -O -  | sed -e 's/[][]//g' -e 's/"//g' -e 's/ //g' | tr '}' '\n'  | awk -F: '{print $3}'
latest
0.16.0
0.16.0rc1
0.16.0rc2
```


