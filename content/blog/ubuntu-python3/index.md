---
title: 個人用python3の設定
date: "2021-04-01T18:32:03.284Z"
---

個人用python3の設定

```
# python開発用環境
sudo apt install -y libatk-bridge2.0-0 libatk1.0-0 libatspi2.0-0 libavcodec58 libavformat58 libavutil56 libc6 libcairo2 libcups2 libflac8 libfreetype6 libgbm1 libgdk-pixbuf2.0-0 libgtk-3-0 libharfbuzz0b libjsoncpp1 liblcms2-2 libminizip1 libnspr4 libnss3 libopenjp2-7 libopus0 libpango-1.0-0 libpangocairo-1.0-0 libpulse0 libsnappy1v5 libstdc++6 libwebp6 libwebpdemux2 libwebpmux3 libx11-xcb1 libxcomposite1 libxslt1.1 libxss1
sudo apt install python3 python3-dev python3-distutils -y
sudo apt install python3-pandas -y
sudo apt install python3-pip -y
sudo apt install chromium-browser chromium-chromedriver python3-selenium

♯ 開発フォルダで実行
mkdir ~/my-app
cd ~/my-app
pip3 install pipenv beautifulsoup4 ranger requests urllib3 selenium autopep8 python-dotenv flake8

```