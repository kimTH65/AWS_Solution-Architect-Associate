<h1>VPC（Virtual Private Cloud）- 가상 프라이빗 클라우드</h1>

<h2>VPC 사이징</h2>  
2^16(65536개)IP 주소 사용가능, 10.0.0.0/16 과 같은 CIDR(Classless Inter - Domain Routing)블록 형태 IP주소 필요
<br><br>허용된 CIDR 블록 사이즈 : 
<br> /28 netmask (minimum with 2 4 - 16 available IP address
<br> /16 netmask (maximum 2/6 16 available IP addddss 4 - 16 available IP address)

<br>개인이 비공개로 라우팅할 수 있는 IP 주소:
<br>10.0.0.0 ～ 10.255.255.255 (10/8 prefix)
<br>172.16.0.0 ～ 172.31.255.255 (172.16/12 prefix)
<br>192.168.0.0 ～ 192.168.255.255 (192.168/16 prefix)

<br>Ipv4는 수정 불가 But 보조 CIDR 연결 가능 

<br>인터넷에 대한 직접 액세스는 공개적으로 라우팅할 수 있는 CIDR에서 불가

<br>AWS 계정내/다른 계정의 vpc와 피어링 연결 가능

<br> 10.1.0.0/16 과 10.0.0.0/16 같은 경우는 OK, But 10.0.0.0/16 과 10.0.37.0/16 은 ip주소가 겹쳐서 연결 끊김

<br> CIDR은 범위가 같거나 더 낮은것과 연결 가능, 10.0.0.0/24 는 10.0.0.0/25 보다 범위가 작은것만 가능

<hr>

<h2>VPC 피어링 연결</h2> 
<br> IPV4/6 사용하여 연결, 같은 네트워크처럼 통신, 다른 계정/리전 VPC 연결가능,
<br> 일대일 관계, 단일 실패 지점 없음, 연결 수 제한 있음, 
<br> 기존 인프라를 이용해 연결하니 게이트웨이/ VPN 연결도 아니며 물리적 하드웨어에 의존 하지 않음,
<br> 트래픽을 AWS 빽본에 유지, 퍼블릭 인터넷 X, 별도 요금 X, 전송 요금 O, CIDR 블록 겹치면 연결 X,

<br> 문제가 생기면 ? 경로, 규칙, 허용, 차단 확인하기

<hr>

<h2>IP 주소</h2> 
<br> 개인 IP 주소 : 
<br> 인터넷 연결 할 수 없음, 내부 인스턴스를 통해 연결, 
<br> 인스턴스 중지 / 재시작 시 / 종료되는 경우에도 네트워크 인터페이스와 연결된다.

<br> 공용 IP 주소 : 
<br> 인터넷을 통해 연결 가능, AWS IP 주소 풀에서 할당되어 AWS 계정과 연결되지 않음,
<br> 인스턴스 중지/ 재시작 시 / 종료되면 해제

<br> 탄력적 IP 주소 : 
<br> 필요에 따라 인스턴스와 연결/해제 가능한 정적,영구적 공용 IP
<br> 해제되지 않는한 개인이 소유
<br> 사용하지 않아도 요금 청구

<hr>

<h2>Elastic Network Interface(ENI)</h2> 
<br> 각 인스턴스는 기본 탄력적 네트워크 인터페이스(기본 네트워크 인터페이스 eth0)에 연결되며 분리 못함

<hr>

<h2> Route Tables</h2> 
<br> 라우팅될 위치 경로 결정하는 규칙 정의, 각 VPC에는 네트워크 트래픽을 라우팅하는 암시적 라우터가 있음
<br> VPC내의 각 서브넷은 한 번에 하나의 라우팅 테이블과 연결되야함,But 라우팅 테이블에 여러 서브넷 연결될 수 있음
<br> 서브넷 경로 명시적으로 연결되지 않은 경우 기본 경로 테이블과 암시적으로 연결

<hr>

<h2> 인터넷 게이트웨이 (IGW)</h2> 

<br> 수평 확장/중복 가능, VPC인스턴스와 인터넷 간의 통신을 허용

<br> 공용 IP가 없으면 NAT(네트워크 주소 변환) 수행
<br>    &emsp; &emsp;&emsp; &emsp; NAT 사용하면 프라이빗 서브넷이 인터넷 접근 가능, But 인터넷에서 접근은 불가,
<br>    &emsp; &emsp;&emsp; &emsp; IPv6 트래픽 지원 x -> 송신 전용 게이트웨이(Egress-only Internet Gateway) 사용
<br>    &emsp; &emsp; &emsp; &emsp;&emsp; &emsp; 송신 전용 게이트웨이 :
<br>    &emsp; &emsp; &emsp; &emsp;&emsp; &emsp; IPv6 트래픽에 사용가능 ,인터넷으로 아웃바운드 허용,But 인터넷에서 인바운드 X
<br>    &emsp; &emsp; &emsp; &emsp;&emsp; &emsp; IPv4를 통한 아웃바운드 전용 인터넷 통신시 NAT 게이트웨이 사용해야함

<br> 트래픽 관리, 권한 부여 및 엑세스 제어, 모니터링 등 제공

<br> 인스턴스에 대한 인터넷 엑세스 사용방법 :
<br> &emsp; &emsp;&emsp; &emsp; 서브넷은 인터넷 게이트웨이의 경로가 있는 RouteTables 가지고 있어야함
<br> &emsp; &emsp;&emsp; &emsp; 인스턴스에 공용IP, 탄력적 IP 할당되어 있어야함
<br> &emsp; &emsp;&emsp; &emsp; 인스턴스와 연결된 보안 그룹 및 NACL이 관련 트래픽을 허용해야함

<hr>

<h2> VPC Security </h2> 

<br> Security groups : ec2 인스턴스에 대한 방화벽 역활, 인바운드 및 아웃바운드 트래픽 모두 제어
<br> &emsp; &emsp;&emsp; &emsp; Stateful 성질(요청 정보를 저장하여 응답하는 트래픽 제어를 하지않음)

<br> Network access control lists (ACLs) : 서브넷에 대한 방화벽 역활, 
<br> &emsp; &emsp;&emsp; &emsp; 서브넷 수준에서 인바운드 및 아웃바운드 트래픽 제어,
<br> &emsp; &emsp;&emsp; &emsp; 서브넷은 한가지 NACLs와 연결가능 But NACLs는 여러 서브넷과 연결가능, 
<br> &emsp; &emsp;&emsp; &emsp; Statelss 성질(요청 정보를 따로 저장하지 않기 때문에 응답하는 트래픽에 대한 필터링을 설정해야함)

<br> Flow logs : VPC의 네트워크 인터페이스로 오가는 IP트래픽에 대한 정보를 캡쳐
<br> &emsp; &emsp;&emsp; &emsp; Flow logs는 Amazon CloudWatch 로그를 사용하여 저장

<br> 같은 서브넷끼리 통신할 때 : Security Group 정책을 거치면서 통신
<br> 다른 서브넷끼리 통신할 떄 : NACL 정책을 거친후, Security Group을 거친다

<hr>

<h2> 서브넷 </h2>  
<br> 공용 서브넷과 비공개 서브넷은 IGW 연결 유무에 따라 달라진다.(인터넷이 연결 되어 있는지에 따라)

<br> 공용 서브넷은 공용 IP, 탄력적 IP 주소가 필요하다.

<br> VPN = 사설 게이트웨이, 인터넷에 연결되어 있진 않지만 가상 사설 게이트웨이를 통해 라우팅된 경우 VPN전용 서브넷 

<hr>

<h2> 공유 VPC </h2> 

<br> EC2 인스턴스, RDS 데이터베이스 같은 애플리케이션 리소스를 공유되고 관리되는 중앙 VPC로 생성, 다른 계정과 공유 가능

<hr>

<h2> VPC 엔드포인트 </h2> 

<br> AWS 서비스에 외부 인터넷 구간으로 접근하지 않고, 직접적으로 접근하여 강력한 보안을 제공하는 프라이빗 액세스 기능

<br> 게이트웨이 엔드포인트(S3, DynamoDB 서비스와 연결), 인터페이스 엔드포인트

<br> 프라이빗 네트워크를 이용한 다른 VPC 웹 서버 접근 방법
<br> &emsp; &emsp;&emsp; &emsp; EC2 인스턴스 → 인터페이스 엔드포인트 → 프라이빗 링크 →  NLB → 각각의 웹 서버
<br> &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;프라이빗 링크 : 인터페이스 엔드포인트와 엔드포인트 서비스를 통한 연결
