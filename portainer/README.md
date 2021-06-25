# Installation de l'outil portainer

### creation de repertoire portainer_data

```bash
mkdir -p ~/devops/portainer_data
```

### configuration du domaine local

```bash
sudo nano /etc/hosts
```

### Ajout du domain

```bash
127.0.0.1    portainer.local
```

### Execution du service

```bash
docker-compose -f "portainer.yml" up -d --build
```
