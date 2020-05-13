#### Give Sudo previleges to the user.
'''sudo useradd -s /bin/bash -d /opt/stack -m stack '''
''' $ echo "stack ALL=(ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/stack
$ sudo su - stack'''

