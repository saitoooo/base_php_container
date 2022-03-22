# Base PHP Container

私的開発用に作成したDockerCompose一式です。

[MyLocal Nginx Proxy](https://github.com/saitoooo/mylocal-nginx-proxy) を利用することを前提にしています。
プロジェクト一式を配置してVSCode開いた後「Reopen Open Container」である程度必要な拡張を含めインストールされると思います。

* PHP Debug
* PHP Intelephense
* phpcs
* php cs fixer

## ホスト名とDBの設定

設定の一部は ** postgresql.env ** と ** web.env ** で設定しています。
ホスト名はnginx proxyとの連携する要素でもあるので注意してください。

## 使い方

1. あらかじめ /etc/hosts 等 .local で終わるホスト名を設定します。
1. そのソフト名をweb.envに設定します
1. MyLocal Nginx Proxyを起動しておきます。
1. このドキュメントのあるフォルダをVSCodeで開いてReopenContainerをする
1. ブラウザで https://[設定したホスト名] でアクセスする
1. phpinfoが表示されます。
1. 煮るなり焼くなり好きにしてください

