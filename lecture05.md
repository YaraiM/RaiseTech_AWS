## 1. EC2 にサンプルアプリケーションをデプロイ

### Puma のみで動作確認

Puma の起動状態確認
![Puma起動状態](images/lecture05/puma-status.png)

Curl で動作確認
![Puma動作確認](images/lecture05/confirm-operation-by-puma.png)

### Puma ＋ Unix Socket を使った動作確認

![Puma＋Unix Socket動作確認](images/lecture05/confirm-operation-by-puma-and-unix-socket.png)

### Nginx の起動確認

Nginx の起動状態確認
![ステータス](images/lecture05/confirm-nginx-working1.png)

ブラウザで表示
![ブラウザの表示](images/lecture05/confirm-nginx-working2.png)

### Puma ＋ Unix Socket ＋ Nginx で動作確認

Curl で動作確認
![Curlで動作確認](images/lecture05/confirm-operation-by-puma-andnginx1.png)

ブラウザで動作確認
![ブラウザで動作確認](images/lecture05/confirm-operation-by-puma-andnginx2.png)

## 2. ALB の作成および動作確認

### マネジメントコンソール画面

ALB の概要
![ALB概要](images/lecture05/ALB-Summary.png)

ターゲットグループの概要
![TG概要](images/lecture05/TG-Summary.png)

### ALB 経由での動作確認

ブラウザで動作確認
![ブラウザで動作確認](images/lecture05/confirm-operation-by-ALB.png)

## 3. S3 の作成およびアプリケーション画像のアップロード・閲覧

### マネジメントコンソール画面

S3 の概要
![S3概要](images/lecture05/S3-summary.png)

S3 のアクセス許可設定
![S3アクセス](images/lecture05/S3-access-permission.png)

S3 の ACL 設定
![S3ACL](images/lecture05/S3-ACL.png)

S3 にアクセスするための IAM ロール作成
![IAMロール作成](images/lecture05/IAM-role-s3.png)

EC2 に S3 にアクセスするための IAM ロールをアタッチ
![IAMアタッチ](images/lecture05/EC2-IAM-role.png)

### アプリケーション側で S3 にアクセスする設定

config/environments/development.rb の設定
![設定1](images/lecture05/config_environments_development.rb.png)

config/storage.yml の設定
![設定2](images/lecture05/config_storage.yml.png)

S3 のバケットネームを.bash_profile に環境変数として設定
![設定3](images/lecture05/bash_profile.png)

### S3 の動作確認

※画像がアップロードされている
![S3動作確認](images/lecture05/confirm-images-on-s3.png)

## 4. インフラ構成図

![構成図](images/lecture05/infrastructure-diagram.png)
