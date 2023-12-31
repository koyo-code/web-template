# コーディングテンプレート

## 概要

通常の静的サイトから WORDPRESS のコーディングまで快適に制作できるテンプレートです。

## 必須環境

1. Node.js
2. Docker(wordpressの場合)

## 必須エディタ

V　S　C　O　D　E

## 必須プラグイン

1. ESLint
2. StyleLint
3. Prettier

## メリット

- 簡単にサイト構築できる
- 静的サイトだけでもok、静的からwordpress構築もシームレスに行える
- lintを通してバグを減らす。scssの順番を自動で揃えてくれる
- dockerで環境構築・データベースを手動で作らなくてもいい
- ローカル環境でSSIが使用できる。
- ファイル更新時にブラウザが更新される(HMR)。
- npmを使って開発ができる。
- huskyを利用し、gitと相性よくweb制作。
- サイトのパフォーマンスアップ

## デメリット

- 更新が少し遅いかも
- 最低限の知識が必要

## 使用方法

1. .env ファイル内をコメントアウトに従って設定
2. npm install
3. npm run prepare

### wordpress

4. docker-compose up -d
5. npm run dev 作業サーバー起動
6. 作業終了時は docker-compose down

## フォルダー構成

- resourceディレクトリに作業用のscss・js・img
- appディレクトリに作業用のhtmlや静的ファイル(resourceでバンドルされない)をセット
- htmlに記述するcssやjsのpassはappディレクトリのassetsの中に合わせる

### wordpress

- docker-compose up -dでappディレクトリに作成される。その中でテンプレートを構成。
- appディレクトリがwp-content等と同じ階層になる。
  静的ファイルはそこに配置。

## html.css.js

- bodyに独自のdata属性(data-page="top")等を使用してページのcssやjsを使用するときに判断させてcssのスコープやjsのスコープを制限している。
# oeuf-
‣敷ⵢ整灭慬整