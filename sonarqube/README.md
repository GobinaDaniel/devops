# Installation de l'outil Jenkins

### creation de repertoire jenkins_data

```bash
mkdir -p ~/devops/sonarqube_data
mkdir -p ~/devops/sonarqube_extensions
mkdir -p ~/devops/sonarqube_logs
mkdir -p ~/devops/postgres_data
mkdir -p ~/devops/sonarqube_conf
```

### configuration du domaine local

```bash
sudo nano /etc/hosts
```

### Ajout du domain

```bash
127.0.0.1    sonarqube.local
```

### Commande pour ajouter le volume de sonarqube dans la machine

```bash
sudo sysctl -w vm.max_map_count=524288
sudo sysctl -w fs.file-max=131072
```

### Execution du service

```bash
docker-compose -f "sonarqube.yml" up -d --build
```
