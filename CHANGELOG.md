# ncmb_unity

## [4.0.4] - 2020-01-30

### 変更点
- FIX [#161](https://github.com/NIFCLOUD-mbaas/ncmb_unity/issues/161) 【SNS認証機能】既に認証して登録した会員で、アプリを再インストールし、再度認証してログインを実施するとcurrentUserがnullになります
- FIX [#163](https://github.com/NIFCLOUD-mbaas/ncmb_unity/pull/163) iOS SDK 3.0.3リリースと合わせて、リッチプッシュ通知機能で利用しているUIWebviewからWKWebviewへ変更

※ iOSの場合、[Xcodeの追加設定](https://mbaas.nifcloud.com/doc/current/push/richpush_unity.html#Xcodeの追加設定)が必要となります

## [4.0.3] - 2019-10-17

### 変更点
- FIX [#158](https://github.com/NIFCLOUD-mbaas/ncmb_unity/issues/158) ログイン後に他のユーザを削除する際、CurrentUserがnullになります
- FIX [#150](https://github.com/NIFCLOUD-mbaas/ncmb_unity/issues/150) 4.0.1/セッション切れなどのケースでResponseDataが空文字だと例外で落ちる
- FIX [#149](https://github.com/NIFCLOUD-mbaas/ncmb_unity/issues/149) 4.0.1/ログインユーザを2回以上更新するとエラー
- FIX [#143](https://github.com/NIFCLOUD-mbaas/ncmb_unity/issues/143) ログイン中のユーザを更新すると以降リクエストエラーになる

## [4.0.2] - 2019-09-19

### 変更点
- [#151](https://github.com/NIFCLOUD-mbaas/ncmb_unity/pull/151) iOS13 対応：デバイストークン取得方法の更新

## [4.0.1] - 2019-07-18

### 変更点
- [#138](https://github.com/NIFCLOUD-mbaas/ncmb_unity/pull/138) 匿名会員認証の機能を追加
- [#141](https://github.com/NIFCLOUD-mbaas/ncmb_unity/issues/141) Android 28を対応
- [#140](https://github.com/NIFCLOUD-mbaas/ncmb_unity/pull/140) Unity 2019対応： 'WWW' is obsolete警告を削除
- FIX [#143](https://github.com/NIFCLOUD-mbaas/ncmb_unity/issues/143) ログイン中のユーザを更新すると以降リクエストエラーになる不具合修正

## [4.0.0] - 2018-09-04

### 変更点
- mobile backendの新ドメインAPI(mbaas.api.nifcloud.com、script.mbaas.api.nifcloud.com)からリクエストするように変更
- 新ペイロード(com.nifcloud.mbaas.*)を受け取れるように修正
- mobile backendから送信されるFirebase Cloud Messagingに対応したプッシュ通知を受信できるように変更

### アップグレードガイド
- プッシュ通知の [基本的な使い方＞Android端末へのビルド](https://mbaas.nifcloud.com/doc/current/push/basic_usage_unity.html#Android端末へのビルド) について、ドキュメントをご確認いただき、下記変更点について対応をお願いいたします。
  - google-services.jsonの配置
  - プラグイン名の変更（`com.nifty.cloud.mb.ncmbgcmplugin.` → `com.nifcloud.mbaas.ncmbfcmplugin.` ）

