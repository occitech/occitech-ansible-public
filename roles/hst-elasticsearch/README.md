# ElasticSearch

* approximative size: 60MB
* default port: 9200
* default ElasticSearch version: 7.3.2

## Usage

To known your local adress run command (using SSH)
```
echo $LOCALSERVER
```

You could try to access your ElasticSearch using curl
```
curl http://root:<elasticserch_pass>@<local_adress>:<elasticsearch_port>
```

To configure access to ElasticSearch UI, you need to create a new transparente redirect (reverse proxy) with the destination URL

```
http://<local_adress>:<elasticsearch_port>/
```
