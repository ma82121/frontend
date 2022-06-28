# コンポーネント設計

## 分類

「コンポーネント」の分類を行い明分化する

- 最小コンポーネント
- 機能コンポーネント
- Screenコンポーネント Pageコンポーネントと1対1の関係
- Hubコンポーネント(Nuxtの場合)
- Pageコンポーネント
- Appコンポーネント(Nextの場合)

### コンポーネントの設計

- 親コンポーネントから決められた型のデータを受け取る
- 受け取ったデータを元に画面描画
- コンポーネント内のDOMに必要なイベントを登録（使わなくなったら削除すること）
- windowに必要なイベントを登録（使わなくなったら削除すること）
- イベント発火時に決められた型のデータを親コンポーネントへ渡す
- nuxt-linkやrouter.pushを使い他画面へ遷移する
- 外部リンクへ遷移する

## Screenコンポーネント

Pageコンポーネントと1対1の関係

/components/Screen/ScreenFoo.vue

▼分割したい場合
/components/Screen/ScreenFoo/ScreenFoo.vue
/components/Screen/ScreenFoo/ScreenFooSub1.vue
/components/Screen/ScreenFoo/ScreenFooSub2.vue

▼動的ページ(/pages/article/_id.vue)の場合
/components/Screen/ScreenArticleId.vue

## Templateコンポーネント

- Template専用グローバル変数の繋ぎ込み

## pageコンポーネント

エントリーポイント
Next,Nuxtではpagesにあたる

- titleタグやmetaタグなどhead情報を書く
- 以下の情報を取得し評価を行う
- 例えばIDが設計通りの文字列で構成されているかなど
  - GET変数
  - POST変数
  - Strorage情報
- 適切な値であればこScreenコンポーネントへ渡す
- 適切な値が揃っていなければエラー画面に自動遷移させる

[戻る](./index.md)
