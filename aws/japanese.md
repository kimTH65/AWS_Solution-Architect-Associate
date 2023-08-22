# AWS
<h5>　
<a href="https://github.com/kimTH65/AWS/blob/main/README.md">한국어</a> 
&emsp;
<a href="https://github.com/kimTH65/AWS/blob/main/aws/japanese.md">日本語</a> 
</h5>
<h2>コンピューティング(Computing)</h2>   


<a href="https://github.com/kimTH65/AWS/blob/main/aws/EC2.md">EC2(Elastic Compute Cloud)</a> : クラウドコンピューティングサービス


<br>  

<a href="https://aws.amazon.com/ko/lambda/faqs/">Lambda </a> : サーバーをプロビジョニングしたり管理したりする必要がないサーバーレスコンピューティングサービス

<br>

<a href="https://docs.aws.amazon.com/ko_kr/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html">Auto Scaling</a> : サーバー自動増設

<br> 
 
SAM(Serverless Application Model) : サーバレスアプリケーションをビルドするための配布ツール

<hr>

 
<!--                                        ----------------------------------------------------------                                      -->


<h2>コンテナ(Container)</h2>  

<a href="https://github.com/kimTH65/AWS/blob/main/aws/ECS.md">ECS(EC2 Container Service)</a> : Dockerコンテナ管理サービス

<br>

ECR(Elastic Container Registry) : Dockerコンテナイメージを保存するRepositoryサービス 

<br>

EKS(Elastic Kubernetes Service) : Kubernetesを簡単に実行できる管理型サービス

<h6>
&emsp;&emsp;&emsp;&emsp;  Kubernetes : 複数のコンテナ(Docker)を管理するサービス
</h6>

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>ネットワーキング(Networking)</h2>

<a href="https://github.com/kimTH65/AWS/blob/main/aws/ELB.md">ELB(Elastic Load Balancing) </a> 

<br>

<a href="https://github.com/kimTH65/AWS/blob/main/aws/VPC.md">VPC(Virtual Private Cloud)</a>

<br>

<a href="https://aws.amazon.com/ko/route53/">Route53</a> - DNS(Domain Name System)

<h6>
&emsp;&emsp;&emsp;&emsp;  Latency Based Routing : 現在位置で遅延時間(Latency)が最も低いリージョンのIPアドレスを知らせる
<br><br>
&emsp;&emsp;&emsp;&emsp;  Weighted Round Robin : サーバーIPアドレスまたはドメイン(ELB)ごとに加重値を付与するトラフィックを調節する機能
<br><br>
&emsp;&emsp;&emsp;&emsp;  DNS Failover : 障害が発生したサーバのIP アドレスまたは、 ドメイン(ELB)を知らせない機能
<br><br>
&emsp;&emsp;&emsp;&emsp;  Geo Routing : 地域別に異なるIPアドレスを教える
</h6>

<br>

<a href="https://docs.aws.amazon.com/ko_kr/vpn/latest/s2svpn/VPC_VPN.html">VPN</a> : ネットワークとネットワーク間のセキュリティ接続を設定するサービス
<h6>
&emsp;&emsp;&emsp;&emsp;Site-to-Site VPN : Clasic VPN、AWS VPC環境とオンプレミス環境のVPN接続
<br><br>  
&emsp;&emsp;&emsp;&emsp;Clinet VPN : 個人がAWSサービスやオンプレミス環境に接続できるようにするサービス 
</h6>
  
<br>

<a href="https://aws.amazon.com/ko/cloudfront/">CDN(Cloud Front)</a> : コンテンツ配信ネットワーク=分散した複数のサーバ/atm機のような感じ、全世界に53のストレージあり

<br>

<a href="https://aws.amazon.com/ko/directconnect/?nc1=h_ls">Direct Connect</a> :データ専用線、AWS環境とオンプレミス環境との接続のためのサービスソリューション

<br>

