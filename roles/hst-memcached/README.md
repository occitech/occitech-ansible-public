# Memcached

Memcached server http://memcached.org/ and PHP module https://pecl.php.net/package/memcached

**WARNING:** do not work with PHP > 5.6.x for now
**WARNING:** you need to reinstall if you change PHP version (due to module compilation)

* size: 150MB
* default server port: 11212
* default server version: 1.4.34
* default PHP module version: 2.2.0

## Usage

To activate PHP module you need to add the following line to your php.ini
```
extension = /home/<YOUR_ACCOUNT_NAME>/memcached/src/memcached-2.2.0/modules/memcached.so
```

You could use the following telnet command to get access to your Memcached server
```
telnet $LOCALSERVER 11212
```
