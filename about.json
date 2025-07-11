# WSL-Setup-Guide
WSL setup for beginners in Windows
Here’s a concise guide for setting up WSL (Windows Subsystem for Linux) and organizing a GitHub repository for it:

---

# **WSL Setup Guide**

## 1. **Prerequisites**
- Ensure your Windows version supports WSL: Windows 10 (Build 19041 or higher) or Windows 11.
- Administrative access to enable features and install software.

## 2. **Enable WSL**
1. Open PowerShell as Administrator.
2. Run:
   ```powershell
   wsl --install
   ```
3. Restart your computer if prompted.

## 3. **Install a Linux Distribution**
1. After restarting, select and install a Linux distribution (e.g., Ubuntu, Debian).
2. Alternatively, run:
   ```powershell
   wsl --install -d <distro-name>
   ```
3. Launch the installed distribution from the Start menu.

## 4. **Update and Upgrade**
Inside the Linux terminal, update and upgrade packages:
```bash
sudo apt update && sudo apt upgrade -y
```

## 5. **Set Up Git**
1. Install Git:
   ```bash
   sudo apt install git -y
   ```
2. Configure Git:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```

## 6. **Connect WSL to GitHub**
1. Generate SSH keys:
   ```bash
   ssh-keygen -t ed25519 -C "your.email@example.com"
   ```
   Follow the prompts to save the key.
2. Add the SSH key to the GitHub account:
   - Copy the key:
     ```bash
     cat ~/.ssh/id_ed25519.pub
     ```
   - Paste it into GitHub > Settings > SSH and GPG keys > New SSH Key.
3. Test the connection:
   ```bash
   ssh -T git@github.com
   ```

## 7. **Install Essential Tools**
```bash
sudo apt install build-essential curl wget -y
```

## 8. **Optional: Install Docker**
1. Install Docker:
   ```bash
   sudo apt install docker.io -y
   ```
2. Add your user to the Docker group:
   ```bash
   sudo usermod -aG docker $USER
   ```
3. Restart WSL or your system for changes to take effect.

---

# **Repository Structure**

### **Repository Name**: `wsl-setup-guide`

### **Folder Structure**:
```
wsl-setup-guide/
│
├── README.md
├── setup/
│   ├── install-wsl.md
│   ├── install-git.md
│   ├── connect-github.md
│   ├── essential-tools.md
│   └── docker-setup.md
├── scripts/
│   ├── wsl-setup.sh
│   ├── git-setup.sh
│   └── docker-setup.sh
└── images/
    ├── wsl-setup.png
    ├── git-config.png
    └── github-ssh-key.png
```

### **File Descriptions**
1. `README.md`: Overview of the repository with setup instructions.
2. `setup/`: Markdown files with detailed setup steps.
3. `scripts/`: Bash scripts for automating the setup process.
4. `images/`: Screenshots and visual guides.

### **README.md Template**
```markdown
# WSL Setup Guide

This repository provides a comprehensive guide to setting up Windows Subsystem for Linux (WSL) on your Windows machine, along with tools like Git and Docker.

## Features
- Step-by-step instructions for WSL installation.
- Git configuration and GitHub connection.
- Essential tools setup.
- Optional Docker installation.

## Repository Structure
- **setup/**: Detailed guides for each step.
- **scripts/**: Automated scripts for setup.
- **images/**: Visual aids.

## Quick Start
1. Clone the repository:
   ```bash
   git clone git@github.com:<your-username>/wsl-setup-guide.git
   ```
2. Navigate to the repository:
   ```bash
   cd wsl-setup-guide
   ```
3. Run the setup script:
   ```bash
   bash scripts/wsl-setup.sh
   ```
