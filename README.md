# farecaster-frames-first
FarecasterのFramesを理解するために作成

# 手順
## 0. asdf でのバージョン設定
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

## 2. X

# 参考
* [Farecaster Docs - Getting Started](https://docs.farcaster.xyz/developers/frames/getting-started)