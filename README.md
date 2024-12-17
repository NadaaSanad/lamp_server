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
