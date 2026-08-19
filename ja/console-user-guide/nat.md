<!-- machine_translated: true -->

<!-- pre-align:aligned sig=b5a6dd9155ad -->

<a id="nat"></a>
## NAT { #nat }

**Security > Network Firewall > コンソール使用ガイド > NAT**

**NAT**(ネットワークアドレス変換)タブでは、インスタンスが外部と通信する際に外部に露出するパブリックIPを設定する送信元NATと、外部から接続するインスタンスと専用で使用するパブリックIPを選択して接続する宛先NATを設定できます。

<br>

<a id="configure-source-nat"></a>
## 送信元NATを設定する { #configure-source-nat }

<a id="add"></a>
### 追加 { #add }

* **追加**をクリックして送信元NATを作成します。
    * NAT前IPで選択するオブジェクトは、**オブジェクト**タブであらかじめ作成しておくことで、**追加**をクリックして追加できるようになります。
    * NAT後IPは、**Network > フローティングIP**であらかじめ作成したIPから1つ選択します。 

![nat_add.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/6.nat/nat2-pub.png)

<a id="modify"></a>
### 修正 { #modify }

* **修正**をクリックして作成された送信元NATを修正します。
    * 修正はパブリックIPとプライベートIPの両方を修正できます。

<a id="delete"></a>
### 削除 { #delete }

* **削除**をクリックして作成された送信元NATを削除します。

<br>

<a id="configure-destination-nat"></a>
## 宛先NATを設定する { #configure-destination-nat }

<a id="configure-destination-nat-add"></a>
### 追加 { #configure-destination-nat-add }

* **追加**をクリックして宛先NATを作成します。
    * NAT前IPは、**Network > フローティングIP**であらかじめ作成したIPから1つ選択します。  
    * NAT後IPで選択するオブジェクトは、**オブジェクト**タブであらかじめ作成しておくことで、**追加**をクリックして追加できるようになります。

![nat_add.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/6.nat/nat3-pub.png)

<a id="configure-destination-nat-modify"></a>
### 修正 { #configure-destination-nat-modify }

* **修正**をクリックして作成された宛先NATを修正します。
    * 修正はパブリックIPとプライベートIPの両方を修正できます。

<a id="configure-destination-nat-delete"></a>

### 削除 { #configure-destination-nat-delete }

* **削除**をクリックして作成された宛先NATを削除します。

!!! tip "ポイント"
    * ポートベースの宛先NATは提供していません。
    * NATを作成した後、**ポリシー**タブに許可ポリシーを追加して初めてパブリック通信が可能になります。
    * インスタンス接続は、宛先タブにNATを追加する際に設定したNAT前IPで接続できます。(インスタンスへの直接的なフローティングIP接続は不要)
    * NATに設定されたNAT後IPを所有するインスタンスに、直接フローティングIPを割り当てた場合、通信に問題が発生する可能性があります。
    * NAT削除後、使用しないNAT前IPは**Network > フローティングIP**から直接削除してください。!!! danger "注意"
    * 送信元または宛先 NAT を追加する際に選択する NAT 前後の IP（プライベート）は、追加する時点で **[オブジェクト]** タブに **[タイプ-サブネット]** として作成されたオブジェクトを表示します。
        * 選択されたオブジェクトは、NAT を追加した後に **[オブジェクト]** タブで変更または削除されても、NAT 設定には影響しません（オブジェクトと NAT は互いに連動しません）。
        例えば、宛先 NAT を追加する際に 10.10.10.10/32 で作成されたオブジェクトを選択して NAT を追加した状態で、**[オブジェクト]** タブに移動して 10.10.10.10/32 で作成されたオブジェクトを 10.10.10.20/32 に変更しても、NAT 設定は変更されません。