# AWS
<h3>
Language 
</h3>
<h5>
<a href="https://github.com/kimTH65/AWS/blob/main/README.md">한국어</a> 
&emsp;
<a href="https://github.com/kimTH65/AWS/blob/main/aws/japanese.md">日本語</a> 
<h2>コンピューティング(Computing)</h2>   


<a href="https://github.com/kimTH65/AWS/blob/main/aws/EC2.md">EC2(Elastic Compute Cloud)</a> : クラウドコンピューティングサービス


<br>  

<a href="https://aws.amazon.com/ja/lambda/faqs/">Lambda </a> : サーバーをプロビジョニングしたり管理したりする必要がないサーバーレスコンピューティングサービス

<br>

<a href="https://docs.aws.amazon.com/ja_jp/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html">Auto Scaling</a> : サーバー自動増設

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

<a href="https://aws.amazon.com/ja/route53/">Route53</a> - DNS(Domain Name System)

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

<a href="https://docs.aws.amazon.com/ja_jp/vpn/latest/s2svpn/VPC_VPN.html">VPN</a> : ネットワークとネットワーク間のセキュリティ接続を設定するサービス
<h6>
&emsp;&emsp;&emsp;&emsp;Site-to-Site VPN : Clasic VPN、AWS VPC環境とオンプレミス環境のVPN接続
<br><br>  
&emsp;&emsp;&emsp;&emsp;Clinet VPN : 個人がAWSサービスやオンプレミス環境に接続できるようにするサービス 
</h6>
  
<br>

<a href="https://aws.amazon.com/ja/cloudfront/">CDN(Cloud Front)</a> : コンテンツ配信ネットワーク=分散した複数のサーバ/atm機のような感じ、全世界に53のストレージあり

<br>

<a href="https://aws.amazon.com/ja/directconnect/?nc1=h_ls">Direct Connect</a> :データ専用線、AWS環境とオンプレミス環境との接続のためのサービスソリューション

<br>

Global Accelerator : AWSのグローバルネットワークインフラを通じてユーザートラフィックを送信し、パフォーマンスを向上させるネットワーキングサービス

<br>

API Gateway : APIを作成/運営/モニタリング(Cloud Watch)およびセキュリティを維持できるサービス、Lambdaと一緒にRESTApiを生成可能

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>ストレージ(Storage)</h2>

<h3>ストレージの種類</h3>

<a href="https://aws.amazon.com/ja/s3/?nc1=h_ls">S3</a>(Amazon Simple Storage Service, 一般)

<h6>&emsp;&emsp;&emsp;&emsp;バケット(Bucket) : 3 で生成できる最上位ディレクトリの概念、名前はS3 リージョンの中で唯一でなければならない </h6>

<h6>&emsp;&emsp;&emsp;&emsp;S3-CORS(Cross-Origin Resource Sharing) : 複数のドメインからアプリケーションのS3バケットへのコンテンツアクセスを許可するために使用されるメカニズム</h6>

<a href="https://aws.amazon.com/ja/s3/storage-classes/glacier/?nc1=h_ls">S3 - Glacier</a>(安価、データアーカイブ) 

<h6>&emsp;&emsp;&emsp;&emsp;Glacier vault lock : ボルトロックポリシーを使用してGlacierの各資格証明集について規定管理が可能。ロック可能</h6>
                             
<div align="center">
<br><h4>S3 ライフサイクル</h4> 
<img src="https://user-images.githubusercontent.com/59690816/167321873-67dc89e2-6c9b-4e9b-b69d-fdb8e7b3efe8.png" width="500" height="350">

<h6>出処 : https://docs.aws.amazon.com/ja_jp/AmazonS3/latest/userguide/lifecycle-transition-general-considerations.html</h6>
</div><br>
<a href="https://aws.amazon.com/ja/ebs/?nc1=h_ls">EBS</a>(Elastic Block Store, 速いブロック) 

<h6>&emsp;&emsp;&emsp;&emsp;DLM(Data Lifecycle Manager) : EBSスナップショット及び削除予約可能</h6>

<br>

