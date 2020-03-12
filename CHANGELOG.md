# ncmb_unity

## [4.0.0] - 2018-09-04

### 変更点
- mobile backendの新ドメインAPI(mbaas.api.nifcloud.com、script.mbaas.api.nifcloud.com)からリクエストするように変更
- 新ペイロード(com.nifcloud.mbaas.*)を受け取れるように修正
- mobile backendから送信されるFirebase Cloud Messagingに対応したプッシュ通知を受信できるように変更

### アップグレードガイド
- プッシュ通知の [基本的な使い方＞Android端末へのビルド](https://mbaas.nifcloud.com/doc/current/push/basic_usage_unity.html#Android端末へのビルド) について、ドキュメントをご確認いただき、下記変更点について対応をお願いいたします。
  - google-services.jsonの配置
  - プラグイン名の変更（`com.nifty.cloud.mb.ncmbgcmplugin.` → `com.nifcloud.mbaas.ncmbfcmplugin.` ）

