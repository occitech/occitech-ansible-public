# Odoo

Role to install a fresh Odoo

* approximative size: 600MB

## Usage

Run the playbook a first time to init project, create a PostreSQL database and configure your website like that:
* Type: User program
* Command: ./odoo-run -d <DATABASE_NAME> -r <DATABASE_USER> -w <DATABASE_PASS> --db_host <DATABASE_HOST> --no-database-list --proxy-mode --addons-path=addons --http-interface $ALWAYSDATA_HTTPD_IP --http-port $ALWAYSDATA_HTTPD_PORT
* Working directory: <ODOO_PATH>/src
* Environment: PYTHON_VERSION=3.6.5

Default odoo users account:
* admin / admin
* demo / demo