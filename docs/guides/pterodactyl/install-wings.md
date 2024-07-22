---
title: "How to Install Pterodactyl Wings: A Step-by-Step Guide"
subtitle: "Wings is the next generation server control plane from Pterodactyl."
description: "Pterodactyl is a free, open-source game server management panel built with PHP, React, and Go. Designed with security in mind, Pterodactyl runs all game servers in isolated Docker containers while exposing a beautiful and intuitive UI to end users. "
icon: simple/pterodactyl
status: new
---

<figure markdown>
  ![Image title](https://shardbyte.com/assets/images/guides/pterodactyl/pterodactyl-image-001.png){ width="580" }
  <figcaption>Pterodactyl</figcaption>
</figure>

# **Pterodactyl Wings**
Pterodactyl Wings is a key component of the Pterodactyl game server management panel. It is the daemon that runs on the server nodes, handling the creation, management, and monitoring of game server instances. Wings uses Docker containers to provide an isolated and secure environment for each game server, ensuring stability and security. By managing resources efficiently and allowing seamless communication with the Pterodactyl panel, Wings makes it easy to deploy and operate multiple game servers on a single physical or virtual server.

### **Prerequisites**

Ensure you have the following before starting the setup process:

- Pterodactyl Panel installed and configured.
- Access to the Pterodactyl admin panel.
- Root or sudo access to the server. (ideally root)
- Basic knowledge of command line operations.

### **Step 1: Creating a Location in Pterodactyl**

## Step 1: Login to Pterodactyl Admin Panel:
1. Open your Pterodactyl Panel in a web browser.
2. Log in with your admin credentials.

## Step 2: Navigate to Locations:
1. In the sidebar, go to **Admin Panel**.
2. Click on **Locations**.

## Step 3: Create a New Location:
1. Click the **Create New** button.
2. **Name:** Enter a name for the location (e.g., "North America").
3. **Short Code:** Enter a short code (e.g., "NA").
4. Click **Create Location** to save.

Your location is now created and can be assigned to nodes for better organization and resource management.

### **Step 2: Create a Node in Pterodactyl Panel**

1. **Login to Pterodactyl Admin Panel:**
    - Open your Pterodactyl Panel in a web browser and log in as an admin.

2. **Navigate to Nodes:**
    - Go to **Admin Panel** > **Nodes** > **Create New**.

3. **Fill in Node Details:**
    - **Name:** Enter a name for your node.
    - **Location:** Select a location.
    - **FQDN:** Enter the domain name or IP address of your node.
    - **Scheme:** Choose `http` or `https` based on your setup.
    - **Daemon Port:** Set to `8080` or your preferred port.
    - **Memory & Disk:** Allocate resources based on your server capacity.
    - **Public:** Enable if you want the node to be publicly accessible.

4. **Save Node:**
    - Click **Create Node** to save your settings.

5. **View Node Configuration:**
    - After saving, you will see a configuration command under **Configuration**.
    - Click **Generate Token** to make the command that will be used to configure Wings.

### **Step 3: Start Wings on Your Node**

1. **Connect to Your Node:**
    - SSH into your server where Wings will be installed.

2. **Install Wings:**
   - Execute the previously generated command to install and configure Wings (The command copied from the Panel).

3. **Start Wings:**

Start Wings using the following command:
``` { .bash .copy }
systemctl start wings
```

### **Step 4: Verify Node Status**

1. Check Node Status:
    - Go back to the Pterodactyl Panel.
    - Navigate to **Admin Panel** > **Nodes**.
    - Your new Node should show as :material-heart-pulse:{ .heart-pulse } **Active** if Wings started successfully.

Congratulations! You've successfully configured and started your Node for Pterodactyl Panel. If you encounter any issues or want to explore additional configuration options, refer to the [Pterodactyl Documentation](https://pterodactyl.io/wings/1.0/installing.html).
