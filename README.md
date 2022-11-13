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
