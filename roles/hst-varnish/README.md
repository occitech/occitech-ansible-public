# Varnish Cache

Provide frontend cache to your website

* documentation: https://varnish-cache.org/
* approximative size: 10MB

## Usage

Run the playbook a first time to init project and configure your website like that:

* Type: User program
* Command: ~/varnish/sbin/varnishd -a $IP:$PORT -F -n ~/varnish/workdir -f ~/varnish/magento2.vcl
* Working directory: varnish/workdir

Some sample configuration files are availables into the Varnish **share/doc/varnish** docs folder.