<a href="https://docs.aws.amazon.com/ja_jp/fsx/?id=docs_gateway">Amazon FSx</a> : Windows Serverに構築される完全管理型ファイルストレージ、SMBプロトコルベース

<br> 

<a href="https://docs.aws.amazon.com/ja_jp/efs/latest/ug/whatisefs.html">EFS(Elastic File System)</a> : Linux Server、EC2用管理型ファイルストレージ、NFS/NASと同様のサービス、NFSプロトコルベース

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

<a href="https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/access_policies.html">IAM</a> - ユーザーアカウントとグループ管理

<h6>
&emsp;&emsp;&emsp;&emsp;<a href="https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/access_policies.html">IAMセキュリティベストプラクティス</a>:ルートユーザ使用アクセスキーロック、役割を使用して権限委任、最小権限付与など
</h6>

<br>

<a href="https://docs.aws.amazon.com/ja_jp/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html">Cloud Watch</a> : AWSサービス観察·モニタリングシステム
<br>

<a href="https://docs.aws.amazon.com/ja_jp/awscloudtrail/latest/userguide/cloudtrail-user-guide.html">Cloud Trail</a> : ユーザー観察、アカウントに対するAPI呼び出し記録

<br>

<a href="https://docs.aws.amazon.com/ja_jp/network-firewall/latest/developerguide/what-is-aws-network-firewall.html">FireWall</a> : ファイア・ウォール

<br>

<a href="https://docs.aws.amazon.com/ja_jp/cognito/latest/developerguide/cognito-user-identity-pools.html">Cognito</a> - ユーザーデータの同期と資格証明
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


<h2>アプリケーション</h2>

<a href="https://docs.aws.amazon.com/ja_jp/workspaces/?id=docs_gateway">Work Spaces</a>  - デスクトップを手軽にプロビジョニング / ユーザー無制限

<h6>&emsp;&emsp;&emsp;&emsp;プロビジョニング: ユーザーのニーズに合わせてリソース割り当て、配置、配布しておいて、すぐに使用できるように準備 </h6>

  
<br> 

<a href="https://docs.aws.amazon.com/ja_jp/workdocs/?id=docs_gateway">Work Docs</a> - ストレージおよび共有サービス / 無料トライアルユーザー最大50名

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>データベース.</h2>
<h3>リレーショナルデータベース</h3>

<a href="https://docs.aws.amazon.com/ja_jp/AmazonRDS/latest/UserGuide/Welcome.html">RDS</a> - 関係型DB、Mysql、Oracleなど

<br> 

<a href="https://docs.aws.amazon.com/ja_jp/redshift/latest/mgmt/welcome.html">Redshift</a> - DWで素早くデータクエリ、ペタ規模

<h6>&emsp;&emsp;&emsp;&emsp;DW（データウェアハウス）=ユーザの意思決定に役立つ、基幹システムのDBに縮尺されたデータを共通形式に変換して管理するDB</h6>

<br>

Aurora : MySQLおよびPostgreSQLと互換性のある完全管理型関係型データベースエンジン

<br>

<h3>キー値(NoSQL)</h3>

<a href="https://docs.aws.amazon.com/ja_jp/amazondynamodb/latest/developerguide/Introduction.html">DynamoDB</a> - NoSQL / SSDの使いやすさ、Qos(Quality of Service)自動的に最適化

<h6>&emsp;&emsp;&emsp;&emsp;TTL(Time to Live) = アイテムごとのタイムスタンプを定義し、アイテムが必要なくなる時期を決定</h6>

<br>

<h3>インメモリ</h3>

<a href="https://docs.aws.amazon.com/ja_jp/AmazonElastiCache/latest/red-ug/WhatIs.html">ElastiCache</a> - キャッシュクラスター、2つのメモリエンジンに対応(Redis/Memcached)

<h6>
&emsp;&emsp;&emsp;&emsp;ElastiCache for Redis : バックアップ、ソフトウェアパッチ、自動障害および復旧を管理、自動スナップショット/手動固有のバックアップスナップショット作成後に利用してクラスター復元
<br><br>
&emsp;&emsp;&emsp;&emsp;ElastiCache for Memcached : インメモリキー値ストアサービス、拡張可能、完全管理型サービス
</h6>

