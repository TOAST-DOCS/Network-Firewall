# NAT

**Security > Network Firewall > 콘솔 사용 가이드 > NAT**

**NAT**(네트워크 주소 변환) 탭에서는 외부에서 접속할 인스턴스와 전용으로 사용할 공인 IP를 선택하여 연결합니다.

<br>

## NAT 설정하기

### 추가

* **추가**를 클릭해 NAT를 생성합니다.
    * NAT 전 공인 IP는 **Network > Floating IP**에서 미리 생성한 IP 중 하나를 선택합니다.  
    * NAT 후 사설 IP에서 선택할 객체는 **객체** 탭에서 미리 생성해야만 **추가**를 클릭해 추가할 수 있습니다.

![nat_add.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.04.05/nat_add_2.png)

### 수정

* **수정**을 클릭해 생성된 NAT를 수정합니다.
    * 수정은 공인 IP와 사설 IP 모두 수정할 수 있습니다.

### 삭제

* **삭제**를 클릭해 생성된 NAT를 삭제합니다.

!!! tip "알아두기"
    * NAT는 목적지 기반 및 1:1 방식만 제공합니다.
    * 포트 기반의 NAT는 제공하지 않습니다.
    * NAT를 생성한 뒤 **정책** 탭에 허용 정책을 추가해야만 공인 통신이 가능합니다.
    * 인스턴스 접속은 NAT를 추가하면서 설정한 NAT 전 공인 IP로 접속 가능합니다. (인스턴스에 직접 Floating IP 연결 불필요)
    * NAT에 설정된 NAT 후 사설 IP를 소유한 인스턴스에 직접 Floating IP를 할당할 경우 통신에 문제가 있을 수 있습니다.
    * NAT 삭제 후 사용하지 않는 NAT 전 공인 IP는 **Network > Floating**에서 직접 삭제하세요.