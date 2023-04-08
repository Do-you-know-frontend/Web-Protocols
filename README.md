# 웹 프로토콜

**1. 웹과 인터넷의 차이**

인터넷은 웹( WWW = World Wide Web )이 아닙니다.

- **인터넷**
    - TCP/IP 기반의 네트워크가 세계적으로 확대되어 연결된 네트워크들의 네트워크를 의미합니다.
- **웹**
    - 웹은 **HTML**이라는 문서 형태와 **HTTP**라는 문서 전송 프로토콜, **URL**로 문서의 위치를 표시하는 시스템을 말합니다.
    - 멀리 떨어진 사람에게 문서를 주고받기 위해 탄생했습니다.

즉, 웹보다 인터넷이 더 광범위한 범주이며, 인터넷으로 여러 기능을 할 수 있는데 그 중에서 **HTTP 프로토콜**을 사용하는 웹이 있는 것입니다.

### 네트워크 프로토콜

컴퓨터와 컴퓨터가 통신을 하려면 일종의 약속 ⇒ 프로토콜(양식)

- 가까운 곳와 연락할 때 : Ethernet 프로토콜 (MAC 주소)
- 멀리 있는 곳과 연락할 때 : ICMP IPv4 ARP (IP주소)
- 여러가지 프로그램으로 연락할 때 : TCP UDP (포트번호)

# **1. 웹이란?**

### **(1) 웹의 정의**

- 월드 와이드 웹(World Wide Web)
- 줄여서 www 또는 웹이라고 함
- 웹은 인터넷에서 운영되는 서비스 중 하나 -> 따라서 웹 자체가 인터넷을 의미하는 것이 아니다.
- 웹을 개발하는 목적? -> 연구자들이 흩어져 있는 정보를 손쉽게 정리하고 공유하기 위함

![https://blog.kakaocdn.net/dn/0SNzP/btrGupyRRO3/so2NiUgpgxG2JnKeAEUVLk/img.png](https://blog.kakaocdn.net/dn/0SNzP/btrGupyRRO3/so2NiUgpgxG2JnKeAEUVLk/img.png)

### **(2) 웹의 특징**

- 인터넷은 컴퓨터 네트워크망을 의미하고, 웹은 인터넷 서비스 중 하나를 의미함
- 인터넷상의 정보를 하이퍼텍스트 방식과 멀티미디어 환경에서 검색할 수 있게 해주는 정보 검색 시스템을 의미함
- HTTP 프로토콜을 사용하며, HTML 문서를 연결하여 다양한 콘텐츠를 제공함
- **많은 사람들이 정보를 쉽게 공유하고 접근할 수 있도록 하는 것을 목적으로 함**

### **(3) 웹의 구조**

- HTML을 중심으로 한 웹의 동작 과정

![https://blog.kakaocdn.net/dn/bf3BgL/btrGv5NbMOE/cVufj8gNrxys9z6zRqK921/img.png](https://blog.kakaocdn.net/dn/bf3BgL/btrGv5NbMOE/cVufj8gNrxys9z6zRqK921/img.png)

# **2. 네트워크**

### **(1) 네트워크(Network)의 정의**

- 사전적 의미 : 전선이나 혈관, 통로 등으로 이루어진 망형 조직
- 가장 많이 쓰이는 의미 : 컴퓨터와 컴퓨터를 연결해주는 망

### **(2) 네트워크를 구축하기 위한 컴퓨터 간의 연결 규격 : 프로토콜(Protocol)**

- TCP/IP : 여러 프로토콜 중 가장 널리 쓰이며 인터넷에서도 사용되고 있는 프로토콜

### (3) 네트워크 계층 모델

1) **TCP/IP 모델**

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b8bcc769-c2c6-459d-9d99-21f115095c7d/Untitled.png)

- 차이점
    - OSI는 **역할** 기반, TCP/IP는 **프로토콜** 기반
    - OSI는 통신 전반에 대한 표준, TCP/IP는 데이터 전송기술 특화

2) **OSI 7계층** 모델-계층별 프로토콜

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4c2aef01-d07e-4c9b-9ed6-2755f953d332/Untitled.png)

빨간박스-프로토콜 구조까지 알기

### 1**) TCP/IP(Transmission Control Protocol/Internet Protocol)**

