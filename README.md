# loadbalancer-manager
OpenStack Octavia 기반 로드밸런서 운영 및 장애 처리를 위한 TUI 관리 도구


LB / Listener / Pool / HealthMonitor 목록 조회
Octavia 서비스 상태/재시작 명령 제공
비정상 LB 삭제 SQL 자동 생성
LB ID 입력 → 삭제 SQL 생성
로그 조회 명령 제공
Amphora 상태 조회
LB 구성 트리 출력 (LB → Listener → Pool → Member 계층)
L7 Policy 목록 조회
Amphora failover 명령
실시간 로그 스트리밍 (tail -f 결과 TUI에서 보기)
