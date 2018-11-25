Gitea git repo that using Postrges backend and operating over HTTPS with self-signed SSL key. Please use 'env GIT_SSL_NO_VERIFY=true git ...' to accept self-signed certificate when using git.

Automation is for deploying on Debian 9 stretch. Vagrantbox image which used is 'generic/debian9'. Ansible version is 2.7.

Default Gitea users:

John Doe   johndoe/JohnDoe jdoe@example.com Administrator

Mary Smith marysmith/MarySmith msmith@example.com User

System and database credentianls are inside deploy.yml 'vars:' section.

Vagrant box uses Virtualbox internal network with NAT (not just simple NAT) so replace net name 'virtualbox__intnet: "NatNetwork"' to your own.
That was made for deploying software from one Linux VBOX machine to another Linux VBOX both located on the same Windows Virtualbox host.
