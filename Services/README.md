Role Name - Services
====================

While applying system updates and patches helps correct known vulnerabilities, one of the best ways to protect the system against as yet unreported vulnerabilities is to disable all 87 | P a g eservices that are not required for normal system operation. This prevents the exploitation of vulnerabilities discovered at a later date. If a service is not enabled, it cannot be exploited. The actions in this section of the document provide guidance on some services which can be safely disabled and under which circumstances, greatly reducing the number of possible threats to the resulting system. Additionally some services which should remain enabled but with secure configuration are covered as well as insecure service clients.

In this Role We will be Ensuring Security from 'inetd services'. inetd is a super-server daemon that provides internet services and passes connections to configured services. While not commonly used inetd and any unneeded inetd based services should be disabled if possible.

And also we will be Ensuring some special purpose services like ntp, chrony, X windows, Avahi etc.

This Role has been created to Ensure various rules for providing better security in Linux Centos 7. The various rules are as follows :-
- Ensuring that chargen, daytime, echo, time are not active.
- Ensuring that rsh, talk, telnet-server, tftp, rsync are not enabled.
- Ensuring ntp is installed and configured.
- Ensuring chrony is installed and configured.
- Ensuring X Windows is not installed on machine.
- Removing Xwindows only if already installed.
- Ensuring that Avahi is not installed.
- Ensuring that DHCP, LDAP, DNS, FTP, HTTP, POP3, IMAP, Samba, NFS server are not enabled.

Role Variables
--------------

1. ntp: It is the path of the ntp configuration file.
2. sysconfig: It is the path of ntpd sysconfig file.
3. chrony: It is the path of the chrony configuration file.
4. chronyd: It is the path of the chronyd sysconfig file.

Dependencies
------------

As we are just Ensuring that some services are Enabled or not so for that purpose some services should be Installed already to perform the Action.
1. Centos 7
2. xinetd package - For inetd services like chargen, echo, datetime & time.
3. avahi package - For verifying that avahi daemon is not enabled.

Author Information
------------------

This role is created by Opstree Solutions to provide better security inside Centos version 7 for various services.