- 컴퓨터 간에 통신할 수 있도록 만든 프로토콜의 종류 중 한 가지
- TCP/IP 프로토콜에 기반하고 있는 것이 인터넷이다
- TCP/IP가 인터넷의 기반 프로토콜로 자리 잡은 이유? -> 하드웨어, 운영체제, 접속 매체와 관계없이 동작할 수 있는 개방형 구조이기 때문

![https://blog.kakaocdn.net/dn/coCoXe/btrGuR9KGj2/1pJ9nEzRX3goPK1oBFXh41/img.png](https://blog.kakaocdn.net/dn/coCoXe/btrGuR9KGj2/1pJ9nEzRX3goPK1oBFXh41/img.png)

### 1-1**) TCP/IP의 특징**

- TCP/IP는 이러한 OSI 7계층을 좀 더 단순화하여 4계층으로 정의한 것임
- TCP : 데이터 흐름 관리, 데이터 정확성 확인 등의 역할을 수행함
- IP : 데이터(패킷)를 목적지까지 전송하는 역할을 담당함
- TCP/IP는 개방형 구조로, 특정 운영체제나 하드웨어에 영향을 받지 않고 근거리와 원거리 모두 데이터를 전송할 수 있음

**OSI 7계층**

- 네트워킹을 위한 물리적 장비에서부터 실제 서비스를 제공하기 위한 애플리케이션에 이르는 단계까지 계층화한 것을 의미함
- 계층화를 통해 상위 레벨에서는 하위 레벨에서 구현한 내용을 모르더라도 표준화된 인터페이스를 통해 네트워크 시스템을 개발, 운영할 수 있음

i**P 주소(IP Address)**

- TCP/IP로 연결된 네트워크에서 각각의 컴퓨터를 구분하기 위해 사용하는 주소
- IP 주소는 숫자로 구성되어 있음
- '123.123.123.123'과 같이 4개로 구분되며, 10진수를 사용함
- 사용할 수 있는 IP 주소 범위

![https://blog.kakaocdn.net/dn/X5FNf/btrGuT7yYTK/VkhkKbdka1KFV1FUElAdsK/img.png](https://blog.kakaocdn.net/dn/X5FNf/btrGuT7yYTK/VkhkKbdka1KFV1FUElAdsK/img.png)

# **3. 인터넷**

### **(1) 인터넷 기반 서비스**

- 웹 이외에도 이메일, FTP, Telnet, DNS 등이 있지만 일반적으로 사용하는 인터넷 기반 서비스로는 웹이 절대적임
- 이메일은 네이버, 다음, 구글과 같은 웹 기반의 메일 서비스를 이용하는 경우가 많음

![https://blog.kakaocdn.net/dn/bZdiVb/btrGtQKtdG0/0K9KIYuBkckjEuiHxbrlk0/img.png](https://blog.kakaocdn.net/dn/bZdiVb/btrGtQKtdG0/0K9KIYuBkckjEuiHxbrlk0/img.png)

## SMTP (Simple Mail Transfer Protocol)

메일 전송 프로그램이 서버로 메일을 보낼 때 사용하는 프로토콜이다. 오직 텍스트만 전송이 가능한 것이 특징이고, 스트림 방식을 이용하여 전송한다. SMTP 는 한 개의 메시지를 해당 서버의 여러 수신자에게 보낼 수 있다는 특징이 있다. 상태 코드는 250 (수신 성공), 550 (수신자 못 찾음)

## FTP (File Transfer Protocol)

파일이 문서, 이미지, 프로그램 등 다양한 형태의 데이터를 갖고 있을 수 있기 때문에 컴퓨터 간의 파일 교환시에 호환성을 보장하는 프로토콜이 필요하다. 컴퓨터 간의 호환성이라는 것은 예를 들어, 한 컴퓨터에서는 JPEG 이미지가 .jpg 로 저장되지만 다른 컴퓨터에서는 .jpeg 로 저장될 수 있다. 또한 어떤 컴퓨터는 파일 경로를 (/) 를 사용하지만 다른 컴퓨터는 () 를 사용할 수도 있다. 이렇기 때문에 파일 전송에 대한 규약인 프로토콜을 이용하여 상호 컴퓨터 간에 파일 전송이 가능하다. FTP 의 특성은 다음과 같다.

- 어떤 형태의 데이터든 전송이 가능하다.
- 파일을 다운로드 & 업로드 할 수 있다.
- 파일에 대한 권한을 설정할 수 있다.
- ASCII 문자로 메시지가 교환된다.
- 파일을 검색하고 조회할 수 있다.

브라우저에서 파일을 다운로드 하게 되면 바로 FTP 프로토콜을 사용하게 된다.

## FTP 통신 방식

HTTP 와는 다르게 FTP 는 클라이언트에서 서버로 한번 연결을 맺어놓은 상태에서 파일을 주고 받는 것이 아니라. 클라이언트에서 서버와의 연결이 맺어지면, 해당 연결은 명령어 입력을 위해 남겨놓고 (Control Connection), 파일을 보낼 때 새로운 연결을 추가하여 파일을 전송한다. (File Connection)

## **SSH**

시큐어 셀(Secure SHell, SSH)은 네트워크 상의 다른 컴퓨터에 로그인하거나 원격 시스템에서 명령을 실행하고 다른 시스템으로 파일을 복사할 수 있도록 해주는 응용 프로그램 또는 그 프로토콜을 가리킨다. 즉, 네트워크 프로토콜 중 하나로 컴퓨터와 컴퓨터가 인터넷과 같은 Public Network를 통해서 서로 통신을 할 때 보안적으로 안전하게 통신을 하기 위해 사용하는 프로토콜이다.

**대표적인 사용 :
    1. 데이터 전송
    2. 원격 제어데이터 전송의 예 :
    ◦ 깃 허브
    ◦ 원격 저장소, 소스 코드를 원격 저장소인 깃헙에 푸쉬할 때 SSH를 활용해 파일을 전송하게 된다.원격 제어의 예 :
    ◦ AWS와 같은 클라우드 서비스는 인스턴스 서버에 접속하여 해당 머신에 명령을 내리기 위해서 SSH을 통한 접속을 해야한다.사용이유 :
    ◦ 보안때문에 FTP나 Telnet과 같은 다른 컴퓨터 통신을 사용하지 않는다.
    ◦ SSH는 보안적으로 훨씬 안전한 채널을 구성한 뒤 정보를 교환하기 때문에 보다 보안적인 면에서 뛰어나다.**

[웹 개발자를 위한 Web Protocols 정리](https://joshua1988.github.io/web-development/web-protocols/)

### **(3) 네트워크에 연결된 컴퓨터들 간의 통신 규약 : 프로토콜(Protocol)**

- [표 1-2]의 서비스는 모두 TCP/IP를 사용하며, TCP/IP 4계층 중에서도 응용 계층에 해당하는 프로토콜임
- 즉 물리적인 네트워크 연결은 TCP/IP를 사용하지만, 응용 계층에서는 서비스마다 별도의 규격이 필요함

### **(4) 네트워크 서비스를 제공하기 위한 일종의 출입문 : 포트(Port)**

- 하나의 컴퓨터에서 여러 개의 네트워크 서비스를 제공하는 경우 이들을 구분하기 위한 목적으로 사용함

- 예) 은행에서 입출금, 대출, 신용카드, 보험 등 업무에 따라 창구를 구분해놓기

- 포트와 프로토콜이 일치하지 않는 경우 정상적인 네트워크 서비스를 이용할 수 없음

### **(5) 도메인 네임 시스템(Domain Name System)**

- 컴퓨터의 IP 주소는 네트워크에서 컴퓨터를 구분해주는 주민번호와 같은 개념
- 인터넷 주소의 형태 : 호스트(컴퓨터) 이름(www) + 도메인 이름(hanbit.co.kr)도메인 이름은 규칙에 따라 붙여지며, 도메인을 관리하는 기관에 일정 비용을 지불하고 구매해야 함
- 도메인 이름을 통한 웹 사이트 접속도 겉으로는 보이지 않지만 내부적으로 도메인 이름을 IP 주소로 변환하는 서비스를 이용함

![https://blog.kakaocdn.net/dn/SpYpE/btrGyOxd0Ty/FaLlYKjL4j6sUt3c9uQ7k0/img.png](https://blog.kakaocdn.net/dn/SpYpE/btrGyOxd0Ty/FaLlYKjL4j6sUt3c9uQ7k0/img.png)

참고 및 출처

짧고 굵게 배우는 JSP 웹 프로그래밍과 스프링 프레임워크(황희정/한빛아카데미(주))
