VPC（Virtual Private Cloud）- 가상 프라이빗 클라우드

<h2>VPC 사이징</h2>  
2^16(65536개)IP 주소 사용가능, 10.0.0.0/16 과 같은 CIDR(Classless Inter - Domain Routing)블록 형태 IP주소 필요
<br><br>허용된 CIDR 블록 사이즈 : /28 netmask (minimum with 2 4 - 16 available IP address
<br> /16 netmask (maximum 2/6 16 available IP addddss 4 - 16 available IP address)
<br>172.16.0.0 ～ 172.31.255.255
<br>192.168.0.0 ～ 192.168.255.255
<br>Ipv4는 수정 불가 But 보조 CIDR 연결 가능 
<br>인터넷에 대한 직접 액세스는 CIDR에서 불가
<br>AWS 계정내 다른 vpc와 피어링 연결 가능
<hr>

<h2>VPC 피어링 연결</h2> 
<br>IPV4/6 사용하여 연결, 같은 네트워크처럼 통신, 다른 계정/리전 VPC 연결가능, 일대일 관계, 단일 실패 지점 없음, 기존 인프라 사용, 하드웨어 의존X,
트래픽을 AWS 빽본에 유지, 퍼블릭 인터넷 X, 별도 요금 X, 전송 요금 O, CIDR 블록 곂치면 연결 X, 연결 수 제한 있음
게이트웨이, 프라이빗 연결x