<br>

<h3>その他</h3>

PostgreSQL : オープンソースオブジェクト-関係型データベースシステム(ORDBMS)、関数/演算子など様々なデータベースオブジェクトのカスタムが可能

<br>

Amazon Neptune : グラフタイプ、IoTアプリケーション、DevOps、産業用テレメトリー

<br>

Amazon DocumentDB : 文書タイプ、コンテンツ管理、カタログ、ユーザープロファイル、MongoDB互換

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>分析</h2>

<a href="https://docs.aws.amazon.com/ja_jp/kinesis/?id=docs_gateway">Kinesis</a> - データ収集処理、リアルタイム処理
<h6>

&emsp;&emsp;&emsp;&emsp;Kinesis Data Streams : リアルタイムデータストリームをキャプチャ/処理/保存/分析してくれるサービス
<br><br>
&emsp;&emsp;&emsp;&emsp;Kinesis Data Analytics : Apache Flinkを使用してリアルタイムでストリーミングデータを変換し分析
<br>  
&emsp;&emsp;&emsp;&emsp;Kinesis Data Firehose : データストリーム処理/転送
  
</h6>
<br>

<a href="https://docs.aws.amazon.com/ja_jp/emr/?id=docs_gateway">Elastic Map Reduce(EMR)</a> - データプロセッシング / ホスティングされるHadoopフレームワークの活用

<br>

<a href="https://docs.aws.amazon.com/ja_jp/datapipeline/latest/DeveloperGuide/what-is-datapipeline.html">Data Pipeline</a> - データアクセス、変換処理、データの移動と変換を自動化するために使用できるWebサービス

<br>

Athena : S3に保存されたデータにクエリを飛ばして簡単にデータを分析できるSQLクエリサービス

<br>

QuickSight : クラウドベースのBI(Business Intelligence)ツールを提供する視覚化ツール

<br>

<a href="https://docs.aws.amazon.com/ja_jp/cloudsearch/?id=docs_gateway">CloudSearch</a> - 完全管理型サービス、ウェブサイト/アプリケーションのための検索ソリューションを簡単にインストール、管理、および拡張

<br>

AppFlow : コードなしでSaaSアプリケーションとAWSサービスの間で安全にデータを送信できる統合サービス

<h6>
&emsp;&emsp;&emsp;&emsp;SaaS(Software as a Service) : サービス型ソフトウェア、クラウドサービスで提供されるソフトウェア   
</h6>
  

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>アプリ·サービス</h2>

<a href="https://docs.aws.amazon.com/ja_jp/ses/latest/dg/Welcome.html">Simple Email Service(SES)</a> - トラックの電子メール、マーケティング メッセージは、異なるタイプの高品質コンテンツ、リアルタイムアクセス

<br>

<a href="https://docs.aws.amazon.com/ja_jp/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html">Simple Queue Service(SQS)</a> - メッセージ損失なしにすべてのスループットレベルでどのデータボリュームも送信、1つの保証But追加データ処理保障X、FIFO

<br>

<a href="https://docs.aws.amazon.com/ja_jp/amazonswf/latest/developerguide/swf-welcome.html">Simple WorkFlow(SWF)</a> - クラウドステータスの追跡、作業調整

<br>

<a href="https://docs.aws.amazon.com/ja_jp/amazon-mq/?id=docs_gateway">MQ(Message Queue)</a> : 管理型メッセージブローカーサービス

<h6>&emsp;&emsp;&emsp;&emsp;メッセージブローカー(message broker) : システムとサービスが互いに通信し、情報を交換できるようにするソフトウェア </h6>

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>配布および管理</h2>

<a href="https://docs.aws.amazon.com/ja_jp/opsworks/latest/userguide/welcome.html">OpsWorks</a> - アプリケーション構成と配布自動化/アプリケーション管理ソリューション、Puppet/ChefレシピおよびBashスクリプトを使用してコード構成
<h6>
&emsp;&emsp;&emsp;&emsp; Chef : オープンソースシステム管理フレームワーク、サーバインフラ構築自動化
<br><br>
&emsp;&emsp;&emsp;&emsp; Puppet : システムサーバ管理フレームワーク
</h6>

