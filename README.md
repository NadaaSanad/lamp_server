# Website Setup Documentation

This project outlines the steps taken to set up a PHP-based website with Apache on a Linux server, making it publicly accessible via HTTPS.

## Steps

### 1. Set up the LAMP Stack
- Installed and configured **Apache** as the web server.
- Installed **MySQL** for database management.
- Installed **PHP** and set up the necessary configurations.

### 2. Configure Apache
- Edited the Apache configuration to serve the website on  port 443 (HTTPS).
- Installed SSL and created a self-signed certificate for HTTPS.

### 3. Set Up Port Forwarding
- Configured router port forwarding to allow external access on ports 80 and 443.

### 4. Set Up Dynamic DNS
- Used a Dynamic DNS service to handle IP address changes and provide a domain name for the server.

### 5. Test the Website
- Verified that the website is accessible externally via HTTP and HTTPS.

### 6. Git & GitHub Integration
- Initialized a Git repository, created a `.gitignore` file, and committed the source code and documentation.
- Pushed the project to GitHub for version control.

## Installation Steps for Local Setup

To set up this project locally, clone this repository and follow the instructions in the `README.md` file.
 ####################################
## 1. IP Address: What It Is and Its Purpose in Networking

An **IP address** (Internet Protocol address) is a unique identifier assigned to every device connected to a network. It serves as an address for communication between devices on the network, enabling the devices to find and communicate with each other over the internet or local network.

There are two main types of IP addresses:
- **IPv4**: A 32-bit address written as four decimal numbers separated by dots (e.g., 192.168.1.1).
- **IPv6**: A 128-bit address written in hexadecimal notation, designed to address the limitations of IPv4 (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

In networking, an IP address is essential for:
- Routing packets of data across networks.
- Identifying devices within a network.
- Enabling services like web hosting, email, and file sharing.

## 2. MAC Address: What It Is, Its Purpose, and How It Differs from an IP Address

A **MAC address** (Media Access Control address) is a hardware address that uniquely identifies network interfaces (NICs) at the data link layer of the OSI model. It is embedded in the hardware (usually in the device’s network card) and is used for communication within the local network.

- **Purpose**: A MAC address ensures that data packets are sent to the correct hardware device on a local network.
- **Format**: It is a 48-bit address usually written in hexadecimal, divided into six groups (e.g., 00:1A:2B:3C:4D:5E).

### Key Differences Between MAC and IP Addresses:
- **MAC Address**:
  - Unique to the hardware.
  - Used for local network communication.
  - Static and not typically changed.
- **IP Address**:
  - Used for routing packets across networks.
  - Can change based on network configuration.
  - Dynamic and often assigned by a DHCP server.

## 3. Switches, Routers, and Routing Protocols: Basic Definitions and Their Roles in a Network

### Switches:
A **switch** is a networking device that connects devices within the same local area network (LAN). It receives incoming data packets and forwards them to the destination device within the same network using MAC addresses.

- **Role**: Operates at the data link layer and is responsible for forwarding data to the correct device in a LAN.

### Routers:
A **router** is a networking device that connects different networks, such as a local network to the internet. Routers forward data packets between networks based on their IP addresses.

- **Role**: Operates at the network layer and is responsible for determining the best path for data to travel across networks and to different destinations.

### Routing Protocols:
Routing protocols are algorithms used by routers to determine the best path for data to travel across networks. Some commonly used routing protocols include:
- **RIP** (Routing Information Protocol): A distance-vector routing protocol used in small networks.
- **OSPF** (Open Shortest Path First): A link-state protocol used in larger, more complex networks.
- **BGP** (Border Gateway Protocol): Used for routing between different autonomous systems (like between ISPs).

## 4. Remote Connection to Cloud Instance: Steps to Connect to a Cloud-Based Linux Instance from a Remote Machine (Using SSH)

To connect to a cloud-based Linux instance from a remote machine using **SSH** (Secure Shell), follow these steps:

### Prerequisites:
- A **cloud instance** (e.g., AWS EC2, Google Cloud Compute Engine) with SSH access enabled.
- The **private key** file (e.g., `my-key.pem`) for authentication.
- The **public IP address** of the cloud instance.

### Steps:
1. **Open a Terminal on your local machine**:
   - On Linux/macOS, use the built-in terminal.
   - On Windows, use tools like **Git Bash** or **PuTTY**.

2. **Set the correct permissions for the private key file**:
   Ensure the private key has restricted permissions:
   ```bash
   chmod 400 /path/to/my-key.pem

