---
title: 個人用linuxbrewとnodeのインストール
date: "2021-04-01T18:32:03.284Z"
---

個人用linuxbrewとnodeのインストール

```
sudo apt install -y vim curl git ruby   zlib1g-dev libssl-dev libbz2-dev libsqlite3-dev libffi-dev liblzma-dev     software-properties-common apt-transport-https ca-certificates
sh -c "$(curl -fsSL https://raw.githubusercontent.com/Linuxbrew/install/master/install.sh)"
echo 'export PATH="/home/linuxbrew/.linuxbrew/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
brew install curl git wget gcc zlib libzip bzip2 readline openssl pkg-config autoconf
brew install anyenv
anyenv install --init
echo 'eval "$(anyenv init -)"' >> ~/.bashrc
source ~/.bashrc
mkdir -p $(anyenv root)/plugin
git clone https://github.com/znz/anyenv-update.git $(anyenv root)/plugins/anyenv-update7
ls
anyenv update
anyenv -v
anyenv install nodenv
exec $SHELL -l
mkdir -p "$(nodenv root)/plugins"
git clone https://github.com/pine/nodenv-yarn-install.git "$(nodenv root)/plugins/nodenv-yarn-install"
echo 'export PATH="$HOME/.yarn/bin:$PATH"' >> ~/.bashrc
touch $(nodenv root)/default-packages
nodenv install --list
nodenv install 14.15.4
nodenv global 14.15.4
nodenv versions
exec $SHELL -l
node -v
yarn -v
yarn global add gulp

```