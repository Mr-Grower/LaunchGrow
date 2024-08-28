# LaunchGrow

# Steps
1. Open WSL from Windows or open your terminal linux (ubuntu)
2. Download daemon
   ```
   sudo apt -y update && sudo apt -y install wget unzip
   wget https://github.com/Mr-Grower/GROW/releases/download/1.0/GROW-Linux.zip
   unzip GROW-Linux.zip
   sudo mv growerd grower-tx grower-cli grower-qt /usr/bin

3. Create grower.conf, copy variables and save file
   ```
   mkdir $HOME/.grower
   nano ~/.grower/grower.conf

   rpcuser=rpc_grower
   rpcpassword=yourpassword
   rpcallowlist=127.0.0.1
   listen=1
   server=1
   txindex=1
   daemon=1
   reindex=1
   staking=1
   addnode=213.199.42.151

4. Finally, start daemon
  ```
  growerd
