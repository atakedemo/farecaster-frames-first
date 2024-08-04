# farecaster-frames-first
FarecasterのFramesを理解するために作成

# 手順
## 0. asdf でのバージョン設定
    mac m2にてasdfでバージョン管理を行なっているため
    ```bash
    asdf local nodejs 20.14.0
    asdf local yarn 1.22.22  
    ```
## 1. セットアップ
1. Yarnの初期化
   ```bash
   yarn init
   ```
2. ライブラリのインストール
   ```bash
   yarn create frog -t vercel

    # PJ名の入力を求められるので、任意の名称を入力する
    ◇  Enter the name of your project
    │  farecaster-frames-tutorial
   ```
3. Frogのガイドラインに則ってビルドまで進められることを確認
   ```bash
   cd ./farecaster-frames-tutorial
   yarn
   yarn dev
   ```

   下記表示が出れば動作問題なし
   ```bash
    ➜  Local:   http://localhost:5173/api
    ➜  Inspect: http://localhost:5173/api/dev
    ➜  Network: use --host to expose
   ```

## 2. Frog Devツールのセットアップ
プロジェクトのルートディレクトリ([./](./))で実施
1. Frogの初期設定を行い、サーバーを起動
※上記「1.セットアップ」とは別ウィンドウのターミナルを実行する
 ```bash
 yarn global add frog
 npx frog
 ```
2. [http://localhost:5174/](http://localhost:5174/)へアクセスする
3. 入力フォームで作成したプロジェクトのエンドポイント（「1.セットアップ」の段階では、[http://localhost:5174/api](http://localhost:5174/api)）
   [Frog Devツール_01](./assets/01_frog_start.png)
4. 開発画面が表示されるので、その場でボタン押下などのインタラクションをテストする
   [Frog Devツール_01](./assets/02_frog_devtool.png)
   
## 3. 

# 参考
* [Farecaster Docs - Getting Started](https://docs.farcaster.xyz/developers/frames/getting-started)
* [frog - Devtools](https://frog.fm/concepts/devtools)