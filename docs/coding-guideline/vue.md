# Vue コーディングガイドライン

- [ ] スタイルをコンポーネントに書く
- [ ] 外部ファイルに書く

## コンポーネント

### インポート

- 下記の順番で記載
- 順位の小さい順に先に記載
- 次にアルファベット順

- フレームワーク本体 vue, nuxtjs etc...
- Vue に依存するライブラリ vee-validate etc...
- Vue に依存しないライブラリ lodash, axios etc...
- 1 行スペース
- 定数
- ユーティリティ

### Vue コンポーネント外

- 当コンポーネントでのみ使用する定数
- 当コンポーネント用の型

### Vue ライブラリのコンポーネントタグ

- パスカルケースで書く
- 要素の記載順 https://eslint.vuejs.org/rules/attributes-order.html eslint に入レル

特定のエレメントにイベントリスナー登録する場合
ref を使う

###

- asyncData
  SEO 施策が必要なページ ... 使うこと
  SEO 施策が必要なページ ... 使わないこと
- data
- watch
  使用禁止
- mounted
- beforeDestroy
  初期表示で作成したイベントを remove する
- methods
  スタイル
  // 必ずクラス名を付けること

[戻る](../index.md)
