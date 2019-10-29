One of several tools we use at Inspire is a system configuration tool known as Ansible, documentation can be found at https://docs.ansible.com/. We use Ansible to keep our linux systems up to date and configured according to our standards.

This purpose of this exercise is:
1. To give you a taste of what a day at Inspire as a sysadmin is like.
2. Give you the chance to show you can bootstrap yourself with a new technology

If any part of this exercise is unclear, please don't hesitate to ask us questions. If you feel it is taking more time to accomplish than you have to commit, please let us know that as well. Our goal is not to waste anyone's time, but to have a simple exercise everyone can learn from.

Please create an ansible playbook that can be run against an Ubuntu 18.04 Linux server and would do the following:
1) Install all updates
2) Create a new user account called “inspire”
3) Create a password for the “inspire” user, also set to “inspire”
4) Create a file in the "inspire" user's home folder called “inspire.txt” with the text “Inspire is awesome” inside the file.
5) Ensure that the apache web server is installed, is running, and starts up automatically if the system is rebooted.

The output of this exercise should be a single Ansible playbook. We will examine your playbook and test it against a fresh Ubuntu 18.04 linux virtual machine in EC2.
