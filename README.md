# Arbeitsweise

## Pushen auf Dockerhub

1. fehlerlose Ausführung des Programms auf dem eigenen Rechner

Zunächst einmal muss man sicherstellen, dass das Programm auf dem eigenen Rechner läuft.

Bei dieser Webanwendung teste ich dies mit `npm run build; npm run start` und öffne dann den Browser auf `localhost:3000`.

2. Testen des Programms in einem Docker-Container

3. Dockerhub repository erstellen

4. Github actions einrichten

## Pushen auf Github Registry

### 1. Pipeline erstellen

### 2. Github Actions secrets einrichten

![secrets](./docs/add-github-secrets-ghcr.png)

### 3. Resultat

![ghcr](./docs/ghcr-result.png)

![alt text](image.png)

## Pushen und Deployen auf AWS

### 1. AWS ECR repository erstellen

![ECR](./docs/create-aws-ecr.png)

### 2. Pipeline erstellen

### 3. AWS ECS Task Definition erstellen

![Task Definition](./docs/add-aws-task-definition.png)

### 4. AWS ECS Cluster erstellen

![Cluster](./docs/add-aws-ecs-cluster.png)

## 5. AWS ECS Service erstellen

![Service](./docs/add-aws-ecs-service.png)

### 6. Github Actions secrets und variables einrichten

#### Secrets

![aws details](./docs/aws-details.png)

![secrets](./docs/add-github-secrets.png)

#### Variabels

![variables](./docs/add-github-variables.png)

### 7. Result

![show load balancer endpoint](./docs/aws-service-show-alb-endpoint.png)

![running](./docs/aws-refcard-03.png)
