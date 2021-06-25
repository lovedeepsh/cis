Role Name - SSH Secure Configurations
=====================================

SSH is a secure, encrypted replacement for common login services such as telnet , ftp , rlogin , rsh , and rcp . It is strongly recommended that sites abandon older clear-text login protocols and use SSH to prevent session hijacking and sniffing of sensitive data off the network.

Once all configuration changes have been made to /etc/ssh/sshd_config , the sshd configuration must be reloaded: "service sshd reload"

This Role has been created to Ensure various rules for providing better security in Linux Centos 7. The various rules are as follows :-
- Ensure permissions on /etc/ssh/sshd_config are configured
- Ensure SSH Protocol is set to 2
- Ensure SSH LogLevel is set
- Ensure SSH root login is disabled
- Ensure SSH Idle Timeout Interval is configured
- Ensure SSH Idle Timeout Interval is configured
- Ensure SSH access is limited


Requirements
------------

The recommendations in this section only apply if the SSH daemon is installed on the system.

Role Variables
--------------

1. sshd_config: This stores the path of ssh_configd file.

Dependencies
------------

1. Centos 7
2. SSH Daemon


Author Information
------------------

This role is created by Opstree Solutions to provide better security inside Centos version 7 for SSH secure configurations.
