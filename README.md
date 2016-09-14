# Requirements
Ansible installed  
SSH credentials to machines you controlled

# How to use
```
git clone https://github.com/8bit-devops/ansible-lemp-stack.git
cd ansible-lemp-stack
```

Update SSH credentials in hosts file to match yours then

# Run playbook
```
ansible-playbook -i hosts/dev playbook-provision.yml -vv 
```

This will install on 1 or many machines on hosts file, then access http://web-ip for your LEMP stack  
MySQL root password is defined in roles/lemp/defaults/main.yml

## Output Information
MySQL: root/password  
DocumentRoot: /var/www/html  
Nginx 1.10.x, PHP-FPM 5.6
drush, composer
# ansible-lemp-stack-php7
