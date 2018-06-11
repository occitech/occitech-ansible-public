# Magento 2

Role to install a fresh Magento 2

**WARNING**: detination path and database will be erased during installation

* approximative size: 760MB

**Prerequisite**: before installation you need to configure PHP to use 7 version with the following paramters
```
memory_limit=256M
extension=zip.so
extension=xsl.so
opcache.enable=1
opcache.memory_consumption = 128M
opcache.interned_strings_buffer=16
opcache.max_accelerated_files=100000
opcache.fast_shutdown=1
```

And add this line to your site **Advanced Settings**
```
LoadModule version_module /usr/alwaysdata/apache/2.2.32/modules/mod_version.so
```