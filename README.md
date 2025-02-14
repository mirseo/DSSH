# DSSH - mirseo SHELL

이 프로젝트는 디스코드를 이용하여 SSH (Bash) 쉘을 에뮬레이션해 서버간 접속을 구현합니다.  

## 주요 기능

- 디스코드 메시지를 이용한 SSH 쉘 에뮬레이션
- 서버 간 파일 전송 및 수신
- 서버 간 명령어 실행
- 서버 간 파일 관리

## 설치 방법

1. Discord 로그인 
2. 봇 초대
3. 봇 설정 (서버 등록)
4. 명령어 사용

## 명령어

- `mirseo connect <서버 이름>`: 가상셸 접속
- `mirseo bash <실행할 명령줄>`: 원격 명령 실행
- `mirseo 2fa <enable/disable>`: 명령 실행 시 2단계 인증 요구 여부 설정
- `mirseo serverinfo`: 서버 정보 반환
- `mirseo connect verify`: 가상셸 연결 시 인증절차 수행(서버 실 소유자 인증 - 생성된 인증파일 업로드)

## 예시

```bash
mirseo connect server1 session(2)
mirseo bash ls
mirseo proxy <port> <http.auth.username> <http.auth.password> # 프록시 기반으로 내부 터널링 (cf 이용 / 토큰 입력 필요)
```
