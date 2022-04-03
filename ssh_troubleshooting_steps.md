# SSH troubleshooting basics 

* Location of ssh client.  

/etc/ssh/ssh_config. 

* Location of ssh server file

/etc/ssh/sshd_config

* Location of authorised keys

~/.ssh/authorized_keys

* check /etc/ssh/sshd_config or update for various options like password authentication setting, no password settings etc. 




**Important commands**


* to copy public key 

ssh-copy-id -i ~/.ssh/lan.pub username@machineip 

Note it will ask for username and password. 

* to ssh into remote machine

ssh -i ~/.ssh/{privatekey} username@machineip

* to generate key 

ssh-keygen