Global Accelerator : AWSのグローバルネットワークインフラを通じてユーザートラフィックを送信し、パフォーマンスを向上させるネットワーキングサービス

<br>

API Gateway : APIを作成/運営/モニタリング(Cloud Watch)およびセキュリティを維持できるサービス、Lambdaと一緒にRESTApiを生成可能

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>ストレージ(Storage)</h2>

<h3>ストレージの種類</h3>

<a href="https://aws.amazon.com/ko/s3/?nc1=h_ls">S3</a>(Amazon Simple Storage Service, 一般)

<h6>&emsp;&emsp;&emsp;&emsp;バケット(Bucket) : 3 で生成できる最上位ディレクトリの概念、名前はS3 リージョンの中で唯一でなければならない </h6>

<h6>&emsp;&emsp;&emsp;&emsp;S3-CORS(Cross-Origin Resource Sharing) : 複数のドメインからアプリケーションのS3バケットへのコンテンツアクセスを許可するために使用されるメカニズム</h6>

<a href="https://aws.amazon.com/ko/s3/storage-classes/glacier/?nc1=h_ls">S3 - Glacier</a>(安価、データアーカイブ) 

<h6>&emsp;&emsp;&emsp;&emsp;Glacier vault lock : ボルトロックポリシーを使用してGlacierの各資格証明集について規定管理が可能。ロック可能</h6>
                             
<div align="center">
<br><h4>S3 ライフサイクル</h4> 
<img src="https://user-images.githubusercontent.com/59690816/167321873-67dc89e2-6c9b-4e9b-b69d-fdb8e7b3efe8.png" width="500" height="350">

<h6>出処 : https://docs.aws.amazon.com/ko_kr/AmazonS3/latest/userguide/lifecycle-transition-general-considerations.html</h6>
</div><br>
<a href="https://aws.amazon.com/ko/ebs/?nc1=h_ls">EBS</a>(Elastic Block Store, 速いブロック) 

<h6>&emsp;&emsp;&emsp;&emsp;DLM(Data Lifecycle Manager) : EBSスナップショット及び削除予約可能</h6>

<br>

<a href="https://docs.aws.amazon.com/ko_kr/fsx/?id=docs_gateway">Amazon FSx</a> : Windows Serverに構築される完全管理型ファイルストレージ、SMBプロトコルベース

<br> 

<a href="https://docs.aws.amazon.com/ko_kr/efs/latest/ug/whatisefs.html">EFS(Elastic File System)</a> : Linux Server、EC2用管理型ファイルストレージ、NFS/NASと同様のサービス、NFSプロトコルベース

<br>

EC2 Instance Store : ブロックレベルの一時ストレージ、ホスト コンピューターに物理的に接続されたディスク

<br>

Snow Family : オフラインデータ転送デバイス , Snowcone - Snowball/Snowball Edge - Snowmobile(100PB)

<h6>
&emsp;&emsp;&emsp;&emsp;Snowball : データ移行およびエッジコンピューティングデバイス、S3と互換性のあるオブジェクトストレージを提供

<br>&emsp;&emsp;&emsp;&emsp;Snowball Edge Storage Optimized - TB~PBサイズのデータをAWSに素早く安全に転送する際

&emsp;&emsp;&emsp;&emsp;Snowball Edge -> S3 -> Glacier(ライフサイクルポリシー)パターンとしてよく使用
  
<br>
  
</h6>

<h3>その他の機能</h3>

<br>

 Snapshot(スナップショット) : 写真を撮るように特定時点でストレージのファイルシステムを捕捉して保管する技術を意味する

<br>

AWS DataSync : ネットワーク帯域幅を最適化し、オンプレミス-AWSストレージ間のデータ移動を加速するオンライン配信サービス

<br>

AWS Storage Gateway : オンプレミスからほぼ無制限のストレージにアクセスできるハイブリッドクラウドストレージサービス

<br>

AWS Transfer Family : SFTP、FTPSおよびFTPプロトコルを使用してS3/EFSに簡単かつ円滑にファイルを転送

