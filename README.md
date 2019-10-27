# docker-compose-nextcloud

## Requrements

* docker
* docker-compose

## Running

### First run

1. Copy .env files and change them according your needs

```bash
cp .app.env app.env
cp .db.env db.env
```

2. Start the stack

```bash
docker-compose up -d
```
### Upgrade

1. Rebuild

```bash
docker-compose build --pull
```

2. Restart

```bash
docker-compose up -d
```
