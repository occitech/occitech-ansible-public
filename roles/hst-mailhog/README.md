# Mailhog

Mailhog is a SMTP server useful for testing https://github.com/mailhog/MailHog

* approximative size: 13MB
* default SMTP port: 1032
* default UI pour: 8032
* default Mailhog version: 0.2.1

## Usage

To known your local adress run command (using SSH)

```bash
echo $LOCALSERVER
```

Set your app to deliver mail using SMTP on your local address and Mailhog SMTP port instead of your default SMTP settings.  
If you use a PHP app, you could configure **sendmail_path** to use **mhsendmail** for sending mail.

```bash
sendmail_path='/home/<acount_name>/bin/mhsendmail  --smtp-addr="<local_address>:<mailhog_port>"'
```

To configure access to Mailhog UI, you need to create a new transparent redirect (reverse proxy) site or add a proxy (example with auth below) into **Advanced Settings** box of an Apache standard site.

```conf
ProxyPreserveHost On
ProxyPass /mail/ http://<local_address>:<mailhog_port>/
ProxyPassReverse /mail/ http://<local_address>:<mailhog_port>/

<Location /mail>
Order Deny,allow
Deny From All

AuthType Basic
AuthName "Restricted"
AuthUserFile "/home/<acount_name>/.htpasswd"
Require valid-user
Satisfy any
</Location>
```
