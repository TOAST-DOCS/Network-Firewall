# ACL

**Security > Network Firewall > 콘솔 사용 가이드 > ACL**

**ACL** 탭에서는 Network Firewall과 연결된 VPC 간 트래픽과 인바운드/아웃바운드 트래픽을 제어할 수 있습니다.

<br>

## ACL 설정하기

### 추가

* 출발지, 목적지, 목적지 포트를 기반으로 정책을 추가할 수 있습니다.
    * 이미 만들어진 객체를 통해 출발지, 목적지, 목적지 포트를 선택합니다.
* 정책의 상태(활성화/비활성화)와 동작(허용/차단), 스케줄을 설정 및 정책별 로깅 여부 등의 옵션을 설정하여 정책을 추가할 수 있습니다.
* 스케줄 기능은 정책의 상태를 활성화 한 이후에 동작합니다(정책이 비활성화되어 있을 경우 스케줄 기능이 적용되지 않습니다.).

![acl_add.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.05.27/acl_add.png)

### 복사

* **복사**를 클릭해 정책을 복사할 수 있습니다.
    * 복사: 복사하고자 하는 정책과 동일한 정책을 복사
    * 역방향 복사: 복사하고자 하는 정책의 출발지와 목적지를 변경하여 복사
    ![acl_copy.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/23.09.07/acl_copy_1.png)

!!! tip "알아두기"
    복사된 정책은 비활성화됩니다. 사용이 필요할 경우 **수정**을 클릭해 정책을 활성화한 뒤 사용하세요.
    
### 수정

* **수정**을 클릭해 정책을 수정할 수 있습니다.

### 이동

* **이동**을 클릭해 정책을 이동할 수 있습니다.
    * default-deny 정책 아래로는 이동이 불가능합니다.
    ![acl_move.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/23.09.07/acl_move_1.png)

### 삭제

* **삭제**를 클릭해 정책을 삭제할 수 있습니다.

!!! danger "주의"
    한번 삭제한 정책은 복구할 수 없으며, default-deny 정책은 삭제할 수 없습니다.

### 정책 일괄 다운로드

* 정책 탭에 생성되어 있는 정책 전체를 한번에 다운로드할 수 있습니다.

### 정책 일괄 등록

* 내려받은 템플릿을 사용하여 정책을 한 번에 등록할 수 있습니다.

![acl_batch.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/23.09.07/acl_batch_1.png)