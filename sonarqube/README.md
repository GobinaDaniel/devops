# Installation de l'outil Jenkins

### creation de repertoire jenkins_data

```bash
mkdir -p ~/devops/sonarqube_data
mkdir -p ~/devops/sonarqube_extensions
mkdir -p ~/devops/sonarqube_logs
mkdir -p ~/devops/postgres_data
mkdir -p ~/devops/sonarqube_conf
mkdir -p ~/devops/sonarqube_temp
```

### configuration du domaine local

```bash
sudo nano /etc/hosts
```

### Ajout du domain

```bash
127.0.0.1    sonarqube.local
```

### Configuration pour l'hôte Docker

```bash
sudo sysctl -w vm.max_map_count=262144
sudo sysctl -w fs.file-max=65536
ulimit -n 65536
ulimit -u 4096
```

### Execution du service

```bash
docker-compose -f "sonarqube.yml" up -d --build
```
