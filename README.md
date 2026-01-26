## 👋 Welcome to pocketbase 🚀

Open-source backend in one file (database, auth, file storage)

## 📋 Description

Open-source backend in one file (database, auth, file storage)

## 🚀 Services

- **app**: ghcr.io/muchobien/pocketbase:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/pocketbase/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/pocketbase" ~/.local/srv/docker/pocketbase
cd ~/.local/srv/docker/pocketbase
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install pocketbase
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
ENCRYPTION_KEY=changeme_encryption_key
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:8090

## 📂 Volumes

- `./rootfs/data/db/pocketbase` - Data storage
- `./rootfs/data/pocketbase/hooks` - Data storage
- `./rootfs/data/pocketbase/public` - Data storage
- `./rootfs/config/pocketbase/initdb` - Data storage

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
