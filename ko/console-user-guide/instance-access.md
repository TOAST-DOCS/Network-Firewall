# 인스턴스 접속

**Security > Network Firewall > 콘솔 사용 가이드 > 인스턴스 접속**

Network Firewall을 생성하고 연결 설정을 모두 완료한 후 Network Firewall을 경유하여 인스턴스에 접속합니다.

<br>

## 설정하기
예를 들어, 1개의 프로젝트 내 2개의 Spoke VPC로 3개의 서브넷을 구성하고, 외부에서 웹방화벽 접속이 필요할 경우 아래와 같이 NAT, ACL을 설정합니다.

<img src="https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.09.12/instance-access.png" height="65%" />

* **Network Firewall > NAT > 목적지** 탭으로 이동
* 추가 버튼 클릭 후 목적사용자 가이드 사용자 지 NAT 설정
    * 설정 전 객체 탭에서 목적지 IP 객체 생성과 여분의 플로팅 IP 필요
    <img src="https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.09.12/nat-add.png" height="65%" />

* **Network Firewall > 정책 > ACL** 탭에서 필요한 ACL을 허용
    * 출발지/목적지 인터페이스는 ALL 설정 가능
     <img src="https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.09.12/access_acl.png" height="65%" />

!!! danger "주의"

    출발지 IP를 보안 그룹에서 허용해야만 인스턴스에 접속 가능합니다.