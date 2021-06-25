# Installation de l'outil CloudBeaver

### create du repertoire dbeaver

```bash
mkdir -p ~/devops/dbeaver
```

### Configuration d'un domain en local

```bash
sudo nano /etc/hosts
```

### Ajout du domain

```bash
127.0.0.1   dbeaver.local
```

### Execution du service

```bash
docker-compose -f "cloud-beaver.yml" up -d --build
```