# AWS

<h2>컴퓨팅</h2>  
<a href="https://github.com/kimTH65/AWS/blob/main/aws/EC2.md">EC2 서버</a>
<br><br><a href="https://github.com/kimTH65/AWS/blob/main/aws/ECS.md">EC2 Container Service </a>
<br><br><a href="https://github.com/kimTH65/AWS/blob/main/aws/ELB.md">ELB(Elastic Load Balancing) </a> 
<br><br><a href="https://aws.amazon.com/ko/lambda/faqs/">Lambda </a>  - 이벤트 응답으로 코드 실행
<br><br><a href="https://docs.aws.amazon.com/ko_kr/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html">Auto Scaling</a> - 서버 자동 증설
<hr>

<h2>네트워킹</h2>
<a href="https://github.com/kimTH65/AWS/blob/main/aws/VPC.md">VPC</a> - 네트워크
<br><br> Route53 - DNS(Domain Name System)
<br><br> Direct Connect - 데이터 전용선, 온프레미스에서 AWS로 전용 네트워크 연결을 쉽게 설정할 수 있는 클라우드 서비스 솔루션

<hr>

<h2>스토리지</h2>
S3(일반) / EBS(Elastic Block Store, 빠른 블록) / Glacier(저렴) 
<br><br>CDN(CLOUD FRONT) - 콘텐츠 전송 네트워크 = 분산된 여러개의 서버/ atm기 같은 느낌 , 전세계에 53개 저장소 있음

<hr>

<h2>관리 및 보안</h2>
IAM - 사용자 계정 및 그룹관리
<br><br> Cloud Watch : 모니터링 시스템
<br><br> Cloud Trail : 계정에 대한 API 호출 기록
<br><br> FireWall : 방화벽

<hr>

<h2>애플리케이션</h2>
Work Spaces - 데스크톱을 간편히 프로비저닝(사용자 요구에 맞게 자원 할당, 배치, 배포 해두고 즉시 사용 가능하게 준비) / 사용자 무제한
<br><br> Work Docs - 스토리지 및 공유 서비스 / 무료 평가판 사용자 최대 50명

<hr>

<h2>데이터베이스</h2>
RDS - 관계형 DB, Mysql, Oracle 등
<br><br> DynamoDB - NoSQL / SSD 사용 빠름 , Qos(Quality of Service) 자동으로 최적화
<br><br> Redishift - DW, 페타규모
<br>&emsp;DW(데이터 웨어 하우스) = 사용자의 의사 결정에 도움줌, 기간시스템의 DB에 축척된 데이터를 공통형식으로 변환후 관리하는 DB
<br><br> ElasticCache - 캐시 클러스터

<hr>

<h2>분석</h2>
Kinesis - 데이터 수집처리, 실시간 처리
<br><br> Elastic Map Reduce(EMR) - 데이터 프로세싱 / 호스팅 되는 하둡 프레임워크 활용.
<br><br> Data Pipeline - 데이터 액세스, 변환처리

<hr>

<h2>앱 서비스</h2>
CloudSearch - 검색기능
<br><br> Simple Email Service(SES) - 트랙잭션 이메일, 마케팅 메시지 도는 다른 유형의 고품질 콘텐츠, 실시간 엑세스
<br><br> Simple Queue Service(SQS) - 메세지 손실 없이 모든 처리량 수준에서 어떤 데이터 볼륨도 전송, 1개 보증 But 추가 데이터 처리 보장 X
<br><br> Simple WorkFlow(SWF) - 클라우드 상태 추적, 작업 조정

<hr>

<h2>배포 및 관리</h2>
OpsWorks - 애플리케이션 구성과 배포 자동화 / 애플리케이션 관리 솔루션 , Chef 레시피 및 Bash 스크립트를 사용해 코드로 구성
<br><br> CloudFormaiton - 리소스 템플릿 생성 / 템플릿 및 연관된 리소스 모음(스택)을 배포 및 업데이트
<br><br> Elastic Beanstalk - 애플리케이션 자동 배포 처리 및 규모 조정
<br><br> CodeDeploy

<hr>

<h2>모바일 서비스</h2>
Simple Notification Service(SNS) - 알림을 스마트폰으로 푸시
<br><br> Cognito - 사용자 데이터 동기화 및 자격 증명
<br><br> Mobile Analytics - 모바일 분석, 보고서 / Cognito와 통합됨
<br><br> ElastiCashe - 캐시 클러스터



