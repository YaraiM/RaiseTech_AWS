## 1. VPC の作成

### 概要

![概要](images/lecture04/vpc-summary.png)

## 2. EC2 の作成

### 概要

![概要](images/lecture04/ec2-summary.png)

---

### セキュリティグループのルール

HTTP/HTTPS および MyIP アドレスからの SSH を許可するインバウンドルール
![インバウンドルール](images/lecture04/ec2-inbound-rule.png)

外部への通信を許可するアウトバウンドルール
![アウトバウンドルール1](images/lecture04/ec2-outbound-rule.png)

RDS への接続を許可するアウトバウンドルール
![アウトバウンドルール2](images/lecture04/ec2-rds-outbound-rule.png)

## 3. RDS の作成

### 概要

![概要](images/lecture04/rds-summary.png)

---

### サブネットグループ

![サブネットG](images/lecture04/rds-subnet-group.png)

---

### セキュリティグループのルール

MyIP アドレスから MySQL への接続を許可するインバウンドルール
![インバウンドルール](images/lecture04/rds-inbound-rule.png)

EC2 からの MySQL への接続を許可するインバウンドルール
![インバウンドルール](images/lecture04/rds-ec2-inbound-rule.png)

外部への通信を許可するアウトバウンドルール
![アウトバウンドルール](images/lecture04/rds-outbound-rule.png)

## 4. EC2 から RDS への接続確認

![接続確認](images/lecture04/mysql-login-success.png)
