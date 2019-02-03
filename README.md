# ZolexNode
- Thank you for owning a ZolexCoin Masternode!  Below are the simple instructions to get up and running with your node.

# Step 1 - Generating TX and Getting Information
- Create a new address in your wallet
- Send exactly 1,000 Zolex to this address
- Now go to the debug console via the Tools menu and type ```masternode outputs```
- After your tx has confirmed on the network, you will see output here, please save this information
- Now type ```masternode genkey``` and save this, it is your private key for Step 2
- Continue to the next step

# Step 2 - Installing the linux wallet and node
- Install a 64 bit Ubuntu 16.04 server from your preferred hosting provider and launch the VPS
- Enter the following line to get started

```apt-get update -y && apt-get upgrade -y && git clone https://github.com/ZolexEcosystem/ZolexNode.git && cd ZolexNode && bash zlx-mn.sh```
- Answer 'y' to the prompts if this is a fresh VPS and you would like to install the wallet
- The script will now ask for your private key saved from step 1, please enter it when prompted and hit enter
- When the script is finished, it will provide you with your masternode IP and private key for the next step

# Step 3 - Configuring the Masternode.config file
- Go to your wallet Tools -> Open Masternode Configuration File
- You'll see an example here, follow it closely
- Enter your masternode name, followed by ip address and port from step 2, followed by your private key from step 1, and finally your tx id and index id from step 1
- An example would like look this:

```mn1 127.0.0.1:33342 93HaPRIVKEYQZE1Yc1K6437tGBDQL8Xg 2bcd3c84TXIDe56834ce18718810b9324456a67c 0```

```name IP:PORT PRIVATE_KEY TX_ID TX_INDEX```

# Step 4 - Starting your Masternode
- Visit your transactions page in your wallet
- Once your transaction that you sent yourself for exactly 1,000 Zolex has 16 confirmations, you may start your node
- You can do this via the masternodes tab

# Congatulations and thank you for your support!  Please make sure you're part of our Discord for future updates and news.
