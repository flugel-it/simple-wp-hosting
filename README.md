# simple-wp-hosting

## Overview
Automatic deployment of LEMP stack with (mostly) default configuration.

## Common usage:
Run
```
ansible-galaxy install geerlingguy.php geerlingguy.nginx geerlingguy.mysql
ansible-playbook playbook.yml
```
## Usage with Vagrant: 
Run `vagrant up`
Run `vagrant ssh`
![ip a](https://khomutsky.com/files/images/vagrant_ip.png "Interfaces")
Copy IP address of interface number 2, and place into `hosts` file.
### GNU/Linux, Unix and OS X:

Add the following line to `/etc/hosts`

`192.168.121.223 example.com`

### Windows:
Add the following line to `C:\Windows\drivers\etc\hosts`:

`192.168.121.223 example.com`

Replace `192.168.121.223` with IP you copied in previous step.
Go to example.com. In case of successful provision you should get php info.
![phpinfo](https://khomutsky.com/files/images/phpinfo.png "PHPInfo")

