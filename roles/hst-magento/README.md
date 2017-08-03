# Magento 1

Role to install a fresh Magento 1, by default it use the following value (where <ACCOUNT> is your account hosting name):
* url: http://<ACCOUNT>.occitech.eu
* backoffice: http://<ACCOUNT>.occitech.eu/admin_<ACCOUNT>
* admin user: <ACCOUNT>
* admin pass: tobechang3d!

**WARNING**: destination path and database will be erased during installation

* approximative size: 600MB

**Prerequisite**: before installation you need to configure PHP to use 5.6 version with the following paramters
```
memory_limit=256M
extension=zip.so
extension=xsl.so
extension=soap.so
opcache.enable=1
opcache.memory_consumption = 128M
opcache.interned_strings_buffer=16
opcache.max_accelerated_files=100000
opcache.fast_shutdown=1
```
