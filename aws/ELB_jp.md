# ELB(Elastic Load Balancer)

<h3>基本事項</h3>

Elastic Load Balancing :  Amazon EC2 インスタンス、コンテナおよびIP アドレスのような複数の対象に対して受信アプリケーションまたはネットワークトラフィックを複数の可用領域に配布

<br>On-premiseのL4スイッチのように負荷分散だけでなく負荷分散対象に対するヘルスチェック(Health Check)、固定セッション(Sticky)、SSL Offload(SSL暗復号化)、ヘルスチェックによるダウンサーバー除外などの機能

<h6>&emsp;&emsp;&emsp;&emsp;On-premise : サーバーをクラウドのような遠隔環境で運営X、独自に保有する電算室サーバーに直接設置して運営する方式を意味する
  
<br>&emsp;&emsp;&emsp;&emsp;L4スイッチ:ロードバランシング(負荷分散サービス)、外部要請をサーバが直接行わず、ソフトウェアが受信してサーバに適切に分配する。</h6>

<br>Connection Draining機能:ユーザーの要請を処理中のEC2インスタンスをすぐに削除できないようにする機能

<hr>
<h3>ELB種類 </h3>
Applicaiton Load Balancer(ALB):OSI 7 Layerの7階層Applicaiton Layerの特性を利用するロードバランサー、クライアントがサービスを要請する状況であるとき
<br> &emsp; &emsp; &emsp; HTTP、HTTPS の特性を主に扱う -> HTTP のヘッダ情報を用いて負荷分散を実施
<br> &emsp; &emsp; &emsp; SSL 認証書を搭載することができ、EC2 の下SSL暗号化/復号化の代わりに進行

<h6> &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; SSL(Secure Sockets Layer):セキュリティプロトコル/ 個人情報保護、認証、完全性をインターネット通信に提供 </h6>

<br> Network Load Balancer(NLB):OSI 7 Layerの4階層に該当し、送信者と受信者の論理的連結を担当、内部に入ってきたトラフィックを処理して内部インスタンスに伝送する際に
<br> &emsp; &emsp; &emsp; endpoint（ユーザ）間の接続を生成し、データをどれだけ送信したか、正しく受信したかなどを確認、TCP/UDPが 代表的

<h6> &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; TCP - データの正確性確認

<br> &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; UDP - ユーザーデータグラムプロトコル、速さ、ストリーミングのように連続性/速度が重要な時に使用</h6>

<br>Classic Load Balancer(CLB):ロードバランサーにインスタンスを登録してルーティング、最も古いロードバランサー(現在あまり使わない)
