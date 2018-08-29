# Redis

Redis server https://redis.io/ and PHP module https://pecl.php.net/package/redis

**WARNING:** you need to reinstall if you change PHP version (due to module compilation)

* size: 2MB
* default server port: 6379
* default server version: 2.4.15
* default PHP module version: 3.1.1

## Usage

To activate PHP module you need to add the following line to your php.ini
```
extension = /home/<YOUR_ACCOUNT_NAME>/redis.so
```

You could use the following telnet command to get access to your Redis server
```
telnet $LOCALSERVER 6379
```

Or use the Redis CLI
```
redis-cli -h $LOCALSERVER -p 6379
```