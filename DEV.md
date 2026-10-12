```bash
php -S localhost:8000
```

```bash
docker compose up
```

Follow guide on http://localhost:8000 with following db creds:

db URL: 127.0.0.1:3306
db user: matomo
db pass: dev_password
db: matomo

Here we go.

Run multiple tracking domains with the same script:

```
cd dev-target
npx http-server --port 8001
```

```
cd dev-target
npx http-server --port 8002
```

Navigate to localhost:8002, refresh, follow link to localhost:8001 on the page. This gives you a cross-domain visit.
