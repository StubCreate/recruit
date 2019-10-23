# recruit
*Webpack 4 (もしくは 3) で Bootstrap v4.0 を利用するサンプルコード
*参照:https://laboradian.com/sample-code-bootstrap4-webpack3/
*これにGulpを足す

*//ディレクトリ

*project
*├─ package.json
*├─ webpack.config.js
*├─ gulpfile.js
*├─ dist/ （Webサーバに配置するファイルを格納するフォルダ）
*│    ├─ index.html （今回は直接編集します）
*│    ├─ js/
*│    │  └─ main.js （JavaScript コードは全てここにまとめられます）
*│    └─ css
*│       └─ main.css （CSS コードは全てここにまとめられます）
*├─ src/  (開発者が作成するファイルを配置するフォルダ)
*│    ├─ js/
*│    │  ├─ app.js （JavaScript のエントリポイント）
*│    └─ scss/
*│       ├─ app.scss （CSS のエントリポイント）
*│       └─ _custom.scss （Bootstrapを利用するコードはここに書きます）
*└─ node_modules/
*     ├
   （省略）

*   //使用プラグイン
*   gulp-sass（sassをコンパイルするためのプラグイン）
*   autoprefixer（必要なベンダープレフィックスを自動で付与）
*   gulp-postcss（autoprefixerを利用するため）
*   browser-sync（ブラウザを自動リロード）
*   gulp-plumber（sassのコンパイルエラーを検知）
*   gulp-notify（デスクトップ通知するためのプラグイン）

*//設定

*//プロジェクトのディレクトリに移動
*$ cd path/to/your-project

*//プロジェクトの初期化
*npm init -y

*//gulp本体のインストール
*$ npm install -D gulp

*//各プラグインのインストール
*$ npm install -D gulp-sass

*$ npm install -D autoprefixer

*$ npm install -D gulp-postcss

*$ npm install -D browser-sync

*$ npm install -D gulp-plumber

*$ npm install -D gulp-notify

*//webpackをgulpで使用する為のプラグイン
*npm i -D gulp webpack webpack-stream

*//npmのパッケージでBootstrapをインストール
*$ npm install --save bootstrap jquery popper.js

*$ npm install --save-dev webpack webpack-cli mini-css-extract-plugin sass-loader node-sass style-loader css-loader precss autoprefixer postcss-loader

*//開発用のファイルを生成
*$ ./node_modules/.bin/webpack -d

*//本番用の圧縮ファイルを生成
*$ ./node_modules/.bin/webpack -p

*//タスクの実行
*npx gulp









   