<h6>
&emsp;&emsp;&emsp;&emsp;Transfer Acceleration : SFTP、FTPSおよびFTPプロトコルを使用してS3/EFSに簡単かつ円滑にファイルを転送
</h6>

<br>

AWS Multipart Upload : 大型オブジェクトを分けてアップロード、既存オブジェクトのコピー

<br>

AWS Elastic Disaster Recovery(DRS) : 安価なストレージ、最小限のコンピューティング/特定の視点復旧で迅速かつ安定的にデータ復旧

<h6>
&emsp;&emsp;&emsp;&emsp;DR(Disaster Recovery) : 災害復旧、災害/危険によりシステムが中断されたときに、それを正常な状態に復旧すること
</h6>

<br>

AWS Backup : アプリケーションのデータ保護、コンプライアンス、ガバナンスを中央管理/自動化する完全管理型ポリシーベースのサービス

<br>

Cross Region Replication(CRR) : 異なるAWSリージョンのS3バケットからオブジェクトコピー

<br>

Simple Region Replication(SRR) : 同一リージョンのS3バケットからオブジェクトコピーに使用

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>管理およびセキュリティ</h2>

<a href="https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/access_policies.html">IAM</a> - ユーザーアカウントとグループ管理

<h6>
&emsp;&emsp;&emsp;&emsp;<a href="https://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/access_policies.html">IAMセキュリティベストプラクティス</a>:ルートユーザ使用アクセスキーロック、役割を使用して権限委任、最小権限付与など
</h6>

<br>

<a href="https://docs.aws.amazon.com/ko_kr/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html">Cloud Watch</a> : AWSサービス観察·モニタリングシステム
<br>

<a href="https://docs.aws.amazon.com/ko_kr/awscloudtrail/latest/userguide/cloudtrail-user-guide.html">Cloud Trail</a> : ユーザー観察、アカウントに対するAPI呼び出し記録

<br>

<a href="https://docs.aws.amazon.com/ko_kr/network-firewall/latest/developerguide/what-is-aws-network-firewall.html">FireWall</a> : ファイア・ウォール

<br>

<a href="https://docs.aws.amazon.com/ko_kr/cognito/latest/developerguide/cognito-user-identity-pools.html">Cognito</a> - ユーザーデータの同期と資格証明
<br>

AWS Organizations : 複数のAWSアカウントを組織に統合し、中央で管理できるアカウント、各アカウントのストレージ使用量を統合してS3コスト削減が可能

<br>

WAF : コンテンツへのアクセスを制御できるよう、CloudFrontに送信されるHTTPおよびHTTPS要求を監視するWebアプリケーションファイアウォール、SQL注入またはサイト間スクリプティング(XXS)のような一般的な攻撃パターンをブロックセキュリティルール定義可能

<h6>&emsp;&emsp;&emsp;&emsp;XXS(交差サイトスクリプティング) : 脆弱な動的ウェブページにコードを追加/掲示し、他のユーザーのPCにマルウェアを実行させる攻撃</h6>

<br>

MFA(Multi-Factor Authentication) : 2段階認証/OTPのようなもの、CognitoユーザープールにMFAを追加して使用する

<br>

AWS Shield : DDoS探知·緩和·対応機能でセキュリティ状態を改善する管理型脅威防止サービス

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>애플리케이션</h2>

<a href="https://docs.aws.amazon.com/ko_kr/workspaces/?id=docs_gateway">Work Spaces</a>  - 데스크톱을 간편히 프로비저닝 / 사용자 무제한

<h6>&emsp;&emsp;&emsp;&emsp;프로비저닝 : 사용자 요구에 맞게 자원 할당, 배치, 배포 해두고 즉시 사용 가능하게 준비 </h6>

  
<br> 

<a href="https://docs.aws.amazon.com/ko_kr/workdocs/?id=docs_gateway">Work Docs</a> - 스토리지 및 공유 서비스 / 무료 평가판 사용자 최대 50명

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>데이터베이스</h2>
<h3>관계형 데이터베이스</h3>

