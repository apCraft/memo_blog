---
title: 個人用ubuntu設定
date: "2021-03-30T18:32:03.284Z"
---

個人用ubuntuの開発環境設定

```
sudo apt update && sudo apt upgrade
sudo update-locale LANG=ja_JP.UTF-8
sudo ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime

sudo apt -y install software-properties-common
sudo apt install neovim -y
sudo update-alternatives --set editor $(which nvim)
sudo apt install unzip wget curl git zsh snapd -y
sudo apt purge -y vim-tiny


#日本語関係とfont追加
sudo apt install 'fonts-takao-*' -y
sudo apt install fonts-ipafont fonts-ipaexfont fonts-vlgothic -y
sudo apt install -y fonts-migmix fonts-ipamj-mincho fonts-horai-umefont fonts-takao xfonts-mona fonts-kouzan-mouhitsu fonts-konatsu
sudo apt install -y fonts-roboto fonts-noto fonts-ricty-diminished
sudo apt install -y language-pack-ja language-pack-gnome-ja fonts-takao-gothic fonts-takao-mincho fonts-takao-pgothic fonts-vlgothic fonts-ipafont-gothic fonts-ipafont-mincho libreoffice-l10n-ja libreoffice-help-ja firefox-locale-ja manpages-ja thunderbird-locale-ja ibus-mozc ibus-anthy kasumi ibus-gtk ibus-gtk3 poppler-data cmap-adobe-japan1 fcitx-mozc fcitx-anthy fcitx-frontend-qt5 fcitx-config-gtk fcitx-config-gtk2 fcitx-frontend-gtk2 fcitx-frontend-gtk3 mozc-utils-gui fcitx-frontend-qt4 fcitx-frontend-qt5 libfcitx-qt0 libfcitx-qt5-1
```