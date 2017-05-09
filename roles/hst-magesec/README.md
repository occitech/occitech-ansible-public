# Mage Security Scanner

https://magesec.org

* source: https://github.com/magesec/magesecurityscanner
* approximative size: 1MB

## Usage

To launch scan on all your account run
```
mwscan --ruleset magesec ~/
mwscan --ruleset magesec ~/storage
```

To whitelist a file
```
sha1sum <FILE_PATH> >> ~/mwscan_whitelist.txt
```

To run scan using whitelist
```
mwscan -w ./mwscan_whitelist.txt --ruleset magesec ~/
```