<a href="https://docs.aws.amazon.com/ko_kr/AmazonRDS/latest/UserGuide/Welcome.html">RDS</a> - 관계형 DB, Mysql, Oracle 등

<br> 

<a href="https://docs.aws.amazon.com/ko_kr/redshift/latest/mgmt/welcome.html">Redshift</a> - DW로 빠르게 데이터 쿼리, 페타규모

<h6>&emsp;&emsp;&emsp;&emsp;DW(데이터 웨어 하우스) = 사용자의 의사 결정에 도움줌, 기간시스템의 DB에 축척된 데이터를 공통형식으로 변환후 관리하는 DB</h6>

<br>

Aurora : MySQL 및 PostgreSQL과 호환되는 완전 관리형 관계형 데이터베이스 엔진

<br>

<h3>키-값(NoSQL)</h3>

<a href="https://docs.aws.amazon.com/ko_kr/amazondynamodb/latest/developerguide/Introduction.html">DynamoDB</a> - NoSQL / SSD 사용 빠름 , Qos(Quality of Service) 자동으로 최적화

<h6>&emsp;&emsp;&emsp;&emsp;TTL(Time to Live) = 아이템별 타임스탬프를 정의하여 아이템이 더 이상 필요하지 않는 시기를 결정</h6>

<br>

<h3>인 메모리</h3>

<a href="https://docs.aws.amazon.com/ko_kr/AmazonElastiCache/latest/red-ug/WhatIs.html">ElastiCache</a> - 캐시 클러스터, 두가지 메모리 엔진 지원(Redis/Memcached)

<h6>
&emsp;&emsp;&emsp;&emsp;ElastiCache for Redis : 백업, 소프트웨어 패치, 자동 장애 및 복구를 관리,자동 스냅샷/수동 고유한 백업 스냅샷 생성 후 이용해 클러스터 복원  
<br><br>
&emsp;&emsp;&emsp;&emsp;ElastiCache for Memcached : 인 메모리 키-값 스토어 서비스, 확장 가능, 완전관리형 서비스
</h6>

<br>

<h3>기타</h3>

PostgreSQL : 오픈 소스 객체-관계형 데이터베이스 시스템(ORDBMS), 함수/연산자 등 다양한 데이터베이스 객체 커스텀 가능

<br>

Amazon Neptune : 그래프 유형, IoT 애플리케이션, DevOps, 산업용 텔레메트리

<br>

Amazon DocumentDB : 문서 유형, 콘텐츠 관리, 카탈로그, 사용자 프로필, MongoDB호환

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>분석</h2>

<a href="https://docs.aws.amazon.com/ko_kr/kinesis/?id=docs_gateway">Kinesis</a> - 데이터 수집처리, 실시간 처리
<h6>

&emsp;&emsp;&emsp;&emsp;Kinesis Data Streams : 실시간 데이터 스트림을 캡처/처리/저장/분석해주는 서비스
<br><br>
&emsp;&emsp;&emsp;&emsp;Kinesis Data Analytics : Apache Flink를 사용하여 실시간으로 스트리밍 데이터를 변환하고 분석
<br>  
&emsp;&emsp;&emsp;&emsp;Kinesis Data Firehose : 데이터 스트림 처리/전송
  
</h6>
<br>

<a href="https://docs.aws.amazon.com/ko_kr/emr/?id=docs_gateway">Elastic Map Reduce(EMR)</a> - 데이터 프로세싱 / 호스팅 되는 하둡 프레임워크 활용.

<br>

<a href="https://docs.aws.amazon.com/ko_kr/datapipeline/latest/DeveloperGuide/what-is-datapipeline.html">Data Pipeline</a> - 데이터 액세스, 변환처리, 데이터의 이동과 변환을 자동화하는 데 사용할 수 있는 웹 서비스

<br>

