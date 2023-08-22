# AWS

<h2>コンピューティング(Computing)</h2>   


<a href="https://github.com/kimTH65/AWS/blob/main/aws/EC2.md">EC2(Elastic Compute Cloud)</a> 　:　クラウドコンピューティングサービス


<br>  

<a href="https://aws.amazon.com/ko/lambda/faqs/ "> Lambda </a>　:　サーバーをプロビジョニングしたり管理したりする必要がないサーバーレスコンピューティングサービス

<br>

<a href="https://docs.aws.amazon.com/ko_kr/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html">Auto Scaling</a>　:　サーバー自動増設

<br> 
 
SAM(Serverless Application Model)　:　サーバレスアプリケーションをビルドするための配布ツール 

<hr>

 
<!--                                        ----------------------------------------------------------                                      -->


<h2>コンテナ(Container)</h2>  

<a href="https://github.com/kimTH65/AWS/blob/main/aws/ECS.md">ECS(EC2 Container Service)</a>　:　Docker コンテナ管理サービス

<br>

ECR(Elastic Container Registry)　:　Dockerコンテナ画像を保存するRepositoryサービス 

<br>

EKS(Elastic Kubernetes Service)　:　Kubernetesを簡単に実行できる管理型サービス

<h6>
&emsp; &emsp; &emsp; Kubernetes : 複数のコンテナ(Docker)を管理するサービス
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
&emsp; &emsp; &emsp; Latency Based Routing : 現在位置で遅延時間(Latency)が最も低いリージョンのIPアドレスを知らせる
<br><br>
&emsp;&emsp;&emsp; &emsp; Weighted Round Robin : サーバーIPアドレスまたはドメイン(ELB)ごとに重み付けされるトラフィックを調節する機能
<br><br>
&emsp; &emsp; &emsp; DNS Failover:障害が発生したサーバのIP アドレスまたはドメイン（ELB）を知らせない機能
<br><br>
&emsp; &emsp; &emsp; Geo Routing : 地域別に異なるIPアドレスを教える
</h6>

<br>

<ahref="https://docs.aws.amazon.com/ko_kr/vpn/latest/s2svpn/VPC_VPN.html ">VPN</a>:あるネットワークとネットワークの間にのセキュリティ接続を設定するサービス
<h6>
&emsp; &emsp; &emsp; Site-to-Site VPN : Clasic VPN、AWS VPC環境とオンプレミス環境のVPN接続
<br><br>  
&emsp; &emsp; &emsp; Clinet VPN : 個人がAWSサービスやオンプレミス環境に接続できるようにするサービス 
</h6>
  
<br>

<ahref="https://aws.amazon.com/ko/cloudfront/ ">CDN(Cloud Front)</a>:コンテンツ配信ネットワーク=分散された複数のサーバ/atm機のような感じ、全世界に53のストレージあり

<br>

<ahref="https://aws.amazon.com/ko/directconnect/ ?nc1=h_ls">Direct Connect</a>:データ専用線、AWS環境とオンプレミス環境との連結のためのサービスソリューション

<br>

Global Accelerator:AWSのグローバルネットワークインフラを通じてユーザートラフィックを送信し、性能を改善するネットワーキングサービス

<br>

API Gateway : APIを生成/運営/モニタリング(Cloud Watch)およびセキュリティを維持できるサービス、Lambda一緒にRESTApiを生成可能

<hr>


<!--                                        ----------------------------------------------------------                                      -->


<h2>ストレージ</h2>

<h3>ストレージ種類</h3>

<a href="https://aws.amazon.com/ko/s3/?nc1=h_ls">S3</a>(Amazon Simple Storage Service, 일반)

<h6> &emsp; &emsp; &emsp; バケット(Bucket) : S3 で生成できる最上位ディレクトリの概念、名前はS3 リージョンの中で唯一でなければならない。 </h6>

<h6> &emsp; &emsp; &emsp; S3 - CORS (Cross-Origin Resource Sharing) : 複数のドメインでアプリケーションのS3バケットへのコンテンツアクセスを許可するために使用されるメカニズム</h6>

<a href="https://aws.amazon.com/ko/s3/storage-classes/glacier/?nc1=h_ls">S3 - Glacier</a>(저렴,데이터 아카이빙) 

<h6> &emsp; &emsp; &emsp; Glacier vaultlock : ボルトロックポリシーを使用してGlacierの各資格証明集に対して規定管理が可能。
