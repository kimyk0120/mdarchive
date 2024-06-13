# aws

핵심가치로 종량제를 원칙으로한다
AZ availability zone

Edge location 캐시 서버들의 모임
  - 글로벌 네트워크 인프라
  - 사용자가 원하는 콘텐츠를 더 빠르게 전달할 수 있도록 도와줌

EC2
  - IaaS
  - T Tinny, M Main 등 타입종류 있음

T 타입
  - burstable performance
  - CPU 크레딧을 사용하여 CPU 사용량을 조절
  - CPU 크레딧이 없으면 CPU 사용량이 낮아짐

Lamda
  - 서버리스 컴퓨팅 서비스  
  - 사용한 만큼만 비용 지불
  - 코드 실행에 필요한 컴퓨팅 리소스만큼만 지불
  - 코드 실행 시간만큼만 비용 지불
  - 코드 실행 시간이 100ms 미만이면 100ms로 청구

S3
  - 객체 스토리지 서비스
  - 파일을 저장할 수 있는 서비스
  - REST API를 사용하여 객체를 저장하고 검색

Route 53
  - DNS 서비스

RDS
  - 관계형 데이터베이스 서비스
  - MySQL, PostgreSQL, Oracle, SQL Server 등을 지원
  - 데이터베이스를 생성, 관리, 백업, 복원, 확장할 수 있음
  
DynamoDB
  - NoSQL 데이터베이스 서비스
  - SSD 기반 무제한 스토리지
  - 자동 이중화 백업(3개 지역 분산)

ElastiCache
  - 인메모리 데이터 스토어 서비스
  - Redis, Memcached를 지원
  - 데이터베이스 쿼리를 빠르게 처리

WAF
  - 관리형 웹 방화벽 서비스
  - CloudFront, API Gateway, ALB 기본적으로 사용하도록 구성됨 

Shield
  - DDoS 공격 방어 서비스
  - Standard, Advanced 두 가지 버전이 있음
  - Standard는 무료, Advanced는 유료

KMS
  - 키 관리 서비스
  - 리스소 데이터 암호화/복호화 

CloudWatch
  - 모니터링 서비스
  - 관리형 aws 리소스 사용량, 성능, 로그, 알람 등을 모니터링
  - amazone sns 서비스를 통한 알람 가능

Amazone SNS (Simple Notification Service)
  - 관리현 메시지 서비스 

Cloudtrail
  - 관리현 이벤트 추적/감사 도구 
  - AWS 계정에 대한 이벤트 추적/감사

공동 책임모델 & 규정준수 프로그램
  - ISMS (Information Security Management System)
    - 정보보호 관리 체계
  - PCI DSS (Payment Card Industry Data Security Standard)
    - 카드 데이터 보호 표준
  - HIPAA (Health Insurance Portability and Accountability Act)
    - 건강보험 이동성 및 책임법


