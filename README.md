## Netty 
자바 기반의 비동기 이벤트 기반 네트워크 애플리케이션 프레임워크



### [TCP 실행 순서]

(windows) 
1. 제어판
2. 프로그램 켜기/끄기
3. Telnet 끄기
4. PC 재시작
5. TCPServer.main() 실행
6. bash 창에서 'telnet localhost 8080' 명령어 실행


### ✔ Netty 서버의 기본 구조

1. **BossGroup**: 연결 수락 담당
2. **WorkerGroup**: 데이터 처리 담당
3. **ServerBootstrap**: 서버 설정 담당
4. **Pipeline**: 들어오고 나가는 데이터 처리 과정
5. **Handler**: 실제 비즈니스 로직 담당

### ✔ 문자열 송수신을 위해 Encoder/Decoder 사용

Byte 데이터를 String으로 변환.
