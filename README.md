
## WKS Platform Docker Compose Setup

This docker-compose configuration leverages pre-built images from the WKS Platform, offering a streamlined approach to quickly set up and deploy the platform on a development environment.

### Clone the Repository

```bash
git clone https://github.com/wkspower/wks-platform-docker.git
cd wks-platform-docker
```

### Start Docker Compose

You have two options to start the Docker Compose setup based on your requirements:

#### Option 1: Camunda 7

```bash
docker-compose -f docker-compose.yaml -f docker-compose.camunda7.yaml -f docker-compose.demo-data-loader.camunda7.yaml -f docker-compose.portal.yaml up -d --build
```

#### Option 2: Camunda 8

```bash
docker-compose -f docker-compose.yaml -f docker-compose.camunda8.yaml -f docker-compose.demo-data-loader.camunda8.yaml -f docker-compose.portal.yaml up -d --build
```

### Accessing Web Applications

After successfully running `docker-compose up` to start the Docker Compose configuration, it may take a while for all the web applications to finish their startup process. Once the startup is complete, you can access the following web applications:

#### WKS Platform Portal

You can access the WKS Platform Portal by opening your web browser and navigating to [http://localhost:3001](http://localhost:3001). Use the following credentials to log in:

- **Username**: demo
- **Password**: demo