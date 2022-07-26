DB 외부 접근 허용
================
* 개요 : VirtualBox를 통해 VM을 하나 만들었다. yum install을 통해 MySQL 설치 후, 호스트 pc에서 접근하려고 하였는데 다음과 같이 에러가 출력.
* Host 'x.x.x.x' is not allowed to connect to this MySQL server
* 해결 방법 : GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' IDENTIFIED BY '패스워드'; 명령어를 통하여 모든 IP에 대한 접근을 허용해준다.
