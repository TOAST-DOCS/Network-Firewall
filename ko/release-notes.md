<!-- pre-align:aligned sig=f90308ef9ace -->

<a id="network-firewall-release-notes"></a>
## Network Firewall 릴리스 노트 { #network-firewall-release-notes }

**Security > Network Firewall > 릴리스 노트**

<a id="july-28-2026"></a>
## 2026. 07. 28. { #july-28-2026 }

<a id="added-features"></a>
### 기능 추가 { #added-features }

* 인터페이스 관리 기능 추가
    * 인터페이스 탭에서 자유롭게 인터페이스를 만들고 Network Firewall에 연결할 수 있습니다.
* 출발지 NAT 기능 추가
    * 인스턴스가 외부 통신할 때 Network Firewall에서 NAT를 설정할 수 있습니다.
        * 1:1 또는 N:1로 설정할 수 있습니다.

<a id="feature-updates"></a>
### 기능 개선/변경 { #feature-updates }

* 라우트 추가 화면 개선
    * 게이트웨이를 직접 입력하지 않고 선택한 이더넷에 맞춰 인터페이스를 선택할 수 있도록 드롭박스 형태로 변경했습니다.
* ACL 정책 추가 화면 개선
    * ACL 정책 추가 시 출발지/목적지 인터페이스를 선택할 수 있도록 화면을 개선했습니다.

<a id="removed-features"></a>
### 기능 삭제 { #removed-features }

* MTU 크기 설정 옵션 삭제
    * Network Firewall에서 사용중인 인터페이스의 MTU 크기 설정 옵션을 삭제했습니다.

<a id="october-28-2025"></a>
## 2025. 10. 28. { #october-28-2025 }

<a id="october-28-2025-feature-updates"></a>
### 기능 개선 { #october-28-2025-feature-updates }

* 복사 기능 개선
    * 양방향 정책 복사가 가능하도록 개선했습니다.

<a id="october-28-2025-removed-features"></a>
### 기능 삭제 { #october-28-2025-removed-features }

* 지원 알고리즘 삭제
    * 보안에 취약한 암호화 및 무결성 알고리즘을 삭제했습니다.
        * 암호화 알고리즘: DES, MD5, SHA1
        * 무결성 알고리즘: DH Groups 1, 2, 5

<a id="april-29-2025"></a>
## 2025. 04. 29. { #april-29-2025 }

<a id="april-29-2025-added-features"></a>
### 기능 추가 { #april-29-2025-added-features }

* 미러링 관리 기능 추가
    * Network Firewall을 경유하는 트래픽을 특정 목적지로 복사하여 전송할 수 있습니다.

<a id="october-15-2024"></a>
## 2024. 10. 15. { #october-15-2024 }

<a id="october-15-2024-added-features"></a>
### 기능 추가 { #october-15-2024-added-features }

* 라우트 관리 기능 추가
    * 라우트를 설정하여 Network Firewall을 경유하는 통신을 분기하여 관리할 수 있습니다.

<a id="october-15-2024-feature-updates"></a>
### 기능 개선 { #october-15-2024-feature-updates }

* Network Firewall 생성 절차 개선
    * Network Firewall 생성 시 가용성 영역을 선택할 수 있도록 개선했습니다.

<a id="july-23-2024"></a>
## 2024. 07. 23. { #july-23-2024 }

<a id="july-23-2024-feature-updates"></a>
### 기능 추가/개선 { #july-23-2024-feature-updates }

* Network Firewall 삭제 기능 추가
    * Network Firewall을 삭제할 수 있는 기능을 추가했습니다.
* Network Firewall 구성 변경 기능 추가    
    * Network Firewall 타입을 단일 또는 이중화를 선택할 수 있는 기능을 추가했습니다.
* 트래픽 로그 개선
    * 트래픽 로그에 노출되는 칼럼 항목을 추가했습니다.

<a id="june-25-2024"></a>
## 2024. 06. 25. { #june-25-2024 }

<a id="june-25-2024-added-features"></a>
### 기능 추가 { #june-25-2024-added-features }

* IPSec VPN 관리 기능 추가
    * 원격지와 안전한 사설 통신이 가능하도록 IPSec VPN 기능을 추가했습니다.
* 로깅 기능 추가
    * ACL 정책별 로깅 여부를 설정할 수 있는 기능을 추가했습니다.

<a id="june-25-2024-feature-updates"></a>
### 기능 개선/변경 { #june-25-2024-feature-updates }

* 정책 스케줄 기능 개선
    * 정책 페이지에서 스케줄 사용 여부를 확인할 수 있도록 UI를 개선했습니다.
    * 스케줄을 10분 단위로 설정할 수 있도록 개선했습니다.
* 모니터 화면 개선
    * 세션 그래프에서 내/외부 세션을 구분하여 노출되도록 개선했습니다.
    * 검색 조건을 개선했습니다.

<a id="may-14-2024"></a>
## 2024. 05. 14. { #may-14-2024 }

<a id="may-14-2024-added-features"></a>
### 기능 추가 { #may-14-2024-added-features }

* NAT 수정 기능 추가
    * NAT 메인 페이지에서 '수정' 기능을 추가했습니다.

<a id="march-26-2024"></a>
## 2024. 03. 26. { #march-26-2024 }

<a id="march-26-2024-feature-updates"></a>
### 기능 추가/개선 { #march-26-2024-feature-updates }

* MTU 설정 기능 추가
    * Network Firewall에서 사용중인 인터페이스의 MTU 크기를 설정할 수 있도록 추가했습니다.   
* Syslog 포트 설정 기능 추가
    * Syslog 설정 시 포트번호를 설정할 수 있는 기능을 추가했습니다.
* UI 개선
    * 로그 항목 중 프로토콜이 숫자가 아닌 문자로 노출되도록 UI를 개선했습니다.

<a id="march-26-2024-removed-features"></a>
### 기능 삭제 { #march-26-2024-removed-features }

* NAT 설정 기능 삭제
    * 옵션에서 제공한 NAT 활성화 기능을 삭제하고 Network Firewall 생성 시 자동으로 활성화되도록 변경했습니다.

<a id="january-23-2024"></a>
## 2024. 01. 23. { #january-23-2024 }

<a id="january-23-2024-added-features"></a>
### 기능 추가 { #january-23-2024-added-features }

* 기밀 정보 암호화를 위해 SKM(secure key manager) 서비스 연동을 추가했습니다.

<a id="bug-fixes"></a>
### 버그 수정 { #bug-fixes }

* 간헐적으로 API 응답이 느린 현상을 수정했습니다.

<a id="december-19-2023"></a>
## 2023. 12. 19. { #december-19-2023 }

<a id="december-19-2023-feature-updates"></a>
### 기능 추가/개선 { #december-19-2023-feature-updates }

* 쿼터 관리 추가
    * 프로젝트별 리소스를 확인할 수 있도록 쿼터 관리 기능을 추가했습니다.
* 검색 조건 추가
    * 정책 일괄 다운로드 시 검색 조건을 추가했습니다.
* 민감 정보 처리 개선
    * CloudTrail에 적재하는 로그 중 민감 정보를 마스킹 처리할 수 있도록 개선했습니다.

<a id="october-31-2023"></a>
## 2023. 10. 31. { #october-31-2023 }

<a id="new-service-launch"></a>
### Network Firewall 신규 서비스 출시 { #new-service-launch }

Network Firewall은 NHN Cloud에서 사용하는 인프라 자산들을 안전하게 보호하기 위해 제공하는 네트워크 보안 서비스입니다.