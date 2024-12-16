# 🗣️ go-grpc-chat <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=Go&logoColor=white"/> <img src="https://github.com/user-attachments/assets/939c63cd-3dd9-43c2-9aee-f800ba4a22ae" height="20">
## 👉 Go 언어와 gRPC 프레임워크 기반으로 만든 채팅 프로그램
### ✅ 프로젝트 소개
Go 언어와 gRPC 프레임워크를 더 알아보기 위한 용도로 작성한 코드입니다.

### RPC란?
RPC는 다른 컴퓨터에게 "이걸 해줘!"라고 원격으로 명령을 요청하는 방식입니다.  
마치 내 컴퓨터 안에서 명령을 내리듯이, 멀리 있는 컴퓨터에 명령을 보낼 수 있게 되는 것입니다.  

클라이언트(요청하는 쪽)가 서버(작업하는 쪽)에게 요청을 보내고, 서버는 결과를 돌려줍니다.  
언제 명령이 들어올지 모르기 때문에 해당 과정은 수신 대기 중인 상태로 유지됩니다.  
또한 명령 요청 시에는 '직접 호출할 서버 함수'와 '전달해야 하는 데이터(파라미터)'를 포함해야 합니다.

### gRPC란?
gRPC는 구글 주도 하에 기존 RPC를 더 빠르고 효율적으로 만든 기술입니다.  
모든 환경에서 실행할 수 있다는 장점이 존재합니다.  
또한 기존 RPC 방식에 비해 추상화가 잘 되어 있어서 더 빠르고 쉽게 구현할 수 있다는 장점 또한 존재합니다.  

### '채팅 프로그램' 형태로 구현한 이유
'원격 명령 요청 방식'을 직관적으로 보기 위해서는 채팅 프로그램 형태가 적합하다는 생각이 들었습니다. 

### 코드 동작 전에 해야 하는 작업
1. 'server' 폴더 위치에서 'go build' 명령어를 입력합니다.
2. 'client' 폴더 위치에서 'go build' 명령어를 입력합니다.

### 코드 동작 방법 (Linux 기준 작성)
1. 'sesrver' 폴더 위치에서 './server' 명령어를 입력하여 server를 활성화시킵니다.
2. 'client' 폴더 위치에서 './client' 명령어를 입력하여 client_1을 활성화시킵니다.
3. 'client' 폴더 위치에서 './client' 명령어를 입력하여 client_2을 활성화시킵니다.  
+) 채팅 작업이므로 적어도 2명의 클라이언트가 존재해야 합니다. 따라서 2번&3번 과정 모두 필요합니다.
4. client_1과 client_2에 원하는 채팅 내용을 입력함으로써 정상적으로 동작하는지 확인합니다.

### 코드 실행 결과
![image](https://github.com/user-attachments/assets/8516a58f-ac58-4de7-9442-5272fd2964c2)
![image](https://github.com/user-attachments/assets/17a15cbe-edbc-4595-af17-8e9a671b0171)
