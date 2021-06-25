# Mise en place de l'outil Nginx Proxy Manager en local

### Creation des repertoires

```bash
mkdir -p ~/devops/nginx/data
mkdir -p ~/devops/nginx/letsencrypt
mkdir -p ~/devops/nginx/storage
```

### Configuration d'un domain en local

```bash
sudo nano /etc/hosts
```

### Ajout du domain qui nous permettra d'accéder facilement ) notre nginx-prox-manager

```bash
127.0.0.1   nginxproxymanager.local
```

### Creation du network qui sera utilisé par tous les outils qui seront mis en place

```bash
docker network create devops_nginx_network
```

### Execution du service

```bash
docker-compose up -d --build
```

### Information de connexion

```bash
- username/password: admin@example.com/changeme
```

