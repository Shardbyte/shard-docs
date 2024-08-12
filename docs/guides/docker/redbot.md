---
title: "Ultimate Guide: Setting Up Red Discord Bot with Docker for Seamless Server Management"
subtitle: "Unlock the Power of Red Discord Bot Using Docker - A Step-by-Step Tutorial for Effortless Deployment and Customization"
description: "Discover the simplicity of deploying the Red Discord Bot using Docker! This comprehensive guide walks you through creating a Discord bot, inviting it to your server, and leveraging Docker or Docker Compose for a streamlined setup. Optimize your server management with Red's powerful features hassle-free."
icon: simple/docker
status: new
---

# **RedBot**

Using Red Discord Bot with Docker offers several advantages. Docker provides a lightweight, portable, and consistent environment for deploying applications, making it easier to manage dependencies and ensure a smooth setup process. With Docker, you can encapsulate the Redbot and its dependencies in a container, reducing potential conflicts and making deployment across different environments seamless. This approach simplifies installation, enhances scalability, and facilitates efficient resource utilization. Whether you're a novice or an experienced user, leveraging Docker for Redbot ensures a reliable and hassle-free experience, allowing you to focus more on exploring and customizing the bot's extensive features.

### **Step 1: Download Prerequisites**

Ensure you have the following before starting the setup process:

- A Discord account
- Sufficient permissions to add a bot to a server
- Docker installed on your system of choice

### **Step 2: Create the Discord Bot**

1. Go to the [Discord Developer Portal](https://discord.com/developers/applications).
2. Click on "New Application" and give your bot a name.
3. Navigate to the "Bot" tab and click "Add Bot."
4. Note down the token generated for your bot. (You will need it later)

### **Step 3: Invite the Bot to Your Server**

1. On the [Discord Developer Portal](https://discord.com/developers/applications), go to the "OAuth2" tab.
2. In the "OAuth2 URL Generator" section, select the "bot" scope.
3. Scroll down and choose the necessary permissions for your bot.
4. Copy the generated URL and paste it into your browser. Follow the prompts to add the bot to your server.

### **Step 4: Create a Docker Compose File**

Create a `docker-compose.yml` file in your preferred text editor with the following content:
``` { .yaml .copy }
# Docker Compose | compose-redbot.yml
#
#
services:
#######################################################
  discord_redbot:
    image: 'shardbyte/bot-red:latest'
    container_name: discord_redbot
    restart: unless-stopped
    environment:
      TOKEN: 'YOUR_BOT_TOKEN'
      TZ: 'Etc/UTC'
      PREFIX: '/'
      PUID: '1000'
      GUID: '1000'
      EXTRA_ARGS: '--no-cogs'
    volumes:
      - '/your/persistent/data/location:/data'
    networks:
      - your_network
#######################################################
networks:
  your_network:
    name: your_network
#######################################################
```
!!! note
    Replace `YOUR_BOT_TOKEN` with the actual token you obtained from the [Discord Developer Portal](https://discord.com/developers/applications).

### **Step 5: Run Red Bot using Docker Compose**

Open a terminal or command prompt and run the following command:
``` { bash .copy }
docker-compose up -d
```
!!! note
    This command starts Red bot in detached mode.

### **Step 6: Verify the Bot is Running**

Check the logs to ensure that Red bot is running without issues:
``` { bash .copy }
docker logs --follow discord-redbot
```

Look for initialization messages and any potential errors in the logs.

### **Step 7: Customize and Explore**

Join your Discord server and test the bot's functionality. You can customize the bot's settings using Red's commands and explore its features.

Congratulations! You've successfully set up the Red Discord bot using Docker Compose. If you encounter any issues or want to explore additional configuration options, refer to the [Red documentation](https://docs.discord.red/en/stable/).
