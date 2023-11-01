# ELB(Elastic Load Balancer)

<h3>기본 사항</h3>

<br>Elastic Load Balancing :  Amazon EC2 인스턴스, 컨테이너 및 IP 주소와 같은 여러 대상에 대해 수신 애플리케이션 또는 네트워크 트래픽을 여러 가용 영역에 배포

<br>On-premise의 L4스위치처럼 부하분산뿐만 아니라 부하 분산 대상에 대한 헬스 체크(Health Check), 고정 세션(Sticky), SSL Offload(SSL 암복호화), 헬스 체크를 통한 다운 서버 제외등 기능

<h6>&emsp;&emsp;&emsp;&emsp;On-premise : 서버를 클라우드같은 원격 환경에서 운영X, 자체적으로 보유하는 전산실 서버에 직접 설치해 운영하는 방식을 의미

<br>&emsp;&emsp;&emsp;&emsp;L4스위치 : 로드 밸런싱(부하분산서비스), 외부 요청을 서버가 직접 하지않고 소프트웨어가 받아서 서버로 적절히 나누어 준다.</h6>

<br>Connection Draining 기능 : 사용자의 요청을 처리 중인 EC2 인스턴스를 바로 삭제하지 못하도록 하는 기능

<hr>
<h2>ELB 종류 </h2>
<br> Applicaiton Load Balancer(ALB) : OSI 7 Layer의 7계층 Applicaiton Layer의 특성을 이용하는 로드밸런서, 클라이언트가 서비스를 요청하는 상황일 때
<br>&emsp;&emsp;&emsp;&emsp; HTTP, HTTPS의 특성을 주로 다룸 -> HTTP의 헤더 정보를 이용해 부하분산을 실시 
<br>&emsp;&emsp;&emsp;&emsp; SSL 인증서를 탑재할 수 있어 EC2를 대신하 SSL 암호화/ 복호화를 대신 진행

<h6>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;  SSL(Secure Sockets Layer) : 보안 프로토콜/ 개인정보 보호, 인증, 무결성을 인터넷 통신에 제공</h6>

<br> Network Load Balancer(NLB) : OSI 7 Layer의 4계층에 해당, 송신자와 수신자의 논리적 연결을 담당, 내부로 들어온 트래픽을 처리하고 내부 인스턴스로 전송할 때
<br>&emsp;&emsp;&emsp;&emsp; endpoint(사용자) 간의 연결을 생성하고 데이터를 얼마나 보냈는지,제대로 받았는지 등 확인, TCP/UDP가 대표적

<h6>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;  TCP - 데이터의 정확성 확인
  
<br>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;  UDP - 사용자 데이터그램 프로토콜, 빠름, 스트리밍같이 연속성/속도가 중요할 때 사용</h6>

<br> Classic Load Balancer(CLB) : 로드밸런서에 인스턴스를 등록하고 라우팅, 가장 오래된 로드밸런서(현재 잘 안씀)
