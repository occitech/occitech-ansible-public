# ElasticSearch

* approximative size: 160MB
* default port: 9200
* default ElasticSearch version: 7.3.2

## Usage

To known your local adress run command (using SSH)

```bash
echo $LOCALSERVER
```

You could try to access your ElasticSearch using curl

```bash
curl http://root:<elasticserch_pass>@<local_adress>:<elasticsearch_port>
```

To configure access to ElasticSearch UI, you need to create a new transparente redirect (reverse proxy) with the destination URL

```bash
http://<local_adress>:<elasticsearch_port>/
```
