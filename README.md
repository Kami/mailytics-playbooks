# Mailytics Ansible Playbooks

## Available Playboks

* `web_servers.yml` - Webapp + PostgreSQL + API service
* `cassandra_servers.yml` - Cassandra
* `token_storage_servers.yml` - Token storage service
* `worker_servers` - Worker jobs

## Development environment information

* Webapp admin panel - admin / admin
* Pgbouncer user - mailyticswebapp / dev

## Notes

### Using django runserver for rapid iteration

```bash
source /data-deploy/mailytics/virtualenv/bin/activate
cd /data/mailytics/webapp
./scripts/flush-db.sh
python mailytics/manage.py runserver 0.0.0.0:8000
```
