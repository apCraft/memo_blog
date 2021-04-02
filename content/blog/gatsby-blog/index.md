---
title: gatsbyテンプレでブログの導入
date: "2021-04-02T00:32:03"
---

gatsbyテンプレでブログの導入

```
npm install -g gatsby-cli
gatsby -v

gatsby new gatsby-starter-blog-amp-to-pwa https://github.com/tomoyukikashiro/gatsby-starter-blog-amp-to-pwa
cd gatsby-starter-blog-amp-to-pwa

# 確認
gatsby develop

# build＆確認
yarn run build && yarn run serve
```