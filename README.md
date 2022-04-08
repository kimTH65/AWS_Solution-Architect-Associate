# AWS

<h2>컴퓨팅</h2>  
EC2 서버
<br><br>EC2 Container Service
<br><br>ELB(Elastic Load Balancing) - L4 : 부하분산서비스(로드 밸런싱), 
<br>&emsp;외부 요청을 서버가 직접 하지않고 소프트웨어가 받아서 서버로 적절히 나누어 준다.
<br><br>Lambda - 이벤트 응답으로 코드 실행
<br><br>Auto Scaling - 서버 자동 증설

<hr>

<h2>네트워킹</h2>
VPC - 네트워크
<br><br> Route53 - DNS(도메인 네임 시스템)
<br><br> Direct Connect - 데이터 전용선

<hr>

<h2>스토리지</h2>
S3(일반) / EBS(Elastic Block Store, 빠른 블록) / Glacier(저렴) 
<br><br>CDN(CLOUD FRONT) - 콘텐츠 전송 네트워크 = 분산된 여러개의 서버/ atm기 같은 느낌

<hr>

<h2>관리 및 보안</h2>
IAM - 사용자 계정 및 그룹관리
<br><br> Cloud Watch : 모니터링 시스템
<br><br> Cloud Trail : 계정에 대한 API 호출 기록

<hr>

<h2>애플리케이션</h2>
Work Spaces - 데스크톱을 간편히 프로비저닝(사용자 요구에 맞게 자원 할당, 배치, 배포 해두고 즉시 사용 가능하게 준비) / 사용자 무제한
<br><br> Work Docs - 스토리지 및 공유 서비스 / 무료 평가판 사용자 최대 50명

<hr>

<h2>데이터베이스</h2>
RDS - 관계형 DB, Mysql, Oracle 등
<br><br> DynamoDB - NoSQL
<br><br> Redishift - DW설정, 페타규모
<br><br> ElasticCache - 캐시 클러스터

<hr>

<h2>분석</h2>
Kinesis - 데이터 수집처리, 실시간 처리
<br><br> EMR - 데이터 프로세싱
<br><br> Data Pipeline - 데이터 액세스, 변환처리

<hr>

<h2>앱 서비스</h2>
CloudSearch - 검색기능
<br><br> Simple Email Service(SES) - 트랙잭션 이메일, 마케팅 메시지 도는 다른 유형의 고품질 콘텐츠, 실시간 엑세스
<br><br> Simple Queue Service(SQS) - 메세지 손실 없이 모든 처리량 수준에서 어떤 데이터 볼륨도 전송, 1개 보증 But 추가 데이터 처리 보장 X
<br><br> Simple WorkFlow(SWF) - 클라우드 상태 추적, 작업 조정

<hr>

<h2>배포 및 관리</h2>
OpsWorks - 애플리케이션 구성과 배포 자동화
<br><br> CloudFormaiton - 리소스 템플릿 생성
<br><br> Elastic Beanstalk - 애플리케이션 자동 배포 처리
<br><br> CodeDeploy

<hr>

<h2>모바일 서비스</h2>
Simple Notification Service(SNS) - 알림을 스마트폰으로 푸시
<br><br> Cognito - 사용자 데이터 동기화 및 자격 증명
<br><br> Mobile Analytics - 모바일 분석, 보고서 / Cognito와 통합됨
<br><br> ElastiCashe - 캐시 클러스터



