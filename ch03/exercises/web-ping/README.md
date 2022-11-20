```dockerfile
FROM diamol/node

ENV TARGET="blog.sixed.com"
ENV METHOD="HEAD"
ENV INTERVAL="3000"

WORKDIR /web-ping
COPY app.js .

CMD ["node", "/web-ping/app.js"]
```


- `FROM` : 기반 이미지
- `ENV` : 환경변수
- `WORKDIR` : 작업 디렉토리
- `COPY` : 파일 복사
- `CMD` : 컨테이너 실행시 실행할 명령어

<br/>

- `FROM diamol/node` : diamol/node 이미지를 기반으로 하겠다는 의미
- `ENV TARGET="blog.sixed.com"` : 환경변수 TARGET에 blog.sixed.com을 넣겠다는 의미
- `ENV METHOD="HEAD"` : 환경변수 METHOD에 HEAD를 넣겠다는 의미
- `ENV INTERVAL="3000"` : 환경변수 INTERVAL에 3000을 넣겠다는 의미
- `WORKDIR /web-ping` :
- `COPY app.js .` : 현재 디렉토리에 있는 app.js를 /web-ping 디렉토리로 복사
- `CMD ["node", "/web-ping/app.js"]` : 컨테이너 실행시 node /web-ping/app.js를 실행하겠다는 의미

<br/>