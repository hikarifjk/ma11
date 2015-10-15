・本サンプルコードはdocomo Developer support提供のトレンド記事抽出SDK for Android（v3.0.1）及びOAuth SDK for Android（v1.1.2）を利用しております。
適宜、最新のSDKの有無をご確認いただき、必要に応じて差し替えてご利用ください。
・サンプルコードの動作に必要なAPIキー、client id、client secretは記載されておりません。
ご自身で取得されたものをご利用ください。

本サンプルコードの各ファイルは下記のように処理を行っております。
package jp.ne.docomo.smt.dev.webcuration.sample_app
・PRNGFixes.java　：SecureRandomの脆弱性対策
・TrendArticleExtractionApplication.java　：トレンド記事抽出SDKサンプル拡張アプリケーションクラス AndroidアプリにおけるSecureRandomの脆弱性対策コードを実行する

package jp.ne.docomo.smt.dev.webcuration.sample_app.activity
・ArticleItemViewHolder.java　：記事一覧およびキーワード検索結果一覧でListView内に表示する項目のViewHolderクラス
・ArticleListFragment.java：記事一覧をListViewで表示するFragment MainActivity内のViewPagerの子要素として生成される
・AuthenticationActivity.java　：認証設定画面
・BaseActivity.java　：MainActivity(記事表示画面)およびKeywordSearchActivity(キーワード検索画面)の基底Activity
・KeywordSearchActivity.java　：キーワード検索画面
・MainActivity.java　：記事表示画面
・MessageDialog.java　：タイトル、メッセージ、およびOKボタンを表示する汎用DialogFragment
・ResultListFragment.java　：キーワード検索結果一覧をListViewで表示するFragment

package jp.ne.docomo.smt.dev.webcuration.sample_app.loader
・BaseLoader.java　：バックグラウンドで安全にデータの取得を行う基底AsyncTaskLoader
・GenreLoader.java　：バックグラウンドでSDKからジャンル情報を取得するAsyncTaskLoader
・SearchLoader.java　：バックグラウンドでSDKからキーワード検索結果を取得するAsyncTaskLoader

package jp.ne.docomo.smt.dev.webcuration.sample_app.oauth
・AccessTokenManager.java　：docomo ID OAuth認証におけるアクセストークンおよび再認証用リフレッシュトークンの管理クラス
・Encryptor.java　：文字列およびバイト配列の暗号化・復号化を行うクラス

package jp.ne.docomo.smt.dev.webcuration.sample_app.provider
・TrendArticleDb.java　：TrendArticleProviderによって管理される各種テーブル定義
・TrendArticleProvide.java　：ジャンル情報、記事コンテンツデータ、記事コンテンツ状態、閲覧ログデータを保持するContentProvider

package jp.ne.docomo.smt.dev.webcuration.sample_app.service
・ArticleStateUpdateService.java　：記事コンテンツ状態を非同期に更新するIntentService 本サンプルアプリでは記事コンテンツの未読・既読状態を更新するのみ
・ArticleUpdateService.java　：記事コンテンツデータを非同期に更新するIntentService
・LogDataSendingService.java　：閲覧ログデータの保存処理および保存されたログデータの一括送信処理を非同期に実行するIntentService
