# CustomEmojiChatting   
Media Interface Lab 2020-2 데모 프로젝트 중 일부인 커스텀 이모티콘 채팅 코드 입니다.   
본 프로젝트는 실제 배포용이 아닌 아이디어 프로토타입용 프로그램입니다.

### 1. 프로젝트 개요   
  * 사용자가 직접 텍스트를 변경 할 수 있는 이모티콘 제공한다.   
    > 이모티콘에 나타나는 텍스트를 사용자가 변경할 수 있다.    
    > 이모티콘 내 텍스트의 위치와 폰트, 색상은 제작자가 에디터에서 정해놓은 템플릿을 따른다.      
  * 이모티콘 제작자에게 이모티콘의 기본 템플릿을 설정 할 수 있는 에디터를 제공한다. 위치 지정 및 폰트, 색상 설정이 가능하다.   
  
### 2. 채팅 구현 방법   
  * Node.js 와 Express를 이용해 서버 생성
  * Socket.io 를 이용해 실시간 통신
  * multer-s3를 이용해 이모티콘 전송 시 AWS S3 버킷에 커스텀 이모티콘 이미지 저장 후 수신자에게 전송

![image](https://user-images.githubusercontent.com/20807197/110667205-6411b580-820d-11eb-85af-7c55f2f8708b.png)

  
### 3. 실행 사진   
* 기본적인 텍스트 채팅과 이모티콘 전송이 가능합니다.
   
![image](https://user-images.githubusercontent.com/20807197/110664114-7c340580-820a-11eb-928d-1f05af96928b.png)
   
![image](https://user-images.githubusercontent.com/20807197/110667558-b7840380-820d-11eb-8d64-3873b286eb12.png)

* 이모티콘에 10자와 30자까지 제작자가 지정한 위치에 삽입이 가능합니다.
      
![image](https://user-images.githubusercontent.com/20807197/110667430-96bbae00-820d-11eb-955d-46a81f7bc0ef.png)

![image](https://user-images.githubusercontent.com/20807197/110667683-daaeb300-820d-11eb-9fef-4e35b0aab88b.png)

![image](https://user-images.githubusercontent.com/20807197/110667736-e7330b80-820d-11eb-95ad-7a82f0411a4f.png)

* 10자 전송 화면
   
![image](https://user-images.githubusercontent.com/20807197/110667355-80aded80-820d-11eb-9c55-eb90c419158d.png)
   
* 30자 전송 화면
   
![image](https://user-images.githubusercontent.com/20807197/110667952-22cdd580-820e-11eb-999c-a7d81f9174d0.png)


### 4. Dependencies   
  "dependencies": {   
      "aws-sdk": "^2.834.0",   
      "express": "^4.17.1",   
      "multer": "^1.4.2",   
      "multer-s3": "^2.9.0",   
      "ngrok": "^3.4.0",   
      "socket.io": "^3.0.5"   
  }   
  
### 5. 개발자   
숙명여자대학교 미디어 인터페이스 연구실 학부생 인턴 - 채정아, 김시원, 전희선
