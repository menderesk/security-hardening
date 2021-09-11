System Security hardening implements security hardenings for servers under your management with Ansible playbook.

This playbook provides:
- Makes root passwords stronger.
- Disables Ctrl+Alt+Delete.
- Install Aide for you to monitor system file and directory changes.
- Makes your password policies stronger.

Your Root Passwords become stronger. Also, these passwords are written to the file /root/strong_pass.yml on your Ansible control host. It creates a separate password for each of your servers and is encrypted with the SHA512 algorithm, allowing you to change the root password on your host.

Disabling Cltr+Alt+Delete, non-root users are prevented from rebooting the system.

You can see all changes in system files and directories by installing Aide. It is also ensured that all these reports are copied to the /var/reports directory of your Ansible control host. In addition, you can create a cron and provide Aide checks at regular intervals.

By disabling the weak feature, which includes the same pattern for your passwords, is less than eight characters, and allows other users, other than root, to create more secure passwords.

This playbook is currently at version 1.0 and is in development. The next version will include:

- Creating Grub and Grub2 password
- Encryption of disks
- Fixing RPC vulnerabilities in NFS v2 and v3 versions
- Removal of unnecessary device services (like cups)
- Carrying Aide Reports to Ansible control regularly
- Activation of the USB Guard application
- Creation of proactive monitoring with Zabbix
- Live Kernel Patch for RHEL, SLES distro.

This playbook has been tested on Ubuntu, Centos, Fedora and SUSE distributions.

You can contribute to the development of this tightening application by contributing.

Thank you for your interest.

E-mail: mendereskeskin@outlook.com