Athena : S3에 저장된 데이터에 쿼리를 날려 간편하게 데이터를 분석할 수 있는 SQL 쿼리 서비스

<br>

QuickSight : 클라우드 기반 BI(Business Intelligence) 도구를 제공하는 시각화 도구 

<br>

<a href="https://docs.aws.amazon.com/ko_kr/cloudsearch/?id=docs_gateway">CloudSearch</a> - 완전 관리형 서비스, 웹 사이트/애플리케이션을 위한 검색 솔루션을 쉽게 설치, 관리 및 확장

<br>

AppFlow : 코드 없이 SaaS 애플리케이션과 AWS 서비스 사이에서 안전하게 데이터를 전송할 수 있는 통합 서비스

<h6>
&emsp;&emsp;&emsp;&emsp;SaaS(Software as a Service) : 서비스형 소프트웨어, 클라우드 서비스로 제공되는 소프트웨어   
</h6>
  

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>앱 서비스</h2>

<a href="https://docs.aws.amazon.com/ko_kr/ses/latest/dg/Welcome.html">Simple Email Service(SES)</a> - 트랙잭션 이메일, 마케팅 메시지 도는 다른 유형의 고품질 콘텐츠, 실시간 엑세스

<br>

<a href="https://docs.aws.amazon.com/ko_kr/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html">Simple Queue Service(SQS)</a> - 메세지 손실 없이 모든 처리량 수준에서 어떤 데이터 볼륨도 전송, 1개 보증 But 추가 데이터 처리 보장 X, FIFO

<br>

<a href="https://docs.aws.amazon.com/ko_kr/amazonswf/latest/developerguide/swf-welcome.html">Simple WorkFlow(SWF)</a> - 클라우드 상태 추적, 작업 조정

<br>

<a href="https://docs.aws.amazon.com/ko_kr/amazon-mq/?id=docs_gateway">MQ(Message Queue)</a> : 관리형 메시지 브로커 서비스

<h6>&emsp;&emsp;&emsp;&emsp;메시지 브로커(message broker) :시스템 및 서비스가 서로 간에 통신하고 정보를 교환할 수 있도록 해주는 소프트웨어 </h6>

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>배포 및 관리</h2>

<a href="https://docs.aws.amazon.com/ko_kr/opsworks/latest/userguide/welcome.html">OpsWorks</a> - 애플리케이션 구성과 배포 자동화 / 애플리케이션 관리 솔루션 , Puppet/Chef 레시피 및 Bash 스크립트를 사용해 코드로 구성

<h6>
&emsp;&emsp;&emsp;&emsp; Chef : 오픈소스 시스템 관리 프레임워크, 서버 인프라구축 자동화
<br><br>
&emsp;&emsp;&emsp;&emsp; Puppet : 시스템 서버관리 프레임 워크
</h6>

<br>

<a href="https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/Welcome.html">CloudFormaiton</a> - 리소스 템플릿 생성 / 템플릿 및 연관된 리소스 모음(스택)을 배포 및 업데이트

<br>

<a href="https://docs.aws.amazon.com/ko_kr/elasticbeanstalk/latest/dg/Welcome.html">Elastic Beanstalk</a> - 애플리케이션 자동 배포 처리 및 규모 조정

<br>

<div align="center">
<h3>비교</h3>
<h6>
편리함 = 1. Elastic Beanstalk(모든 형태 자동화)&emsp;2.OpsWorks(Chef/Puppet이해 필요)&emsp;3. CloudFormaiton
<br><br>
자유도(세세한 설정가능) = 1.CloudFormaiton&emsp;2.OpsWorks&emsp;3.Elastic Beanstalk
</h6>
</div>
<br>

<h3>개발자 도구</h3>

<a href="https://docs.aws.amazon.com/ko_kr/codedeploy/latest/userguide/welcome.html">CodeDeploy</a> - EC2인스턴스, 온프레미스 인스턴스, 서버리스 Lambda 함수 등의 서비스로 애플리케이션 배포를 자동화하는 서비스

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>모바일 서비스</h2>

