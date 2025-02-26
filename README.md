# DVWA Development Container for VS Code

This repository provides a **Visual Studio Code Dev Container** setup for **Damn Vulnerable Web Application (DVWA)** using Docker. This environment allows penetration testers and security enthusiasts to explore and practice web application security in an isolated, controlled setup.

## Features
- **Pre-configured Docker setup** for DVWA
- **Seamless integration with VS Code Dev Containers**
- **MySQL database setup** for DVWA
- **Persistent storage** for database data
- **Port forwarding for easy access** via `http://localhost:8080`

## Prerequisites
Before you start, ensure you have the following installed on your system:
- [Docker](https://www.docker.com/get-started)
- [Visual Studio Code](https://code.visualstudio.com/)
- [VS Code Remote - Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## Setup Instructions
1. **Clone this repository:**
   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```
2. **Open the folder in VS Code.**
3. **Reopen the project inside the Dev Container:**
   - Click on **"Reopen in Container"** when prompted
   - Or open the command palette (`Ctrl+Shift+P`) and select:
     ```
     Remote-Containers: Reopen in Container
     ```
4. **Wait for the container to build and start.**
5. **Access DVWA in your browser:**
   - Open `http://localhost:8080`
   - Use the default credentials:
     - Username: `admin`
     - Password: `password`

## File Overview
- `.devcontainer/devcontainer.json` - Configures the VS Code Dev Container.
- `docker-compose.yml` - Defines the Docker services for DVWA and MySQL.
- `README.md` - This documentation.

## Learning Web Application Security
DVWA is an excellent platform to practice web application security concepts, including:
- SQL Injection
- Cross-Site Scripting (XSS)
- Command Injection
- Security Misconfigurations

**⚠️ Warning:** This environment is intentionally vulnerable. Do not expose it to the internet or use it on production machines.

## Troubleshooting
If you encounter issues:
- Make sure Docker is running
- Restart the Dev Container (`Ctrl+Shift+P` → **Remote-Containers: Rebuild and Reopen in Container**)
- Check container logs: `docker logs dvwa-dev`

Happy Hacking! 🛡️

