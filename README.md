# vagrant-nodejs
Nodejs vagrant setup


## Update package list, then install node and npm
sudo apt-get update && sudo apt-get install nodejs npm

# Download nvm install.sh and run with bash
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash

# reload .bashrc so nvm command works
source ~/.bashrc

# Explicitly install supported node version
nvm install 10.16

# Install Stencil CLI
npm install -g @bigcommerce/stencil-cli

# move into theme dir
cd ~/path/to/theme/dir

# initialize a new .stencil config for the theme
stencil init

# install theme modules
npm install

# serve a live, Browsersync enabled preview of the theme
stencil start
