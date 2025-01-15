# 🐳 Deploy MariaDB and PhpMyAdmin with Docker Compose

This guide will show you how to deploy MariaDB and phpMyAdmin using Docker Compose from this repository.

## 📋 Prerequisites
- Docker and Docker Compose must be installed on your system.
- A basic understanding of Docker and Docker Compose is recommended.

## 1️⃣ Step 1: Clone the repository
```
git clone https://github.com/racksync/mariadb-pma-docker.git
```

## 2️⃣ Step 2: Navigate to the repository directory
```
cd mariadb-pma-docker
```

## 3️⃣ Step 3: Configure Environment Variables
Copy the example .env file and modify it according to your needs:
```bash
cp default.env .env
```
Edit the .env file to set your desired:
- Database credentials
- WordPress configuration
- Timezone
- Ports for MariaDB, phpMyAdmin, and WordPress
- phpMyAdmin settings

After configuration, you can access:
- WordPress at http://ip-address:8000
- phpMyAdmin at http://ip-address:8080

## 4️⃣ Step 4: Start the containers 🚀
In the same directory where the docker-compose.yml file is located, run the following command:
```
docker-compose up -d
```

## 5️⃣ Step 5: Access phpMyAdmin 🌐
Once the containers are running, you can access phpMyAdmin by visiting ```http://ip-address:8080``` in your web browser. You should see the phpMyAdmin login page. Use the username root and password password to log in.

## 6️⃣ Step 6: Adjust the containers ⚙️
Once you have verified that the containers are running, you can adjust the containers to your needs. For example, you can change the port that phpMyAdmin is exposed on by editing the docker-compose.yml file. then execute the following command:
```docker-compose up -d --no-deps --build [container-name]```

## 7️⃣ Step 7: Stop and remove the containers 🛑
```docker-compose down```

### 📚 Automation Training

- 🛒 [สินค้าและบริการ](http://racksync.com)
- 📖 [เทรนนิ่งคอร์ส](https://facebook.com/racksync)

### 👥 Community

- 🏘️ [Home Automation Thailand](https://www.facebook.com/groups/hathailand)
- 🛍️ [Home Automation Marketplace](https://www.facebook.com/groups/hatmarketplace)
- 💬 [Home Automation Thailand Discord](https://discord.gg/Wc5CwnWkp4) 

## 🏢 [RACKSYNC CO., LTD.](https://racksync.com)

RACKSYNC Co., Ltd. specializes in automation and smart solutions of all scales. We are experts in designing, implementing, and monitoring sophisticated automation systems. Our team of specialists provides comprehensive consulting services and technical implementation for both residential and commercial projects. Beyond automation, we offer full-cycle Software as a Service (SaaS) development, helping businesses transform their operations through custom digital solutions. With our deep expertise in IoT, home automation, and enterprise systems, we deliver reliable and innovative solutions tailored to each client's unique requirements.

📍 RACKSYNC COMPANY LIMITED 🌏 Suratthani, Thailand 84000 
🌐 Website : [racksync.com](https://racksync.com) 
📧 Email : devops@racksync.com 
📞 Tel : +66 85 880 8885 

[![Home Automation Thailand Discord](https://img.shields.io/discord/986181205504438345?style=for-the-badge)](https://discord.gg/Wc5CwnWkp4) [![Github](https://img.shields.io/github/followers/racksync?style=for-the-badge)](https://github.com/racksync) 
[![WebsiteStatus](https://img.shields.io/website?down_color=grey&down_message=Offline&style=for-the-badge&up_color=green&up_message=Online&url=https%3A%2F%2Fracksync.com)](https://racksync.com)



