# npmでn8nをインストールしてセルフホストする

https://docs.n8n.io/hosting/installation/npm/

## Try n8n with npx

`npx` を使用することですぐにローカルホストを立ち上げられるみたい。

```bash
npx n8n
```

[ローカルホスト](http://localhost:5678) へアクセスできる。

## Install globally with npm

n8nをグローバルにインストールする。

```bash
npm install -g n8n@1.118.1
```

バージョンを指定してインストールする。
バージョンは [こちら](https://docs.n8n.io/release-notes/) から確認する。

ローカルにインストールして試してみる。

```bash
mkdir sample-project
cd sample-project
npm init -y
npm install n8n@1.118.1
./node_modules/.bin/n8n
```

これで [ローカルホスト](http://localhost:5678) にアクセスできる。

## ユースケース

EC2インスタンス上でインストールしてApacheやNginxでホスティングを行う。カスタムノードを用いた詳細な制御をしたい場合に有効である。
