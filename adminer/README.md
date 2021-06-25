# Installation de l'outil Adminer

### Creation du repertoire mysql_data

```bash
mkdir -p ~/devops/mysql_data
```

### Configuration d'un domain en local

```bash
sudo nano /etc/hosts
```

### Ajout du domain

```bash
127.0.0.1   adminer.local
```

### Execution du service

```bash
docker-compose -f "adminer.yml" up -d --build
```