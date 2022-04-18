# AWS

<h2>컴퓨팅</h2>  

<a href="https://github.com/kimTH65/AWS/blob/main/aws/EC2.md">EC2 서버</a>

<br>

<a href="https://github.com/kimTH65/AWS/blob/main/aws/ECS.md">EC2 Container Service </a>

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

<a href="https://docs.aws.amazon.com/ko_kr/codedeploy/latest/userguide/welcome.html">CodeDeploy</a> - EC2인스턴스, 오프레미스 인스턴스, 서버리스 Lambda 함수 등의 서비스로 애플리케이션 배포를 자동화하는 서비스

<hr>

<h2>모바일 서비스</h2>

Simple Notification Service(SNS) - 알림을 스마트폰으로 푸시

<br>

Cognito - 사용자 데이터 동기화 및 자격 증명

<br>

Mobile Analytics - 모바일 분석, 보고서 / Cognito와 통합됨

<hr>

<h2>용어</h2>

