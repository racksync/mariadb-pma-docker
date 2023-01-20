# Deploy MariaDB and PhpMyAdmin with Docker Compose

This guide will show you how to deploy MariaDB and phpMyAdmin using Docker Compose from this repository.

## Prerequisites
- Docker and Docker Compose must be installed on your system.
- A basic understanding of Docker and Docker Compose is recommended.

## Step 1: Clone the repository
```
git clone https://github.com/racksync/mariadb-pma-docker.git
```

## Step 2: Navigate to the repository directory
```
cd mariadb-pma-docker
```

## Step 3: Edit necessaries variable like port and password.

```
MYSQL_ROOT_PASSWORD: [YOUR_ROOT_PASSWORD]
```

## Step 4: Start the containers
In the same directory where the docker-compose.yml file is located, run the following command:
```
docker-compose up -d
```

## Step 5: Access phpMyAdmin
Once the containers are running, you can access phpMyAdmin by visiting ```http://ip-address:8080``` in your web browser. You should see the phpMyAdmin login page. Use the username root and password password to log in.


## Step 6: Adjust the containers
Once you have verified that the containers are running, you can adjust the containers to your needs. For example, you can change the port that phpMyAdmin is exposed on by editing the docker-compose.yml file. then execute the following command:
```docker-compose up -d --no-deps --build [container-name]```

## Step 7: Stop and remove the containers
```docker-compose down```