<a href="https://docs.aws.amazon.com/ko_kr/sns/latest/dg/welcome.html">Simple Notification Service(SNS)</a> - 알림을 스마트폰으로 푸시

<br>

Mobile Analytics - 모바일 분석, 보고서 / Cognito와 통합됨

<br>

AppSync : DynamoDB,Lambda 등 연결 후 GraphQL(쿼리 언어) API 개발을 용이하게 하는 완전관리형 서비스

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>용어 및 기타 </h2>

<h3>클라우드 컴퓨팅 모델</h3>

<br>IaaS : 서비스로서의 인프라, 클라우드 IT의 기본 구성요소

<br>PaaS : 서비스로서의 플랫폼, 기본 인프라 관리할 필요 없음, 애플리케이션 배포 및 관리에 집중

<br>SaaS : 서비스로서의 소프트웨어, 서비스 공급자가 운영하고 관리하는 완제품 제공

<br><h3>암호화 및 PKI(Public Key Infrastructure)</h3>

<br>SSE-S3 : Amazon S3 관리형 키를 사용한 서버측 암호화, 가장 강력한 블록 암호(AES-256)사용하여 데이터 암호화

<br>SSE-KMS : AWS Key Management Service에 저장된 KMS키를 사용한 서버 측 암호화

<br>SSE-C : 고객 제공 키를 사용한 서버 측 암호화, 사용자가 암호화 키 관리

<br>ACM(AWS Certificate Manager) : AWS 인증서 관리자

<br>Cloud HSM : 관리형 하드웨어 보안 모듈로 암호화된 키 스토리지 제공

<br><h3>Migration</h3>

<br>AWS SMS(Server Migration Service) : VMware,Azure등의 가상 머신을 AWS 클라우드로 마이그레션하는 것을 자동화

<br>AWS MGN(Application Migration Service) : Lift and Shift 마이그레이션에 권장되는 기본 마이그레이션 서비스

<h6>&emsp;&emsp;&emsp;&emsp;Lift and Shift : 애플리케이션을 클라우드로 마이그레이션 하는 방식 중 하나</h6>

<br>AWS DMS(Database Migration Service) : DB,DW 등을 쉽게 마이그레이션할 수 있는 클라우드 서비스

<br>AWS ADS(Application Discovery Service) : 서버 사양 정보, 하드웨어 구성, 성능,실행 프로세스,네트워크 연결 정보등 수집하여 데이터 센터 서버의 현재 상태에 대한 스냅샷을 확보하도록 지원/ 정보 탐색후 수집한 정보로 마이그레이션 프로젝트를 계획하는데 도움을 줌

<br><h3>IP</h3>

<br>ROA(Route Origin Authorization) : 고객이 특정 자율 시스템에서 IP 알림을 인증하기 위해 RIR에서 생성한 객체

<br>Fixed IP : 고정 IP, 내부 IP

<br>Floating IP : 유동적 IP, 클라우드 내에서 가상머신이 인터넷과 외부망에 접근하기 위해 배정 받는 IP

<br><h3>기타</h3>

<br>IOPS(Input/Output Operation Per Second) : 초당 입출력 속도
<h6>&emsp;&emsp;&emsp;&emsp;IOPS SSD = 주요 성능 특성이 iops인 ssd</h6>

<br>ISCSI(Internet Small Computer System Interface) : 컴퓨터 환경에서 데이터 스토리지 시설을 이어주는 IP기반의 스토리지 네트워킹 표준
<br>IP망을 통해 SCSI 명령을 전달함으로서 인트라넷을 거쳐 데이터 전송을 쉽게하고 먼 거리에 걸쳐 스토리지를 관리하는데 쓰인다.

<br>이더넷(LAN에서 사용) - 인터넷 - 인트라넷(인터넷과 비슷하지만 폐쇠적)

