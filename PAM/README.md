Role Name - Pluggable Authentication Modules (PAM)
==================================================

PAM (Pluggable Authentication Modules) is a service that implements modular authentication modules on UNIX systems. PAM is implemented as a set of shared objects that are loaded and executed when a program needs to authenticate a user. Files for PAM are typically located in the /etc/pam.d directory. PAM must be carefully configured to secure system authentication. While this section covers some of PAM, please consult other PAM resources to fully understand the configuration capabilities.

This Role has been created to Ensure various rules for providing better security in Linux Centos 7. The various rules are as follows :-
- Ensure PAM is installed
- Ensure password creation requirements are configured
- Ensure lockout for failed password attempts is configured & also ensuring password reuse is limited
- Ensure lockout for failed password attempts is configured & also ensuring password reuse is limited
- Ensure password expiration is 365 days or less
- Ensure inactive password lock is 30 days or less
- Ensure default group for the root account is GID 0
- Ensure root login is restricted to system console
- Ensure access to the su command is restricted

Role Variables
--------------

1. pwquality_conf: It is the path of the file where password creation recquirements are configured.
2. login_defs: It is the path of the file where we need to define password expiration is 365 days or less.
3. days: Value to set inactive password lock is 30 days or less.
4. GID: Value to set default group for the root account is GID 0.
5. admin_user: value to define the username for which to set default group for the root account is GID 0. 
6. securetty: It is a path of the file where we need to define root login is restricted to system console
7. su: It is a path of the file where we need to define access to the su command is restricted.
8. paswd_auth: It is a path of the file where we need to define lockout for failed password attempts is configured & also ensuring password reuse is limited.
9. system_auth: It is a path of the file where we need to define lockout for failed password attempts is configured & also ensuring password reuse is limited.

Dependencies
------------

Centos 7

Author Information
------------------

This role is created by Opstree Solutions to provide better security inside Centos version 7 Pluggable Authentication Module (PAM).
