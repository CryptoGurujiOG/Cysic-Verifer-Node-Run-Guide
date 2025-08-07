# Cysic-Verifer-Node-Run-Guide
In this guide, I will walk you through step-by-step instructions to set up and run a Cysic verifier node on Windows (via WSL), macOS, and VPS, making the process easy and efficient.

![image alt](https://github.com/CryptoGurujiOG/Cysic-Verifer-Node-Run-Guide/blob/48e8cc98a3708c2752dfe8ce998b9e2b8d63820c/Screenshot%205.jpeg)

## Verifier Node Requirements:

- Minimum 8 GB Ram
- Minimum 2 Core CPU
- 100 GB Storage
- PC or VPS with WSL, Ubuntu, or MacOS
- New Metamask and Keplr wallet

---

Before we start:
Create a new MetaMask wallet, then import the same wallet into Keplr wallet using the same seed phrase.

- Metamask wallet: [Link](https://metamask.io/download)
- Keplr wallet: [Link](https://www.keplr.app/get)

---

- If you want to run verifier node on your pc/laptop, then install WSL using this 👉 [Guide](https://github.com/CryptoGurujiOG/Install-Ubuntu-on-Windows-using-WSL)
- If you want to run verifier node on a VPS then watch my video guide 👉 [video](https://youtu.be/NK431xjj7yA)

---

# Step 1:

- Visit: https://app.cysic.xyz/
- Click Sign in
- Click Connect Wallet
- Connect your EVM wallet (Metamask)
- Click Bind Invite Code (top right)
- Enter Invite code 👉 2c609
- Verify Invite Code
- Choose a Name and Submit 
- Click on your wallet address (top right)
- Connect your Keplr wallet
- Click Social Tasks and complete all tasks
- Click on the Faucet icon
- Claim 0.1 testnet $CYS daily for 7 days
- You will need minimum 0.7 testnet $CYS to run a verifier node
  
# Step 2:

## Update system and install dependencies:

- Linux (WSL, Ubuntu, or VPS)

```
sudo apt update && sudo apt upgrade -y && sudo apt install -y screen wget
```
- MacOS
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" && brew update && brew install screen wget
```

## Install and Run Verifier Node:

- Create a screen session:

```
screen -S cysic
```

- Linux (WSL, Ubuntu, or VPS)
- Replace ```0x-Fill-in-your-reward-address-here``` with your actual with your actual Metamask ```EVM address```

```
curl -L https://github.com/cysic-labs/cysic-phase3/releases/download/v1.0.0/setup_linux.sh > ~/setup_linux.sh && bash ~/setup_linux.sh 0x-Fill-in-your-reward-address-here

cd ~/cysic-verifier/ && bash start.sh
```
- MacOS
- Replace ```0x-Fill-in-your-reward-address-here``` with your actual with your actual Metamask ```EVM address```

```
curl -L https://github.com/cysic-labs/cysic-phase3/releases/download/v1.0.0/setup_mac.sh && bash ~/setup_mac.sh 0x-Fill-in-your-reward-address-here

cd ~/cysic-verifier/ && bash start.sh
```

- After running the command above, wait a few minutes, you will see a new ```your current worker address```

![image alt](https://github.com/CryptoGurujiOG/Cysic-Verifer-Node-Run-Guide/blob/52b99bfa45e136bd6e3a76124c3da129a5844c7d/Screenshot%201.png)

- Now you can exit the Screen to keep verifier node running in the background
- Press ```Ctrl+A+D``` to exit the Screen

# Step 3:

- Visit: https://app.cysic.xyz/verifier
- Click on the Reserve 
- Select the ```your current worker address``` in the Worker Address Section
- Enter 0.51 amount and Reserve

![image alt](https://github.com/CryptoGurujiOG/Cysic-Verifer-Node-Run-Guide/blob/5eecdfd24a04d78295f027405d50efb0a93e9adc/Screenshot%204.png)

- After a few minutes, you will see ```Standard ACTIVE``` under ZK Verifier Status

![image alt](https://github.com/CryptoGurujiOG/Cysic-Verifer-Node-Run-Guide/blob/1afad7a0faac3d3bad88dc5d90fa343a008cb3b3/Screenshot%202.png)

- Visit: https://app.cysic.xyz/dashboard/verifier
- Enter your main EVM wallet address from Metamask to check Node status and Distributed Rewards

![image alt](https://github.com/CryptoGurujiOG/Cysic-Verifer-Node-Run-Guide/blob/44d08c654fe1a19158530ef4432f426f57e02358/Screenshot%203.png)

✅ Now you are all set

### I will soon share a step-by-step video guide on my YouTube channel.

- Twitter: https://x.com/CryptoGurujiOG
- Youtube: https://www.youtube.com/@CryptoGurujiOG
- Telegram: https://www.telegram.me/cryptogurujiog

