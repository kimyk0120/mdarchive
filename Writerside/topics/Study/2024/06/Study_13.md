# aws

Amazone SQS (Simple Queue Service)
  - 메시지 대기열 서비스

Amazone SNS (Simple Notification Service)
  - 메시지 발행 및 구독 서비스

Lambda
  - 서버리스 컴퓨팅 서비스
  - 코드를 실행하고 서버 관리를 자동화
  - 15분 이하의 작업에 적합
  - 웹서비스 백엔드 등의 빠른 처리에 적합
  - 이벤트 기반의 서비스에 적합
  - 서버를 프로비저닝 또는 관리 X

ECS or EKS
  - 컨테이너 관리 서비스
  - ECS : Docker 컨테이너를 실행하는 서비스
  - EKS : Kubernetes를 실행하는 관리 서비스

Fargate
  - 컨테이너용 서버리스 컴퓨팅 서비스
  - 컨테이너를 실행하는 서버를 관리하는 서비스

리전(Region) 선택 핵심  
  - 규정준수
  - 근접성
  - 기능 사용성 
  - 가격

AZ (Availability Zone)
  - 데이터 센터의 물리적인 위치
  - 하나의 리전에 여러개의 AZ가 존재
  - 하나의 AZ가 다운되어도 다른 AZ는 정상적으로 작동

엣지 로케이션 (Edge Location)
  - CDN 서비스를 제공하는 데이터 센터
  - CloudFront 서비스를 이용하여 전 세계에 캐시 서버를 두고 사용자에게 빠른 서비스 제공














