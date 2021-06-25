# Installation de l'outil Jenkins

### creation de repertoire jenkins_data

```bash
mkdir -p ~/devops/jenkins_data
```

### configuration du domaine local

```bash
sudo nano /etc/hosts
```

### Ajout du domain

```bash
127.0.0.1    jenkins.local
```

### Execution du service

```bash
docker-compose -f "jenkins.yml" up -d --build
```
