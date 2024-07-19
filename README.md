# Unity✕MicroCMSお知らせサンプル
MicroCMSで作成したコンテンツをUnityで閲覧することができるサンプルプロジェクトです。
![スクリーンショット 2024-07-19 16 39 31](https://github.com/user-attachments/assets/0de389df-fbfc-40ec-83b2-b3e38ffcf5c6)
![スクリーンショット 2024-07-19 23 25 35](https://github.com/user-attachments/assets/ba4cf2bd-9544-4a9b-ac32-a26a2f74edb0)


## 動作環境
### Unity側
Unity 2022.3.9f1

UniRx 7.1.0 [https://assetstore.unity.com/packages/tools/integration/unirx-reactive-extensions-for-unity-17276?locale=ja-JP](https://assetstore.unity.com/packages/tools/integration/unirx-reactive-extensions-for-unity-17276?locale=ja-JP)

unity-webview 1.0.0 [https://github.com/gree/unity-webview](https://github.com/gree/unity-webview)

### Web側
Node.js ^20

Next.js ^14

next-micro-cms 0.1.0


## ローカル環境での実行方法
MicroSMCに関しては[https://document.microcms.io/manual/signup](https://document.microcms.io/manual/signup)を参照。


### Unity
"unity-html"ディレクトリをプロジェクトとして開く

Assets → Scene → SampleHTMLSceneを開く

Canvas → WebPageManagerのInspector内にあるアクセスしたいURLに変更。(初期値としてLocalhostが登録されています。)


### Next.js
".env.example"を参考に".env"ファイルに必要な環境変数を記入。

"web"ディレクトリ移動後

'''
npm run dev
'''
でローカル環境を立ち上げる
