# コンポーネント設計

## 分類

「コンポーネント」を明分化する

- 最小コンポーネント
- 機能コンポーネント
- Screen コンポーネント Page コンポーネントと 1 対 1 の関係
- Hub コンポーネント(Nuxt の場合)
- Page コンポーネント
- App コンポーネント(Next の場合)

### コンポーネントの設計

- 親コンポーネントから決められた型のデータを受け取る
- 受け取ったデータを元に画面描画
- コンポーネント内の DOM に必要なイベントを登録（使わなくなったら削除すること）
- window に必要なイベントを登録（使わなくなったら削除すること）
- イベント発火時に決められた型のデータを親コンポーネントへ渡す
- nuxt-link や router.push を使い他画面へ遷移する
- 外部リンクへ遷移する

## Screen コンポーネント

Page コンポーネントと 1 対 1 の関係

/components/Screen/ScreenFoo.vue

▼ 分割したい場合
/components/Screen/ScreenFoo/ScreenFoo.vue
/components/Screen/ScreenFoo/ScreenFooSub1.vue
/components/Screen/ScreenFoo/ScreenFooSub2.vue

▼ 動的ページ(/pages/article/\_id.vue)の場合
/components/Screen/ScreenArticleId.vue

## Template コンポーネント

- Template 専用グローバル変数の繋ぎ込み

## page コンポーネント

エントリーポイント
Next,Nuxt では pages にあたる

- title タグや meta タグなど head 情報を書く
- 以下の情報を取得し評価を行う
- 例えば ID が設計通りの文字列で構成されているかなど
  - GET 変数
  - POST 変数
  - Strorage 情報
- 適切な値であればこ Screen コンポーネントへ渡す
- 適切な値が揃っていなければエラー画面に自動遷移させる

[戻る](./index.md)
