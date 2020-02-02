Role Name
=========

Installs msmtp as a simple solution for sending mails from managed servers.

Requirements
------------

No special requirements.

Role Variables
--------------

* msmtp_account_name: internal name of your email account
* msmtp_account_host: hostname of mail server
* msmtp_account_port: port to use for connecting mail server
* msmtp_tls: on/off wether to use TLS or not
* msmtp_tls_starttls: on/off wether to use STARTTLS or not
* msmtp_tls_trust_file: default: /etc/ssl/certs/ca-certificates.crt
* msmtp_account_from: from address to be used when sending mails
* msmtp_account_auth: on/off wether to use authentication
* msmtp_account_user: user account used to connect to mail server
* msmtp_account_password: password to be used for connecting to server
* msmtp_root_mail_receiver: mails for root and default are send to this email address

Dependencies
------------

No dependencies

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: msmtp }

License
-------

GPL v3

Author Information
------------------

ab@andreasbehnke.com