<br>

<a href="https://docs.aws.amazon.com/ja_jp/AWSCloudFormation/latest/UserGuide/Welcome.html">CloudFormaiton</a> - リソーステンプレートの作成 / テンプレートおよび関連するリソースコレクション(スタック)を配布および更新

<br>

<a href="https://docs.aws.amazon.com/ja_jp/elasticbeanstalk/latest/dg/Welcome.html">Elastic Beanstalk</a> - アプリケーションの自動配布処理と規模調整

<br>

<div align="center">
<h3>比較.</h3>
<h6>
便利=1. Elastic Beanstalk(全形態自動化)&emsp;2.OpsWorks(Chef/Puppet理解必要)&emsp;3. CloudFormaiton
<br><br>
自由度(詳細設定可能) = 1.Cloud Formaiton &emsp; 2.Ops Works &emsp; 3.Elastic Beanstalk
</h6>
</div>
<br>

<h3>開発者ツール</h3>

<a href="https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/welcome.html">CodeDeploy</a> - EC2インスタンス、オンプレミスインスタンス、サーバレスLambda関数などのサービスでアプリケーション配布を自動化するサービス

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>モバイル·サービス</h2>

<a href="https://docs.aws.amazon.com/ja_jp/sns/latest/dg/welcome.html">Simple Notification Service(SNS)</a> - 通知をスマホでプッシュ

<br>

Mobile Analytics - モバイル分析、レポート/Cognitoと統合される

<br>

AppSync : DynamoDB,Lambda など接続後のGraphQL(クエリ言語)API開発を容易にする完全管理型サービス

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>用語その他</h2>

<h3>クラウドコンピューティングモデル</h3>

<br>IaaS:サービスとしてのインフラ、クラウドITの基本構成要素

<br>PaaS:サービスとしてのプラットフォーム、基本インフラ管理不要、アプリケーションの配布·管理に集中

<br>SaaS:サービスとしてのソフトウェア、サービスプロバイダが運営·管理する完成品の提供

<br><h3>暗号化およびPKI(Public Key Infrastructure)</h3>

<br>SSE-S3 : Amazon S3 管理型鍵を使ったサーバ側暗号化、最も強力なブロック暗号(AES-256)を使用してデータ暗号化

<br>SSE-KMS : AWS Key Management サービスに保存されたKMSキーを使用したサーバ側暗号化

<br>SSE-C:顧客提供キーを使用したサーバ側暗号化、ユーザが暗号化キー管理

<br>ACM(AWS Certificate Manager):AWS認証書管理者

<br>Cloud HSM:管理型ハードウェアセキュリティモジュールで暗号化されたキーストレージを提供

<br><h3>Migration</h3>

<br>AWS SMS(Server Migration Service):VMware、Azureなどの仮想マシンをAWSクラウドにマイグレーションすることを自動化

<br>AWS MGN(Application Migration Service) : Lift and Shift マイグレーションに推奨される基本移行サービス

<h6> &emsp; &emsp; &emsp; Lift and Shift : アプリケーションをクラウドに移行する方式の一つ </h6>

<br>AWS DMS(Database Migration Service):DB、DWなどを簡単に移行できるクラウドサービス

<br>AWS ADS(Application Discovery Service):サーバー仕様情報、ハードウェア構成、性能、実行プロセス、ネットワーク接続情報などを収集し、データセンターサーバーの現在の状態に対するスナップショットを確保できるよう支援/情報探索後に収集した情報への移行プロジェクトを計画するのに役立つ

<br><h3>IP</h3>

<br>ROA(Route Origin Authorization):顧客が特定自律システムでIP通知を認証するためにRIRで生成したオブジェクト

<br>FixedIP:固定IP、内部IP

<br>Floating IP:流動的IP、 クラウド内で仮想マシンがインターネットと外部ネットワークにアクセスするために割り当てられるIP

