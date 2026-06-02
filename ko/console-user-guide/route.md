# 라우트

**Security > Network Firewall > 콘솔 사용 가이드 > 라우트**

**라우트** 탭에서는 Network Firewall을 경유하는 통신의 경로를 지정할 수 있습니다.

![policy-route.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.09.12/policy-route.png)

> [참고]
> 
> * Network Firewall의 기본 게이트웨이는 NAT 이더넷이며, 수정하거나 삭제할 수 없습니다.
> * 라우트 설정이 변경될 경우 통신에 문제가 있을 수 있으므로 유의하여 설정하세요.  

### 추가

* **추가**를 클릭해 이더넷을 선택하고, 목적지와 게이트웨이를 입력합니다. 
    * 목적지: 서브넷 형식으로 입력
    * 이더넷: NAT, TRAFFIC, VPN(IPSec VPN 기능 사용 시) 중 선택
    * 게이트웨이: 호스트 형식으로 입력

> [참고]
> 
> * 이더넷을 VPN으로 선택할 경우 게이트웨이는 지정하지 않아도 됩니다.
> * IPSec VPN과 연동된 사설 IP 대역에 대한 라우트 설정은 반드시 이더넷을 VPN으로 설정하세요.
> * 목적지 서브넷 입력 시 아래와 같은 유효성 메시지가 노출될 경우 서브넷 범위를 사전에 확인하여 서브넷의 시작 IP로 입력하세요.
>   * [예시]
>       * 192.168.199.0/21 (X) → 192.168.192.0/21 (O)
>       * 172.16.100.0/20 (X) → 172.16.96.0/20 (O)
>       * 10.10.10.130/25 (X) → 10.10.10.128/25 (O)
> 
> ![route_add.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.09.12/route_add.png)

### 수정

* **수정**을 클릭해 라우트를 수정할 수 있습니다.

### 삭제

* **삭제**를 클릭해 라우트를 삭제할 수 있습니다.

<br>