# AWS

<h2>컴퓨팅</h2>  

<a href="https://github.com/kimTH65/AWS/blob/main/aws/EC2.md">EC2 서버</a>

<br>

<a href="https://github.com/kimTH65/AWS/blob/main/aws/ECS.md">ECS(EC2 Container Service) </a>

<br>

<a href="https://github.com/kimTH65/AWS/blob/main/aws/ELB.md">ELB(Elastic Load Balancing) </a> 

<br>

<a href="https://aws.amazon.com/ko/lambda/faqs/">Lambda </a>  - 이벤트 응답으로 코드 실행

<br>

<a href="https://docs.aws.amazon.com/ko_kr/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html">Auto Scaling</a> - 서버 자동 증설

<hr>

<h2>네트워킹</h2>

<a href="https://github.com/kimTH65/AWS/blob/main/aws/VPC.md">VPC</a> - 네트워크

<br>

<a href="https://aws.amazon.com/ko/route53/">Route53</a>  - DNS(Domain Name System)

<br>

<a href="https://aws.amazon.com/ko/directconnect/?nc1=h_ls">Direct Connect</a> - 데이터 전용선, 온프레미스에서 AWS로 전용 네트워크 연결을 쉽게 설정할 수 있는 클라우드 서비스 솔루션

<hr>

<h2>스토리지</h2>

<a href="https://aws.amazon.com/ko/s3/?nc1=h_ls">S3</a>(Amazon Simple Storage Service, 일반) / 
<br>
<a href="https://aws.amazon.com/ko/ebs/?nc1=h_ls">EBS</a>(Elastic Block Store, 빠른 블록) /
<br>
<a href="https://aws.amazon.com/ko/s3/storage-classes/glacier/?nc1=h_ls">Glacier</a>(저렴,데이터 아카이빙) 

<br>

<a href="https://aws.amazon.com/ko/cloudfront/">CDN(CLOUD FRONT)</a> - 콘텐츠 전송 네트워크 = 분산된 여러개의 서버/ atm기 같은 느낌 , 전세계에 53개 저장소 있음

<hr>

<h2>관리 및 보안</h2>

<a href="https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/access_policies.html">IAM</a> - 사용자 계정 및 그룹관리

<br>

<a href="https://docs.aws.amazon.com/ko_kr/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html">Cloud Watch</a> : 모니터링 시스템

<br>

<a href="https://docs.aws.amazon.com/ko_kr/awscloudtrail/latest/userguide/cloudtrail-user-guide.html">Cloud Trail</a> : 계정에 대한 API 호출 기록

<br>
<a href="https://docs.aws.amazon.com/ko_kr/network-firewall/latest/developerguide/what-is-aws-network-firewall.html">FireWall</a> : 방화벽

<hr>

<h2>애플리케이션</h2>

<a href="https://docs.aws.amazon.com/ko_kr/workspaces/?id=docs_gateway">Work Spaces</a>  - 데스크톱을 간편히 프로비저닝(사용자 요구에 맞게 자원 할당, 배치, 배포 해두고 즉시 사용 가능하게 준비) / 사용자 무제한

<br> 

<a href="https://docs.aws.amazon.com/ko_kr/workdocs/?id=docs_gateway">Work Docs</a> - 스토리지 및 공유 서비스 / 무료 평가판 사용자 최대 50명

<hr>

<h2>데이터베이스</h2>

<a href="https://docs.aws.amazon.com/ko_kr/AmazonRDS/latest/UserGuide/Welcome.html">RDS</a> - 관계형 DB, Mysql, Oracle 등

<br>

<a href="https://docs.aws.amazon.com/ko_kr/amazondynamodb/latest/developerguide/Introduction.html">DynamoDB</a> - NoSQL / SSD 사용 빠름 , Qos(Quality of Service) 자동으로 최적화

<br> 

<a href="https://docs.aws.amazon.com/ko_kr/redshift/latest/mgmt/welcome.html">Redishift</a> - DW, 페타규모

<br>

&emsp;&emsp;&emsp;&emsp;DW(데이터 웨어 하우스) = 사용자의 의사 결정에 도움줌, 기간시스템의 DB에 축척된 데이터를 공통형식으로 변환후 관리하는 DB

<br>

<a href="https://docs.aws.amazon.com/ko_kr/AmazonElastiCache/latest/red-ug/WhatIs.html">ElasticCache</a> - 캐시 클러스터

<hr>

<h2>분석</h2>

<a href="https://docs.aws.amazon.com/ko_kr/kinesis/?id=docs_gateway">Kinesis</a> - 데이터 수집처리, 실시간 처리

<br>

<a href="https://docs.aws.amazon.com/ko_kr/emr/?id=docs_gateway">Elastic Map Reduce(EMR)</a> - 데이터 프로세싱 / 호스팅 되는 하둡 프레임워크 활용.

<br>

<a href="https://docs.aws.amazon.com/ko_kr/datapipeline/latest/DeveloperGuide/what-is-datapipeline.html">Data Pipeline</a> - 데이터 액세스, 변환처리, 데이터의 이동과 변환을 자동화하는 데 사용할 수 있는 웹 서비스

