---
title: ブログのカスタマイズ
date: 2019-08-16 22:41:15
tags:
---
# テーマの変更
staticgen.comからNetlifyヘデプロイした際のテーマ"landscape"から"light"というテーマに変更しました。
テーマのファイルはサブモジュールとして定義されていました。

```
  git submodule deinit -f themes/landscape
  git submodule add https://github.com/hexojs/hexo-theme-light themes/light
```

テーマの変更後、最初に出ていたエラーメッセージが出なくなりました。

# 最適化
hexo-all-minifierというプラグインを導入しました。
書いてあるとおりにnpmでインストールし、```_config.yml```に```all_minifier: true```を記載しました。
