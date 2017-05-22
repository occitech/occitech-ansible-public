# Magento

Role to install a fresh Magento 1

* approximative size: 0MB

WARNING: before installation you need to configure PHP to use 5.6 version with the following paramters
```
memory_limit=256M
extension=zip.so
extension=xsl.so
extension=soap.so
zend_extension=/usr/languages/php/5.5.30/lib/php/extensions/no-debug-non-zts-20121212/opcache.so
opcache.enable=1
opcache.memory_consumption = 128M
opcache.interned_strings_buffer=16
opcache.max_accelerated_files=100000
opcache.fast_shutdown=1
```
