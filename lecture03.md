## 1.AP サーバーについて調べる

Q. AP サーバーの名前とバージョンは？

A. Puma 6.4.2

エビデンス画像
![APサーバーの名前とバージョン](images/lecture03/ap-server-version.png)

---

Q. AP サーバーを終了させた場合、引き続きアクセスできるか？

A. できない。

エビデンス画像
![APサーバー停止時にアクセス不可](images/lecture03/access-unavailable-during-ap-server-shutdown.png)

## 2.DB サーバーについて調べる

Q. DB サーバーの名前とバージョンは？

A. MySQL 5.7.44

エビデンス画像
![DBサーバーの名前とバージョン](images/lecture03/mysql-version.png)

---

Q. DB サーバーを終了させた場合、引き続きアクセスできるか？

A. できない。

エビデンス画像
![DBサーバーの停止操作](images/lecture03/mysql-shutdown-operation.png)![DBサーバー停止時のブラウザ表示](images/lecture03/browser-display-during-mysql-shutdown.png)

---

Q. Rails の構成管理ツールは？

A. Bundler

エビデンス画像
![Bundlerのバージョン](images/lecture03/bundler-version.png)

## 3.学んだこと、感じたこと

- Web アプリケーションに関わるキーワードを復習する良い機会になりました。
- Ruby に触れたことがなかったので、Gem や Bundler は初めて知りました。
- Java でポートフォリオを作成していた時はアプリケーションサーバーを意識していませんでした。今後の開発では、トラブルシューティングを迅速に行えるよう、意識したいと思います。
- この講座の本旨ではないと思いますが、MySQL 等の環境構築にかなり時間がかかりました。これから慣れていきたいと思います。
