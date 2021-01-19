# c9-on-ubuntu
These are set of commands to install/host c9 on ubuntu




`
sudo apt-get install git -y
sudo apt-get update
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt install nodejs
node --version
npm --version
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
nvm --version
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
nvm --version
sudo apt install build-essential
git clone https://github.com/c9/core.git c9sdk
cd c9sdk
sudo apt install python2
python --version
sudo apt install python
python --version
scripts/install-sdk.sh
cd ~
npm install pm2 -g
pm2 --version
pm2 start c9sdk/server.js --name "c9" -- --auth username:password --port 8000 -w ~ --collab true
pm2 logs c9
clear
`
