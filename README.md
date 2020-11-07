# iOS-samples

自分がアプリを作るにあたって習作として単機能なアプリを作って実装の確認をしたものをサンプルとしてまとめていくレポジトリ。ソースは基本的に https://github.com/dropcontrol こちらの個人アカウントに上げています。iOSアプリの企画、デザイン、開発などのご相談があれば気軽に info[at]signalcompose.com にお問い合わせください。

* [MapAndLocation](https://github.com/dropcontrol/MapAndLocation/)  
MapKitとCoreLocationCoreLocationをSwiftUI2.0で使うサンプル。参考にしたのは、 https://youtu.be/eDUErLFFgNo こちら。SwiftUI2.0で、delagateをどう書くかの参考にもなると思う。

* [LocationUpdata](https://github.com/dropcontrol/LocationUpdata)  
上記のMapAndLocationからCoreLocationだけを使って、現在の緯度経度をボタンを押すと取得する、というアプリ。delegate（に限らずクラスでも同じだと思う）を使ってボタンなどのアクションによって値をどう変化させるか？@Stateと@Publisedの使い方あたりも参考になると思う。本当はLocationUpdateって名前にしたかったのだがtypoしてる、、、
解説記事＞https://qiita.com/dropcontrol/items/c9f434fb3b9b5806f14e

* [ViewControllerDelegatePattern](https://github.com/dropcontrol/ViewControllerDelegatePattern)
View間で値を渡すパターン。Viewを二つ用意。親から子へ渡すパターンと、子から親へ渡すパターン。またNavigationLinkを使ったページ遷移のサンプルにもなっている。
解説記事＞https://qiita.com/dropcontrol/items/cfceaf0dd3fddcef4543

* [PDFViewer](https://github.com/dropcontrol/PDFViewer/tree/main)
PDFをPageViewControllerを利用してページごとにめくれるビュワー。SwiftUIでのNotificationCenterの設定の仕方や、@ObservedObjectを複数のViewで共有する、などのサンプルにもなっている。@ObservableObjectをどこでインスタンス化して、それをどうViewで渡していくのか？がミソ。ページ番号はNotificationCenterと@objservableObjectのインスタンスの組み合わせで取得／表示している。
解説記事＞https://qiita.com/dropcontrol/items/7e89915470b1cb89270c