<hr>

<h2>앱 서비스</h2>

<a href="https://docs.aws.amazon.com/ko_kr/cloudsearch/?id=docs_gateway">CloudSearch</a> - 검색기능

<br>

<a href="https://docs.aws.amazon.com/ko_kr/ses/latest/dg/Welcome.html">Simple Email Service(SES)</a> - 트랙잭션 이메일, 마케팅 메시지 도는 다른 유형의 고품질 콘텐츠, 실시간 엑세스

<br>

<a href="https://docs.aws.amazon.com/ko_kr/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html">Simple Queue Service(SQS)</a> - 메세지 손실 없이 모든 처리량 수준에서 어떤 데이터 볼륨도 전송, 1개 보증 But 추가 데이터 처리 보장 X, FIFO

<br>

<a href="https://docs.aws.amazon.com/ko_kr/amazonswf/latest/developerguide/swf-welcome.html">Simple WorkFlow(SWF)</a> - 클라우드 상태 추적, 작업 조정

<hr>

<h2>배포 및 관리</h2>

<a href="https://docs.aws.amazon.com/ko_kr/opsworks/latest/userguide/welcome.html">OpsWorks</a> - 애플리케이션 구성과 배포 자동화 / 애플리케이션 관리 솔루션 , Puppet/Chef 레시피 및 Bash 스크립트를 사용해 코드로 구성

<br>&emsp;&emsp;&emsp;&emsp; Chef : 오픈소스 시스템 관리 프레임워크, 서버 인프라구축 자동화

<br>&emsp;&emsp;&emsp;&emsp; Puppet : 시스템 서버관리 프레임 워크

<br>

<a href="https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/Welcome.html">CloudFormaiton</a> - 리소스 템플릿 생성 / 템플릿 및 연관된 리소스 모음(스택)을 배포 및 업데이트

<br>

<a href="https://docs.aws.amazon.com/ko_kr/elasticbeanstalk/latest/dg/Welcome.html">Elastic Beanstalk</a> - 애플리케이션 자동 배포 처리 및 규모 조정

<br>
비교 : 편리함 = 1. Elastic Beanstalk(모든 형태 자동화)&emsp;2.OpsWorks(Chef/Puppet이해 필요)&emsp;3. CloudFormaiton

<br>&emsp;&emsp;&emsp; 자유도(세세한 설정가능) = 1.CloudFormaiton&emsp;2.OpsWorks&emsp;3.Elastic Beanstalk

<br><a href="https://docs.aws.amazon.com/ko_kr/codedeploy/latest/userguide/welcome.html">CodeDeploy</a> - EC2인스턴스, 오프레미스 인스턴스, 서버리스 Lambda 함수 등의 서비스로 애플리케이션 배포를 자동화하는 서비스

<hr>

<h2>모바일 서비스</h2>

<a href="https://docs.aws.amazon.com/ko_kr/sns/latest/dg/welcome.html">Simple Notification Service(SNS)</a> - 알림을 스마트폰으로 푸시

<br>

<a href="https://docs.aws.amazon.com/ko_kr/cognito/latest/developerguide/cognito-user-identity-pools.html">Cognito</a> - 사용자 데이터 동기화 및 자격 증명

<br>

Mobile Analytics - 모바일 분석, 보고서 / Cognito와 통합됨

<hr>

<h2>용어</h2>

<br>Amazon FSx : Windows Server에 구축되는 완전관리형 파일 스토리지,SMB 프로토콜 기반

<br>EFS(Elastic FIle System) : EC2용 관리형 파일 스토리지, NFS/NAS와 동일한 서비스 , NFS 프로토콜 기반

<br>ECR(Elastic Container Registry) : AWS 관리형 컨테이너 이미지 레지스트리 서비스

<br>Aurora : MySQL 및 PostgreSQL과 호환되는 완전 관리형 관계형 데이터베이스 엔진

<br>AZ(Availability Zone/가용 영역) : 클라우드 서비스를 사용할 수 있는 국가(지역)

<br>IOPS(Input/Output Operation Per Second) : 초당 입출력 속도

<br>IOPS SSD : 주요 성능 특성이 iops인 ssd

<br>ISCSI(Internet Small Computer System Interface) : 컴퓨터 환경에서 데이터 스토리지 시설을 이어주는 IP기반의 스토리지 네트워킹 표준
<br>IP망을 통해 SCSI 명령을 전달함으로서 인트라넷을 거쳐 데이터 전송을 쉽게하고 먼 거리에 걸쳐 스토리지를 관리하는데 쓰인다.

<br>이더넷(LAN에서 사용) - 인터넷 - 인트라넷(인터넷과 비슷하지만 폐쇠적)

<br>버킷(Bucket) : S3에서 생성할 수 있는 최상위 디렉토리의 개념, 이름은 S3 리전 중에서 유일해야함. 

