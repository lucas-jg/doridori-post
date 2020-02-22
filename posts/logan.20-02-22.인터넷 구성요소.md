   ### 인터넷 구성요소
- Protocol 
    - TCP / IP
        - Transmission Control Protocol / Internet Protocol
        - 정의
            - 통신 개체간의 교환되는 메시지 포멧과 순서, 송수신, 다른 이벤트체 따른 행동들을 정의
        - 인터넷의 규칙
        - 인터넷의 모든 해동은 프로토콜을 통해 제어
        - 프로토콜의 역할
            - End System
                - Congestion - Control Protocol
                    - 송수신자 간의 패킷 조절
            - Router
                - 데이터 경로 설정

    - 계층구조
        - Stack
            - Application Layer
                - HTTP 프로토콜 : 웹문서 요청과 전송
                - FTP 프로토콜 : 파일 전송
                - DNS (Domain Name Service) : 도메인 주소 연결
                - Packet : Application에서는 Message로 표현
                
            - Transport Layer
                - TCP / UDP 프로토콜
                    - TCP
                        - 목적지로 Message 전달 보장
                        - 긴 메세지는 짧게 나눔
                        - Congestion Control Protocoal : 흐름제어
                    - UDP
                        - 위의 여러기능을 하지 않는 심플한 Protocol
                - Packet : Transport에서는 Segment로 표현
                
            - Network Layer
                - IP Protocol
                    - 출발지와 목적지에 대한 주소
                    
            - Physical Layer
                - 하드웨어적인 비트 전송 관련 역할
                - 이더넷 광케이블, 동축케이블의 구조가 다른 것들의 비트 전달 방식 조정
                
- endSystem, Host
    - 인터넷에 연결되는 컴퓨터나 다른 모든 장치를 이르는 말
    - 두 컴퓨터가 통신 할 때, 두 컴퓨터는 끝과 끝에 있고 그 사이에 데이터를 주고 받는 방식
    - 하위에는 Client, Server
    
- 처리량 : ThroughPut
    - 네트워크 경로를 따라 두 프로세스 간의 통신세션에서 송신 프로세스가 수신 프로세스로 비트를 전달할 수 있는 비율
    - 컴퓨터간 데이터 전달시 일정시간에 비트량의 수신과 송신
