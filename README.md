# Docker Drop

Docker Drop is a tiny click game built as a single static HTML file. Run it inside a Docker container to demo container basics.

## Build and run

```bash
docker build -t docker-drop .
docker run --rm -p 8080:80 docker-drop
```

Open <http://localhost:8080> in your browser and start clicking the orb.

## Elasticsearch deployment (Docker)

Spin up a single-node Elasticsearch container with Docker Compose:

```bash
docker compose -f docker-compose.elasticsearch.yml up -d
```

Verify it is running:

```bash
curl http://localhost:9200
```

Tear it down when you are done:

```bash
docker compose -f docker-compose.elasticsearch.yml down
```
