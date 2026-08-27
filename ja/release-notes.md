<!-- pre-align:aligned sig=f90308ef9ace -->

<a id="network-firewall-release-notes"></a>
## Network Firewallリリースノート { #network-firewall-release-notes }

**Security > Network Firewall > リリースノート**

<a id="july-28-2026"></a>
## 2026. 07. 28. { #july-28-2026 }

<a id="added-features"></a>
### 機能追加 { #added-features }

* インターフェース管理機能の追加
    * インターフェースタブで自由にインターフェースを作成し、Network Firewallに接続できます。
* 送信元NAT機能の追加
    * インスタンスが外部と通信する際、Network FirewallでNATを設定できます。
        * 1:1またはN:1で設定できます。

<a id="feature-updates"></a>
### 機能改善・変更 { #feature-updates }

* ルート追加画面の改善
    * ゲートウェイを直接入力せず、選択したイーサネットに合わせてインターフェースを選択できるよう、プルダウン形式に変更しました。
* ACLポリシー追加画面の改善
    * ACLポリシーの追加時に、送信元/宛先インターフェースを選択できるよう画面を改善しました。

<a id="removed-features"></a>
### 機能削除 { #removed-features }

* MTUサイズ設定オプションの削除
    * Network Firewallで使用中のインターフェースのMTUサイズ設定オプションを削除しました。

<a id="october-28-2025"></a>
## 2025. 10. 28. { #october-28-2025 }

<a id="october-28-2025-feature-updates"></a>
### 機能改善 { #october-28-2025-feature-updates }

* コピー機能の改善
    * 双方向のポリシーコピーが可能となるよう改善しました。

<a id="october-28-2025-removed-features"></a>
### 機能削除 { #october-28-2025-removed-features }

* サポートアルゴリズムの削除
    * セキュリティ面で脆弱な暗号化及び完全性アルゴリズムを削除しました。
        * 暗号化アルゴリズム: DES、MD5、SHA1
        * 完全性アルゴリズム: DH Groups 1, 2, 5

<a id="april-29-2025"></a>
## 2025. 04. 29. { #april-29-2025 }

<a id="april-29-2025-added-features"></a>
### 機能追加 { #april-29-2025-added-features }

* ミラーリング管理機能の追加
    * Network Firewallを経由するトラフィックを特定の宛先にコピーして送信できます。

<a id="october-15-2024"></a>
## 2024. 10. 15. { #october-15-2024 }

<a id="october-15-2024-added-features"></a>
### 機能追加 { #october-15-2024-added-features }

* ルート管理機能の追加
    * ルートを設定して、Network Firewallを経由する通信を振り分けて管理できます。

<a id="october-15-2024-feature-updates"></a>
### 機能改善 { #october-15-2024-feature-updates }

* Network Firewall作成手順の改善
    * Network Firewallの作成時にアベイラビリティゾーンを選択できるよう改善しました。

<a id="july-23-2024"></a>
## 2024. 07. 23. { #july-23-2024 }

<a id="july-23-2024-feature-updates"></a>
### 機能追加/改善 { #july-23-2024-feature-updates }

* Network Firewall削除機能の追加
    * Network Firewallを削除できる機能を追加しました。
* Network Firewall構成変更機能の追加    
    * Network Firewallのタイプを単一または冗長化から選択できる機能を追加しました。
* トラフィックログの改善
    * トラフィックログに表示されるカラム項目を追加しました。

<a id="june-25-2024"></a>
## 2024. 06. 25. { #june-25-2024 }

<a id="june-25-2024-added-features"></a>
### 機能追加 { #june-25-2024-added-features }

* IPSec VPN管理機能の追加
    * 遠隔地と安全なプライベート通信を行えるよう、IPSec VPN機能を追加しました。
* ロギング機能の追加
    * ACLポリシー別にロギングの有無を設定できる機能を追加しました。

<a id="june-25-2024-feature-updates"></a>
### 機能改善・変更 { #june-25-2024-feature-updates }

* ポリシースケジュール機能の改善
    * ポリシーページでスケジュール使用の有無を確認できるようUIを改善しました。
    * スケジュールを10分単位で設定できるよう改善しました。
* モニター画面の改善
    * セッショングラフで内/外部セッションを区別して表示されるよう改善しました。
    * 検索条件を改善しました。

<a id="may-14-2024"></a>
## 2024. 05. 14. { #may-14-2024 }

<a id="may-14-2024-added-features"></a>
### 機能追加 { #may-14-2024-added-features }

* NAT修正機能の追加
    * NATメインページに「修正」機能を追加しました。

<a id="march-26-2024"></a>
## 2024. 03. 26. { #march-26-2024 }

<a id="march-26-2024-feature-updates"></a>
### 機能追加/改善 { #march-26-2024-feature-updates }

* MTU設定機能の追加
    * Network Firewallで使用中のインターフェースのMTUサイズを設定できるよう機能を追加しました。   
* Syslogポート設定機能の追加
    * Syslog設定時にポート番号を設定できる機能を追加しました。
* UI改善
    * ログ項目のうち、プロトコルが数字ではなく文字で表示されるようUIを改善しました。

<a id="march-26-2024-removed-features"></a>
### 機能削除 { #march-26-2024-removed-features }

* NAT設定機能の削除
    * オプションで提供していたNAT有効化機能を削除し、Network Firewallの作成時に自動で有効化されるよう変更しました。

<a id="january-23-2024"></a>
## 2024. 01. 23. { #january-23-2024 }

<a id="january-23-2024-added-features"></a>
### 機能追加 { #january-23-2024-added-features }

* 機密情報の暗号化のために、SKM(Secure Key Manager)サービスとの連携を追加しました。

<a id="bug-fixes"></a>
### バグ修正 { #bug-fixes }

* 断続的にAPIレスポンスが遅くなる現象を修正しました。

<a id="december-19-2023"></a>
## 2023. 12. 19. { #december-19-2023 }

<a id="december-19-2023-feature-updates"></a>
### 機能追加/改善 { #december-19-2023-feature-updates }

* クォータ管理の追加
    * プロジェクト別のリソースを確認できるよう、クォータ管理機能を追加しました。
* 検索条件の追加
    * ポリシーの一括ダウンロード時に検索条件を追加しました。
* 機密情報処理の改善
    * CloudTrailに積載するログのうち、機密情報をマスキング処理できるよう改善しました。

<a id="october-31-2023"></a>
## 2023. 10. 31. { #october-31-2023 }

<a id="new-service-launch"></a>
### Network Firewall新規サービスリリース { #new-service-launch }

Network Firewallは、NHN Cloudで使用するインフラ資産を安全に保護するために提供するネットワークセキュリティサービスです。
