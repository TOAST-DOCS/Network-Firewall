## Network Firewallの概要

**Security > Network Firewall > 概要**

Network Firewallは、NHN Cloudで使用するインフラ資産を安全に保護するために提供するネットワークセキュリティサービスです。
NHN Cloudに特化したアクセス制御を適用でき、別途、ファイアウォール製品を使用しなくても、簡単にファイアウォール機能を使用できます。

!!! tip "ポイント"

    Network Firewallサービスは、韓国(パンギョ)リージョンの場合、新規のネットワーク環境でのみ利用できます。
    韓国(パンギョ)リージョンで2022年3月7日以前に作成したプロジェクトは、改善前のネットワーク環境であるため、Network Firewallサービスを利用するにはプロジェクトを新しく作成する必要があります。

<br>

## 主な機能

* 効率的にネットワーク通信ポリシーを管理できます。
    * ステートフル(Stateful)方式で、1つのポリシーでトラフィックを制御します。
* Hub-Spoke構造で、外部の攻撃から安全にインスタンスを保護できます。
    * VPC間の内部トラフィックとインバウンド/アウトバウンドトラフィックを制御します。
* 複数のインターフェースを接続し、ルートを設定してトラフィックを制御できます。
* インターネット環境において、サイト間の暗号化されたトンネルを通じて安全な仮想プライベートネットワーク(VPN)を提供します。    
* ネットワークの遮断と許可に対するリアルタイムのログ検索とバックアップ機能を提供します。
    * お客様の環境に合わせて、様々なバックアップ方式を提供します(Syslog、Object Storage、Log & Crash Search)。
* 安定した運用のために高可用性(冗長化)を提供します。

<br>

## サービス構成図
サービスは以下の5つの形態で構成できます。

### 1つのプロジェクト
<img src="https://static.toastoven.net/prod_nfw/26.07.28/1.overview/architecture1.png" height="70%">

### 1つ以上のプロジェクト
<img src="https://static.toastoven.net/prod_nfw/26.07.28/1.overview/architecture2.png" height="70%" width="100%" />


### 異なるリージョン間のプロジェクト
<img src="https://static.toastoven.net/prod_nfw/26.07.28/1.overview/architecture3.png" height="70%" width="100%" />


### 1つのプロジェクト内の2つのSpoke VPC
<img src="https://static.toastoven.net/prod_nfw/26.07.28/1.overview/architecture4.png" height="70%" width="100%" />


### 1つのVPC内の複数のサブネット
<img src="https://static.toastoven.net/prod_nfw/26.07.28/1.overview/architecturer5.png" height="50%" width="100%" />


!!! tip "ポイント"

    * 上記の構成図は一般的な構成であり、お客様の環境によってNetwork Firewallを除くWEB、WAS、Load Balancerなどの構成が異なる場合があります。

    * 他のリージョンのプロジェクト環境では、同じプロジェクト間でのみ構成可能です。詳細については、[ユーザーガイド](https://docs.nhncloud.com/ko/Network/Peering%20Gateway/ko/console-guide/)をご参照ください。

!!! danger "注意"

    サービス構成時、2022年3月7日以前に構成したネットワーク環境とは接続できません。
    
    例えば、2022年3月7日以前に構成したネットワーク環境を使用するプロジェクトと、それ以降に構成したネットワーク環境を使用するプロジェクトが作成されている場合、新規のネットワーク環境にNetwork Firewallを作成することはできますが、改善前のネットワーク環境をSpoke VPCとして使用することはできません。
