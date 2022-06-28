# Vueコーディングガイドライン



## コンポーネント

### インポート

- 下記の順番で記載
- 順位の小さい順に先に記載
- 次にアルファベット順

- フレームワーク本体 vue, nuxtjs etc...
- Vueに依存するライブラリ vee-validate etc...
- Vueに依存しないライブラリ lodash, axios etc...
- 1行スペース
- 定数
- ユーティリティ

### Vueコンポーネント外

- 当コンポーネントでのみ使用する定数
- 当コンポーネント用の型

### Vueライブラリのコンポーネントタグ

- パスカルケースで書く
- 要素の記載順 https://eslint.vuejs.org/rules/attributes-order.html eslintに入レル

特定のエレメントにイベントリスナー登録する場合
refを使う

### 

- asyncData
SEO施策が必要なページ ... 使うこと
SEO施策が必要なページ ... 使わないこと

data
watch
使用禁止
mounted
beforeDestroy
初期表示で作成したイベントをremoveする
methods
スタイル
// 必ずクラス名を付けること



[戻る](../index.md)