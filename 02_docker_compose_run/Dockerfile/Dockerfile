FROM node:20.4.0

# 앱 디렉토리 생성 및 지정
RUN mkdir -p /data/service
WORKDIR /data/service

# node 셋팅을 위한 module 설치 
COPY ./source/ .
RUN cd /data/service
RUN npm install

# 앱 소스 추가 및 모듈 실행
EXPOSE 3001
CMD npm start