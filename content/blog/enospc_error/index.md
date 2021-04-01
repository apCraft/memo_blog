---
title: ENOSPCエラー
date: "2021-04-01T18:32:03.284Z"
---

ENOSPCエラーが出る場合の対応
内部でwatchを使っているようでファイル数が多くなるとエラーになる

> echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
