# Load Balancer Manager

OpenStack Octavia 기반 로드밸런서 운영 및 장애 처리를 위한 TUI 관리 도구입니다.

## 배경

OpenStack Octavia 운영 중 API로 삭제되지 않는 비정상 LB가 발생하는 경우,
수동으로 상태를 파악하고 DB에서 직접 처리해야 하는 번거로움이 있었습니다.
현황 파악, 장애 처리 명령 생성, 로그 조회를 하나의 TUI 도구로 통합했습니다.

## 주요 기능
LB 구성 트리 조회 — LB → Listener → Pool → Member 계층 구조 한눈에 확인
Amphora 상태 조회 및 Failover 명령
비정상 LB 삭제 SQL 자동 생성 — LB ID 입력 시 Octavia DB 직접 삭제용 SQL 생성
Octavia 서비스 상태 확인 및 재시작 명령 제공


## 환경
인프라: OpenStack (Octavia)
언어: Go (단일 바이너리 빌드, 의존성 없이 배포 가능)


## 사용법

./loadbalancer-manager

OpenStack 연동 기능은 ~/contrabass-openrc 또는
LB_MANAGER_OPENSTACK_OPENRC 환경변수로 openrc 경로를 지정하세요.
