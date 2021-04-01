---
title: ENOSPCエラー
date: "2021-04-01T18:32:03.284Z"
---

ENOSPCエラーが出る場合の対応
内部でwatchを使っているようでファイル数が多くなるとエラーになる

```
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```
ant designやmaterial uiを導入した場合は設定が必須なよう。

[](
https://zukucode.com/2018/01/linux-watch.html
)
