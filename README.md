# DHIS2 Central Log Console

A repository for a reference DHIS2 logging server console.

## Installation

1. Install recent Docker.

2. Download and launch the configuration

```shell
git clone https://github.com/dhis2-sre/dhis2-console.git /opt/console
cd /opt/console
echo "OPENSEARCH_ADMIN_PASS=$(openssl rand -base64 12)" > .env
docker compose up -d
```

3. For production use, change default passwords for all users in your OpenSearch setup
