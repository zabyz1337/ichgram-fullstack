# ICHgram Fullstack

Fullstack social network project built with React, Express and MongoDB.

## Requirements

- Git
- Docker Desktop

## Clone

```bash
git clone --recurse-submodules https://github.com/zabyz1337/ichgram-fullstack.git
cd ichgram-fullstack
```

## Start

```bash
docker compose up --build
```

## Application

Frontend:

```text
http://localhost:5173
```

Backend:

```text
http://localhost:5000
```

MongoDB:

```text
mongodb://localhost:27017/ichgram
```

## Stop

```bash
docker compose down
```

## Remove database data

```bash
docker compose down -v
```