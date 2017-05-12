# Airflow

Airflow

* presentation: http://nerds.airbnb.com/airflow/
* documentation: http://pythonhosted.org/airflow/

**WARNING:** default port (8080) is already used on our hosting, changed to 8088

* approximative size: 12MB
* default server port: 8088
* default server version: 1.8.0

## Usage

To known your local adress run command (using SSH)
```
echo $LOCALSERVER
```

To configure access to Airflow UI, you need to create a new transparent redirect (reverse proxy) site or add a proxy (example with auth below) into **Advanced Settings** box of an Apache standard site if you wand to add http authentification.

```
ProxyPreserveHost On
ProxyPass / http://<local_address>:<airflow_port>/
ProxyPassReverse / http://<local_address>:<airflow_port>/

<Location />
Order Deny,allow
Deny From All

AuthType Basic
AuthName "Restricted"
AuthUserFile "/home/<acount_name>/.htpasswd"
Require valid-user
Satisfy any
</Location>
```