<br>정적 콘텐츠(누가 언제 서버에 요청하더라도 같은 내용을 보여줌) / 동적 콘텐츠(누가,언제,어떻게 서버에 요청 하냐에 따라 다른 내용을 보여줌) 

<br>File Server란 : OS에 따라 Windows 파일서버, Unix 파일서버, Linux 파일서버가 있음
<br>&emsp;&emsp;&emsp;&emsp; Windows 파일서버는 CIFS(Common Internet File System)을 사용해서 클라이언트에 스토리지 공유
<br>&emsp;&emsp;&emsp;&emsp; Unix나 Linux는 NFS(Network File System)을 사용

<br>SnowMobile : 초대용량 데이터를 AWS로 이전하는 데 사용하는 엑사바이트 규모의 데이터 전송 서비스. 최대 100PB

<br>Snowball : 데이터 마이그레이션 및 엣지 컴퓨팅 디바이스, S3와 호환되는 객체 스토리지 제공
<br>&emsp;&emsp;&emsp;&emsp; Snowball Edge Storage Optimized - TB～PB사이즈의 데이터를 AWS로 빠르고 안전하게 전송할 떄
<br>&emsp;&emsp;&emsp;&emsp; Snowball Edge -> S3 -> Glacier(수명주기 정책)패턴으로 많이 사용

<br>Snowball Edge : 선택 가능한 온보드 스토리지와 컴퓨팅 파워를 갖춘 Snowball 디바이스의 한 유형

<br>SFA(Sales Force Automation) : 영업 자동화

<br>Snapshot(스냅샷) : 사진 찍듯이 특정 시점에 스토리지의 파일 시스템을 포착해 보관하는 기술을 의미

<br>인스턴스 스토어 : 인스턴스에 블록 수준의 임시 스토리지를 제공

<br>PostgreSQL : 오픈 소스 객체-관계형 데이터베이스 시스템(ORDBMS), 함수/연산자 등 다양한 데이터베이스 객체 커스텀 가능

<br>OLTP(OnLine Transaction Processing) : 온라인 트랜잭션 처리, 네트워크 상의 온라인 사용자들의 Database에 대한 일괄 트랜잭션 처리

<br>&emsp;&emsp;&emsp;&emsp;트랜잭션 : 데이터베이스의 상태를 변화시키기 위해 수행하는 작업의 단위

<br>OLAP(OnLine Analytical Processing) : 데이터 웨어하우스 등의 시스템과 연관되어 Data를 분석, 정보를 분석/모델링 하게 하는 분석 방법

<br>NS(Name Server) : 도메인에 대한 정보(A레코드, MX레코드 등)을 가지고 있는 서버

<br>WAF : 콘텐츠에 대한 액세스를 제어할 수 있도록 CloudFront로 전송되는 HTTP 및 HTTPS 요청을 모니터링하는 웹 애플리케이션 방화벽

<br>EKS(Elastic Kubernetes Service) : 쿠버네티스(도커랑 비슷)를 쉽게 실행할 수 있도록 하는 관리형 서비스

<br>SMS(Server Migration Service) : VMware,Azure등의 가상 머신을 AWS 클라우드로 마이그레션하는 것을 자동화

<br>STS(Security Token Service) : AWS리소스에 대한 액세스를 제어할 수 있는 임시 보안 자격 증명을 생성

<br>RAID(Redundunt Array of Independent Disk) : 2개이상의 디스크를 병렬로 처리하여 성능 및 안정성을 향상시킴, 디스크 오류나 데이터 손실등 장애 대응을 위한 용도로도 사용할 수 있다.

<br>&emsp;&emsp;&emsp;&emsp; RAID-0 : 두 개 이상의 디스크에 데이터를 순차적으로 저장하는 방식, 
<br>&emsp;&emsp;&emsp;&emsp; 하나의 디스크에 문제가 생기면 모든데이터 유실, 오직 성능향상을 위한 방식

<br>&emsp;&emsp;&emsp;&emsp; RAID-1 : 데이터 처리 시, 동일한 디스크에 똑같이 저장하는 방식, 복구/안정성 높음, 용량 반으로 줄어듬

<br>&emsp;&emsp;&emsp;&emsp; RAID-3,4 :0과 같이 분산처리방식 + 에러 체크 및 수정을 위한 패리티(parity)정보를 별도 디스크에 저장

<br>&emsp;&emsp;&emsp;&emsp; RAID-5 : 분산 에러처리 / RAID-6 : 패리티, 최소 4개 이상의 하드 2개 까지 커버 

<br>&emsp;&emsp;&emsp;&emsp; RAID-10 : 우선 미러링 그후 스트리핑, 디스크 4개중 2개씩 미러링/스터리핑

<br>PV(반가상화) AMI(Amazon Machine Image)

<br>SAML(Security Assertion Markup Language) 페더레이션(신뢰가 설정된 도메인의 컬렉션)

<br>192.168.0.1 -> A레코드 -> dev.blog.co.kr -> CNAME ->dev.plusblog.co.kr 

<br>고객 제공 암호화 키(SSE-C)