<br>정적 콘텐츠(누가 언제 서버에 요청하더라도 같은 내용을 보여줌) / 동적 콘텐츠(누가,언제,어떻게 서버에 요청 하냐에 따라 다른 내용을 보여줌) 

<br>File Server란 : OS에 따라 Windows 파일서버, Unix 파일서버, Linux 파일서버가 있음
<br>&emsp;&emsp;&emsp;&emsp; Windows 파일서버는 CIFS(Common Internet File System)을 사용해서 클라이언트에 스토리지 공유
<br>&emsp;&emsp;&emsp;&emsp; Unix나 Linux는 NFS(Network File System)을 사용

<br>OLTP(OnLine Transaction Processing) : 온라인 트랜잭션 처리, 네트워크 상의 온라인 사용자들의 Database에 대한 일괄 트랜잭션 처리

<h6>&emsp;&emsp;&emsp;&emsp;트랜잭션 : 데이터베이스의 상태를 변화시키기 위해 수행하는 작업의 단위</h6>

<br>OLAP(OnLine Analytical Processing) : 데이터 웨어하우스 등의 시스템과 연관되어 Data를 분석, 정보를 분석/모델링 하게 하는 분석 방법

<br>NS(Name Server) : 도메인에 대한 정보(A레코드, MX레코드 등)을 가지고 있는 서버

<br>STS(Security Token Service) : AWS리소스에 대한 액세스를 제어할 수 있는 임시 보안 자격 증명을 생성

<br>RAID(Redundunt Array of Independent Disk) : 2개이상의 디스크를 병렬로 처리하여 성능 및 안정성을 향상시킴, 디스크 오류나 데이터 손실등 장애 대응을 위한 용도로도 사용할 수 있다.
<h6>
&emsp;&emsp;&emsp;&emsp; RAID-0 : 두 개 이상의 디스크에 데이터를 순차적으로 저장하는 방식, 
<br>&emsp;&emsp;&emsp;&emsp; 하나의 디스크에 문제가 생기면 모든데이터 유실, 오직 성능향상을 위한 방식
  
<br>&emsp;&emsp;&emsp;&emsp; RAID-1 : 데이터 처리 시, 동일한 디스크에 똑같이 저장하는 방식, 복구/안정성 높음, 용량 반으로 줄어듬

<br>&emsp;&emsp;&emsp;&emsp; RAID-3,4 :0과 같이 분산처리방식 + 에러 체크 및 수정을 위한 패리티(parity)정보를 별도 디스크에 저장

<br>&emsp;&emsp;&emsp;&emsp; RAID-5 : 분산 에러처리 / RAID-6 : 패리티, 최소 4개 이상의 하드 2개 까지 커버 

<br>&emsp;&emsp;&emsp;&emsp; RAID-10 : 우선 미러링 그후 스트리핑, 디스크 4개중 2개씩 미러링/스터리핑
  
</h6>

<br>SAML(Security Assertion Markup Language) 페더레이션(신뢰가 설정된 도메인의 컬렉션)

<br>192.168.0.1 -> A레코드 -> dev.blog.co.kr -> CNAME ->dev.plusblog.co.kr 

<br> ALIAS : 명령어

<br> SCP = 조직, OU = 조직 단위

<br> 스팟 플릿 : 사용자가 지정한 기준에 따라 시작되는 스팟 인스턴스의 집합

<br> ec2 플릿 : 인스턴스 유형, AWS 가용 영역, Amazon EC2 용량 등 간편하게 프로비저닝

<br> 스팟 블록 : 스팟 인스턴스

<br> 폴링 : 충돌 회피/동기화 처리 등을 목적으로 상태를 주기적으로 검사하여 일정한 조건을 만족할 때 송수신 등의 자료처리를 하는 방식

<br> 데이터 샤딩(Sharding) : 데이터를 다수의 데이터베이스에 분산하여 저장

<br>Exam Topics : https://www.examtopics.com/exams/amazon/aws-certified-solutions-architect-associate-saa-c02/

