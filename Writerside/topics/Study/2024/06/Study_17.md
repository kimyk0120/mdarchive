# aws

EC2 인스턴스 스토어 
  - 인스턴스 스토리지
    - 인스턴스 종료 시 삭제
    - EBS 볼륨 연결 시 데이터 보존

EBS (Elastic Block Store)
  - EC2 인스턴스 수명 주기가 끝나도 데이터 보존
  - EBS 볼륨
    - 다양한 크기와 유형
    - EC2인스턴스와 연결하여 사용
    - 지속적 쓰기 작업 및 백업에 용이 
    - 스냅샷 백업본 생성 가능

S3
  - Simple Storage Service
  - 데이터를 객체로 저장
  - 객체를 버킷에 저장
  - 최대 5TB의 객체 저장 가능
  - 객체의 버전 관리 
  - S3 standard
    - 99.999999999%의 내구성
    - 3개 이상 시설에 데이터 복제
  - S3 정적 웹 사이트 호스팅 
    - 정적 웹 사이트 호스팅
    - S3 버킷에 웹 사이트 파일 저장
  - S3 Standard-IA
    - 자주 액세스하지 않는 데이터 저장
    - Amazon S3 Standard와 비슷하지만 스토리지 가격은 더 저렴하고 검색 가격은 더 높음
  - S3 Glacier
    - 아카이브 데이터 저장
    - 데이터 검색 시간, 보유기간이 길어도 되는 데이터 저장
    - 저장소 잠금 정책 설정 가능
    - 수명 주기 정책 설정 가능

EBS vs S3
  - 블록 vs 객체 
    - 변경 사항이 있을 때 마다 증분 블록을 다시 쓰는 EBS
    - 객체는 변경 사항이 있을 때 전체 객체를 다시 쓰는 S3

EFS (Elastic File System)
  - Elastic File System
  - 관리형 파일 시스템 
  - 여러 인스턴스가 동시에 액세스 가능
  - 필요에 따라 확장 및 축소가 가능
  - EBS는 인스턴스에 볼륨이 열결하고 가용 영역수준의 리소스라 동일한 가용 영역에 있어야함, 볼륨이 자동으로 확장되지는 않음
  - EFS는 자동 규모 조정이 되며 여러 인스턴스 동시 읽기 및 쓰기가 가능
  - 리전 기반의 리소스
  - Amazon EBS 볼륨은 단일 가용 영역에 데이터를 저장합니다. Amazon EC2 인스턴스를 EBS 볼륨에 연결하려면 Amazon EC2 인스턴스와 EBS 볼륨 모두 동일한 가용 영역에 상주해야 합니다.
  - Amazon EFS는 리전별 서비스입니다. 이 서비스는 여러 가용 영역에 걸쳐 데이터를 저장합니다. 중복 스토리지를 사용하면 파일 시스템이 위치한 리전의 모든 가용 영역에서 동시에 데이터에 액세스할 수 있습니다. 또한 온프레미스 서버는 AWS Direct Connect를 사용하여 Amazon EFS에 액세스할 수 있습니다.

RDS (Relational Database Service)
  - 관리형 관계형 데이터베이스 서비스
  - Amazon Aurora
    PostgreSQL
    MySQL
    MariaDB
    Oracle Database
    Microsoft SQL Server

Aurora
  - MySQL, PostgreSQL과 호환되는 관리형 관계형 데이터베이스
  - 6개의 데이터 복사본을 3개의 가용 영역에 복제하고 지속적으로 Amazon S3에 데이터를 백업
  - 표준 MySQL 데이터베이스보다 최대 5배 빠르며 표준 PostgreSQL 데이터베이스보다 최대 3배

AWS RDS와 AWS Aurora의 차이점
  - RDS MySQL 과 AWS Auroral MySQL의 가장 큰 차이점은 Storage 및 관리 주체, Read Replica의 구성 방식 세가지
  - Storage : RDS MySQL은 자체 EBS로 운영하지만, Aurora MySQL은 Shared Storage를 사용한다.
    관리 주체 : RDS MySQL은 관리자가 RDS MySQL의 버전을 관리하지만, Aurora MySQL은 AWS가 개발해서 버전 업그레이드를 주기적으로 하기 떄문에 optional 또는 mandatory가 AWS에 의해 정해질 수 있다.
    Read Replica 구성 : RDS MySQL은 standby와 read replica를 만들 때 binlog를 사용하지만, Aurora의 경우 내부 storage 및 redo log 전송을 통해 빠른 통기화가 가능하며 bandwidth를 줄일 수 있다.













