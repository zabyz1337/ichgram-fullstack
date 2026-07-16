# ICHgram Fullstack

Fullstack social network built with React, Express, MongoDB and Docker.

---

## Technologies

- React
- Vite
- Express.js
- MongoDB
- Docker
- Docker Compose

---

## Requirements

Before starting, install:

- Git
- Docker Desktop

Check Docker installation:

```bash
docker --version
docker compose version
```

---

## Clone project

```bash
git clone --recurse-submodules https://github.com/zabyz1337/ichgram-fullstack.git
cd ichgram-fullstack
```

If submodules were not downloaded:

```bash
git submodule update --init --recursive
```

---

## Start application

Build containers:

```bash
docker compose up --build
```

or run in background:

```bash
docker compose up -d --build
```

Stop containers:

```bash
docker compose down
```

Rebuild after changes:

```bash
docker compose up --build
```

---

## Application

Frontend

```
http://localhost:5173
```

Backend API

```
http://localhost:5000
```

MongoDB

```
mongodb://localhost:27017
```

---

## Demo data

After the containers are running, populate a new database with demo users,
posts, comments, likes, notifications and messages:

```bash
docker compose exec backend npm run seed
```

The command is safe to run again: if the demo account already exists, no data
is changed and no duplicates are created.

Demo login:

```
Email: demo@ichgram.test
Password: Demo123!
```

The demo account is displayed as **Daniel Weber** (`daniel.weber`). The seed
also creates the `itcareerhub` profile, its six JPEG posts, conversations,
likes and comments.
