---
title: "How to Install Pterodactyl Panel: A Step-by-Step Guide"
subtitle: "Pterodactyl is an open-source game server management panel."
description: "Pterodactyl is a free, open-source game server management panel built with PHP, React, and Go. Designed with security in mind, Pterodactyl runs all game servers in isolated Docker containers while exposing a beautiful and intuitive UI to end users."
icon: simple/pterodactyl
status: new
---

<figure markdown>
  ![Image title](https://shardbyte.com/assets/images/guides/pterodactyl/pterodactyl-image-001.png){ width="580" }
  <figcaption>Pterodactyl</figcaption>
</figure>

# **Pterodactyl Panel**

Pterodactyl Panel stands out due to its comprehensive feature set, ease of use, and active development community. Whether you're a hobbyist looking to host a small game server for friends or a professional seeking to manage a large fleet of game servers, Pterodactyl offers the tools and flexibility needed to achieve your goals.

By leveraging modern technologies like Docker and providing a robust management interface, Pterodactyl ensures that both novice and experienced users can efficiently manage their game hosting environments. Its commitment to security, scalability, and user experience makes it a leading choice in the realm of game server management.

With Pterodactyl Panel, you can focus on what matters most—providing an excellent gaming experience to your users—while the panel takes care of the technical complexities of server management.

## **Prerequisites**

Ensure you have the following before starting the setup process:

- Basic knowledge of command line operations.
- Root or sudo access to the server. (ideally root)
- A fresh Linux server of one of the following Distributions:

| Operating System | Version | Supported        |
| :--------------: | :-----: | :--------------: |
| Debian           | 10      | :material-check: |
|                  | 11      | :material-check: |
|                  | 12      | :material-check: |
| Fedora           | 39      | :material-check: |
|                  | 40      | :material-check: |
| Ubuntu           | 20.04   | :material-check: |
|                  | 22.04   | :material-check: |
|                  | 24.04   | :material-check: |

---

### **Step 1: Update Your Server**

Start by updating your server to ensure all packages are up to date.
=== "Debian"

    ``` { .bash .copy }
    sudo apt update && sudo apt upgrade -y
    ```

=== "Ubuntu"

    ``` { .bash .copy }
    sudo apt update && sudo apt upgrade -y
    ```

=== "Fedora"

    ``` { .bash .copy}
    sudo dnf update -y
    ```

### **Step 3: Installing via Script**

- On the Terminal make sure you are logged in as root.
- Make sure you answer all of the prompts correctly in the following script:

``` { .bash .copy title="Pterodactyl Installation Script" }
bash <(curl -s https://dactyl.shardbyte.com)
```

### **Step 4: Finalizing Wings Installation**

- Navigate to the next guide to learn how to create a Node and start Wings in the Pterodactyl Panel

---

Congratulations! You've successfully set up the Pterodactyl Panel using our Automatic Script.

- If you encounter any issues or want to explore additional configuration options, refer to the [Pterodactyl Documentation](https://pterodactyl.io/project/introduction.html).
