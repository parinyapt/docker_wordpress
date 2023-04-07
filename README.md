# Run Wordpress with Docker Compose

## Getting Started
#### Step 1: Add Environment Variable on .env file
```env
DB_ROOT_PASSWORD=root123
DB_USERNAME=user1
DB_PASSWORD=user1pwd
DB_NAME=wordpress_db
WEB_SERVER_PORT=8888
PHPMYADMIN_PORT=8889
NETWORK_NAME=wordpress_network
```
or
```bash
cp .env.template .env
```

#### Step 2: Create Docker Network
```bash
docker network create {NETWORK_NAME}
```

#### Step 3: Run Docker Compose
```bash
docker-compose up -d
```

> By Parinya Termkasipanich