<br><h3>その他</h3>

<br>IOPS(Input/Output Operation Per Second):毎秒入出力速度
<h6> &emsp; &emsp; &emsp; IOPS SSD=主な性能特性がipsであるssd</h6>

<br>ISCSI(Internet Small Computer System Interface):コンピュータ環境でデータストレージ施設をつなぐIPベースのストレージネットワーキング標準
<br>IP網を通じてSCSI命令を伝達することで、イントラネットを経てデータ伝送を容易にし、遠い距離にわたってストレージ管理を行うのに 使われる。

<br>イーザネット(LANで使用) - インターネット - イントラネット(インターネットと似ているが廃衰的)

<br>静的コンテンツ(誰がいつサーバに要請しても同じ内容を表示する)/動的コンテンツ(誰が、いつ、どのようにサーバに要請するかによって異なる内容を表示する) 

<br>File Serverとは:OSによってはWindowsファイルサーバ、Unixファイルサーバ、Linuxファイルサーバがある
<br> &emsp; &emsp; &emsp; Windows ファイルサーバーはCIFS (Common Internet File System) を使用してクライアントにストレージ共有
<br>&emsp;&emsp;&emsp;&emsp; Unix나 Linux는 NFS(NetworkFile System)を使用

<br>OLTP(OnLine Transaction Processing):オンライントランザクション処理、ネットワーク上のオンラインユーザのDatabaseに対する一括トランザクション処理

<h6> &emsp; &emsp; &emsp; トランザクション:データベースの状態を変化させるために行う作業の単位</h6>

<br>OLAP(OnLine Analytical Processing):データウェアハウスなどのシステムに関連してデータを分析、情報を分析/モデリングさせる分析方法

<br>NS(Name Server):ドメインに関する情報(Aレコード、MXレコードなど)を持っているサーバ

<br>STS(Security Token Service):AWSリソースへのアクセスを制御できる一時的なセキュリティ資格証明を生成

<br>RAID(Redundunt Array of Independent Disk):2つ以上のディスクを並列に処理して性能および安定性を向上させる、ディスクエラーやデータ損失など障害対応のための用途にも使用できる。
<h6>
&emsp; &emsp; &emsp; RAID-0 : 2つ以上のディスクにデータを順次保存する方式、 
<br> &emsp; &emsp; &emsp; 一つのディスクに問題が発生すると、すべてのデータ流失、ただ性能向上のための方式
  
<br> &emsp; &emsp; &emsp; RAID-1 : データ処理時、同じディスクに同じように保存する方式、復旧/安定性が高い、容量が半分に減る

<br> &emsp; &emsp; &emsp; RAID-3, 4:0 のように分散処理方式+エラーチェック及び修正のためのパリティ情報を別途ディスクに保存

<br>&emsp;&emsp;&emsp;&emsp;RAID-5:分散エラー処理 / RAID-6:パリティ、最低4つ以上のハード2つまでカバー 

<br> &emsp; &emsp; &emsp; RAID-10:まずミラーリングその後、ストリッピング、ディスク4つのうち2つずつミラーリング/スターリーピング
  
</h6>

<br>SAML(Security Assertion Markup Language)フェデレーション(信頼が設定されたドメインのコレクション)

<br>192.168.0.1 -> Aレコード -> dev.blog.co.kr -> CNAME ->dev.plusblog.co.kr 

<br>ALIAS:コマンド

<br>SCP=組織·OU=組織単位

<br>スポットフリート:ユーザーが 指定した基準に従って開始されるスポットインスタンスの集合

<br>ec2フリート:インスタンスタイプ、AWS可用領域、Amazon EC2容量など手軽にプロビジョニング

<br>スポットブロック:スポットインスタンス

<br>ポーリング:衝突回避/同期化処理などを目的に状態を周期的に検査し、一定の条件を満たす時に送受信などの資料処理を行う方式

<br>データシャーディング(Sharding):データを多数のデータベースに分散して保存

<br>Exam Topics : https://www.examtopics.com/exams/amazon/aws-certified-solutions-architect-associate-saa-c02/
