## 인터페이스

**Security > Network Firewall > 콘솔 사용 가이드 > 인터페이스**

**인터페이스** 탭에서는 Network Firewall에 사용할 인터페이스를 생성하고 관리합니다.

![(interface1)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/5.interface/interface1.png)

<br>

## 인터페이스 설정하기

### 추가
* **추가**를 클릭해 인터페이스를 추가합니다.
    * 이름을 입력하고, VPC, 서브넷을 선택합니다.
    ![(interface2)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/5.interface/interface2.png)

### 수정
* **수정**을 클릭해 인터페이스를 수정할 수 있습니다.
    * VPC와 서브넷은 수정이 불가능합니다.

### 삭제
* **삭제**를 클릭해 인터페이스를 삭제할 수 있습니다.

### 사용 설정
* 오버플로우 메뉴에서 인터페이스를 사용 또는 미사용으로 설정할 수 있습니다.
![(interface4)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/5.interface/interface4.png)

!!! tip "알아두기"

    수정은 이름과 설명만 수정 가능합니다.

!!! danger "주의"
    
    * 사용 중인 인터페이스는 삭제할 수 없습니다.
        * ACL 및 라우트 설정에 해당 인터페이스가 없고, 인터페이스 탭에서 미사용 상태여야만 삭제 가능합니다.
    * 인터페이스 미사용 설정 시 통신에 문제가 있을 수 있습니다.