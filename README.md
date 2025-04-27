<p align="center">
  <img src="https://raw.githubusercontent.com/Shuvopme/your-repo-name/main/banner.png" alt="Gensyn Node Run - Customed By Shuvo" width="100%" /> />
</p>

<h1 align="center">🚀 Gensyn Node Run - Customed By Shuvo</h1>

<p align="center">
  <strong>Easy installation for MacOS, Windows (WSL), Linux, and VPS Users!</strong>
</p>

<p align="center">
  <a href="https://t.me/gensyntrackbot">
    <img src="https://img.shields.io/badge/Telegram-Bot-blue?style=for-the-badge&logo=telegram" alt="Telegram Bot" />
  </a>
  <a href="https://gensyn-testnet.explorer.alchemy.com">
    <img src="https://img.shields.io/badge/Explorer-View-green?style=for-the-badge&logo=graphql" alt="Explorer" />
  </a>
  <a href="https://dashboard.gensyn.ai/">
    <img src="https://img.shields.io/badge/Dashboard-Visit-orange?style=for-the-badge&logo=data" alt="Dashboard" />
  </a>
</p>

---

## ✅ System Requirements

- Minimum **16GB RAM** (Swap enabled if RAM < 16GB)
- Recommended GPU: **RTX 3090/4090** (Optional for higher performance)
- Platforms Supported: **MacOS, Windows (WSL2), Linux Ubuntu/Debian VPS**

---

## ⚡ Quick Start Installation

### 1. Setup Swap Memory (Recommended)

```bash
sudo swapoff -a && sudo rm -f /swapfile
sudo fallocate -l 8G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile
swapon --show && free -h
echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab

2. Update Packages and Install Dependencies

sudo apt update && sudo apt upgrade -y
sudo apt install curl wget git build-essential python3 python3-venv python3-pip screen lsof -y

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update && sudo apt install yarn -y


MacOS Users:
Install Homebrew fiscreen

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install python3 git screen

3. Download and Install Node Script

curl -sSL https://raw.githubusercontent.com/Shuvopme/Gensyn-Node-Run/main/node.sh | bash

🛠️ Running the Node

screen -S gensyn

cd $HOME
rm -rf gensyn-testnet
git clone https://github.com/zunxbt/gensyn-testnet.git
chmod +x gensyn-testnet/gensyn.sh
./gensyn-testnet/gensyn.sh

Detach screen: Ctrl + A, then D
Reconnect screen: screen -r gensyn

🔥 Backup Your Node

curl -sSL -O https://raw.githubusercontent.com/Shuvopme/your-repo-name/main/backup.sh
chmod +x backup.sh
./backup.sh

📚 Useful Links
Gensyn Tracker Bot

Testnet Explorer

Gensyn Dashboard

<p align="center"> 🚀 Powered by <strong>Shuvo</strong> | Let's Decentralize the Future! </p> ```
