# 080258

<도커 교과서> 예제 코드입니다.

# 실습 환경 초기화 명령

- 실습 환경 초기화

```shell
docker container rm -f ${docker container is -aq}
```

<br/>

- 이미지 용량 회수

```shell
docker image rm -f ${docker iamge ls -f reference='diamol/*' -q}
```


<br/>
<br/>
<br/>

# 컨테이너로 Hello World 실행하기

```shell
docker container run diamol/ch02-hello-diamol
```

![image](https://user-images.githubusercontent.com/46955032/201517015-7f52fe53-d22c-4a2e-b1e6-b5ab771f6c0a.png)
