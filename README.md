
# Docker (volume) + Nginx + HTML

A simple project to apply the basics of Docker.

## How to start

Clone

```bash
  git clone https://github.com/SauloAlmeida/docker-volume-html
```

Go to directory

```bash
  cd docker-volume-html/app
```

Build a docker image with nginx

```bash
  docker build -t docker-volume-server server/.
```

Run a container and pass the resource folder to the volume

```bash
  docker run -v <PC_PATH>\app\resource:/usr/share/nginx/html -dp 8081:80 docker-volume-server
```

Go to: http://localhost:8081/