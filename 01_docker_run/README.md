# Docker 명령어로 컨테이너 실행하기

## docker 컨테이너 실행
``` bash
$ docker run [옵션] [image:tag]

# httpd:latest 이미지를 가져와 컨테이너명을 example_httpd 로 지정하여 실행한다.
$ docker run --name nodeserver node:21-alpine3.18
```
![docke-1-1](./../data/img/docker-1-1.png)  

## 문제 1
아래의 명령어가 의미하는바를 작성 하세요.
``` bash
$ docker run -d --name ex_jenkins --restart=on-failure \
-p 8001:8080 \
-v /data/data/jenkins:/var/jenkins_home \
-e TZ=Asia/Seoul \
--network siwon-network \
jenkins/jenkins:jdk21

```

## 문제 2
아래의 옵션에 해당하는 컨테이너 실행하는 명령어를 작성하세요.
``` text
- 컨테이너 이미지 : node:21-alpine3.18
- 백그라운드 실행
- 컨테이너명 : study_node
- 포트 : 외부에서 8100 로 들어와 내부에 3001으로 받음
- restart : always
- 볼륨 : ./data -> /data
- 환경설정 : 
    - TZ=Asia/Seoul # 서버 시간 설정
```
