# EC2 (Elastic Compute Cloud)

<h2>EC2 機能</h2> 

<h3>基本事項</h3>

<a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/ec2-instances-and-amis.html">インスタンスおよびAMI(Amazon Machine Image)</a> : インスタンス=仮想コンピューティング環境/AMI=サーバに必要なOS、ソフトウェアを構成された状態で提供されるテンプレート
<h6>
&emsp;&emsp;&emsp;&emsp;PV(半仮想化)AMI:guest OSがHypervisor(仮想マシンを生成して実行するプロセス)によりHardwareを制御
<br><br>
&emsp;&emsp;&emsp;&emsp;HVM(ハードウェア仮想マシン)AMI : guestと完全に独立し、OS修正なしで使用が可能
</h6>
<br><br>
<a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/Using_Tags.html">タグ</a>:ユーザーが生成してAmazon EC2 リソースに割り当てることができるメタデータ
<br><br>
<a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/instance-types.html">インスタンスタイプ</a> : インスタンスのためのCPU、メモリ、ストレージ、ネットワーキング容量様々な構成を提供
<br><br><a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/using-regions-availability-zones.html">リージョン(Region)及び可用領域(AZ)</a>:インスタンスとEBSボリュームなどのリソースを他の物理的な場所からアクセスできるリージョン及び可用領域
<h6>&emsp;&emsp;&emsp;&emsp;AZ(Availability Zone) : 各リージョン内の隔離された位置、個別データセンターで構成されている</h6>
<hr>
<h3>ネットワーキング·セキュリティ</h3>
<br>
<a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/ec2-key-pairs.html">キーペア</a>で 
インスタンスログイン情報保護(AWSはパブリック鍵保存、ユーザーは秘密鍵安全場所に保管)
<br><br>
<a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/ec2-security-groups.html">セキュリティグループ</a>
を使用してインスタンスに接続できるプロトコル、ポート、ソースIP範囲を指定するファイアウォール機能
<br><br>
<a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/elastic-ip-addresses-eip.html">弾力的IPアドレス(EIP)</a>:動的クラウドコンピューティングのための固定IPv4アドレス
<br><br>

<a href="https://github.com/kimTH65/AWS/blob/main/aws/VPC_jp.md">VPC(Virtual Private Cloud)</a> : AWSクラウドから論理的に隔離されているが、希望するたびにお客様のネットワークと接続可能な仮想ネットワーク
<hr>
<h3>ストレージ</h3>
<br>インスタンスストアボリューム:一時データ保存するストレージボリューム、インスタンス中断、最大節電モード/終了時に削除される
<br><br>EBS(Elastic Block Store):Amazon EBSボリュームを使って永久 ストレージボリュームにデータを保存

<hr>
<h3>Linuxインスタンス作業</h3>
<br>AWS Systems Manager Run Command:PowerShellのようなものを利用して命令を送ること

<br>LAMP(Linux、Apache、MYSQL/MairaDB、PHP/Perl/Pythonのような言語)ウェブサーバー、LAMPスタック:
<br>&emsp;&emsp;&emsp;&emsp; Amazon Linux 2インスタンスにPHPおよびMariaDBサポートを含むApacheウェブサーバ

<br>Secure Sockets Layer/Transport Layer Security(SSL/TLS):ウェブサーバとウェブクライアントとの間で暗号化された チャンネルを作ってデータ盗聴防止

<hr>
<h3>Amazon EC2アクセス</h3>
<br>CLI(AWS Command Line Interface) 
<br><br>AWS Tools for Windows PowerShell

<hr>
<h3><a href="https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/instance-purchasing-options.html">Amazon EC2 価格</a></h3>
<br>プリティア:無料
<br><br>On-Demand instances:約定決済なしで秒単位で使用したインスタンス料金を支払う
<br><br>Savings Plans:1/3年間、1時間当たりUSDで一括した使用量を約定し、コスト削減
<br><br>予約インスタンス:1/3年間、インスタンスタイプ/地域を含めて特定のインスタンスに約定してコスト削減
<br><br>Spot Instances:未使用 EC2 インスタンス要請でコスト大幅削減
