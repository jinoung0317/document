### Docker mariaDB container setting
### date : 2021-12-26

---

### 변경한 Docker image commit
 
```shell
    docker commit COMTAINER IMAGE_NAME
```

### docker image tag

1. docker cloud에 로그인
```shell
    docker login
```
 
2. docker user id 변수 지정
```shell
    export DOCKER_ID_USER=DOCKER_ID_USER
```
 
3. docker image에 태그 달기
```shell
    docker tag DOCKER_TAG $DOCKER_ID_USER/IMAGE_NAME
```

### docker image push

4. docker image push 하기
```shell
    docker push $DOCKER_ID_USER/IMAGE_NAME
```


## 예제
```shell
    > docker commit DB-DEV mariadb

    > docker login

    > export DOCKER_ID_USER="kestrel960408"

    > docker tag mariadb $DOCKER_ID_USER/mariadb:10.5.9

    > docker push $DOCKER_ID_USER/mariadb
```


 
[REPO]
 
 1. [Docker(도커) 컨테이너 커밋, 이미지 푸쉬하기](https://nicewoong.github.io/development/2018/03/06/docker-commit-container/)


 