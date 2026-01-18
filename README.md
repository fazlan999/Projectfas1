# Docker Drop

Docker Drop is a tiny click game built as a single static HTML file. Run it inside a Docker container to demo container basics.

## Build and run

```bash
docker build -t docker-drop .
docker run --rm -p 8080:80 docker-drop
```

Open <http://localhost:8080> in your browser and start clicking the orb.
