# 利用者の動作環境

## 分類

パソコンソフトに習い、下記のように分類

- 推奨環境
- 基本動作環境
- 対象外

### ex

#### 推奨環境

- Windows Windows12 x EDGE
- Mac OSX11/12 x Safari
- Android OS は 2 世代前まで x Chrome
- iPhone OS は 2 世代前まで x Safari

※ブラウザは最新バージョンであること

#### 基本動作環境

- Windows Windows10/12 x EDGE
- Mac OSX11/12 x Safari
- Android OS は 2 世代前まで x Chrome
- iPhone OS は 2 世代前まで x Safari
- iPad OS は 2 世代前まで x Safari

※ブラウザは最新バージョンであること

## いつ決定するか

動作環境が広いほど工数に影響を及ぼす
プロジェクトが稼働してからできるだけ早い段階で決定する
ユーザーへの伝え方など細部は後の方になるかもしれないが

## シェア

- 新規開発の場合は参考サイトより、世界のシェアを把握
- 既存改修の場合は GoogleAnalytics などで計測したデータより既存の顧客のシェアを把握

## 作業効率

- 動作環境を広げれば広げるほど、ライブラリの選定やコード量など開発に影響を及ぼす

## ユーザーにはどうやって伝えるべきか

- [ ] 伝えない
- [ ] 動作環境を記載したページを設ける。
- [ ] アクセス時に動作環境を満たさない端末であればアラートを出す

## ユーザーにはどこまで伝えるべきか

- 推奨環境を簡潔に書く
- WebGL を多用したサイトでは対応する CPU を書いてもいいかもしれない

## 参考サイト

statcounter  
<https://gs.statcounter.com/>

Apple 公表データ  
<https://developer.apple.com/support/app-store/>

Google 公表データ  
<https://developer.android.com/about/dashboards/index.html#Platform>

[戻る](./index.md)
