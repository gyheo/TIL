# Docker

## docker 주요 명령어

```shell
컨테이너 생성 및 시작
$ docker run [image]

컨테이너 생성
$ docker create [image]

컨테이너 시작
$ docker start [container]

실행중인 컨테이너 상태 확인
$ docker ps

전체 컨테이너 상태 확인
$ docker ps -a

컨테이너 상세 정보 확인
$ docker inspect [container]

컨테이너 종료 (SIGTERM 시그널 전달)
$ docker stop [container]

컨테이너 강제 종료 (SIGKILL 시그널 전달)
$ docker kill [container]

모든 컨테이너 종료
$ docker stop $(docker ps -a -q)

컨테이너 삭제 (실행중인 컨테이너 불가)
$ docker rm [container]

컨테이너 강제 종료 후 삭제 (SIGKILL 시그널 전달)
$ docker rm -f [container]

컨테이너 실행 종료 후 자동 삭제
$ docker run --rm ...

중지된 모든 컨테이너 삭제
$ docker container prune
```

## docker 네트워크 드라이버

```shell
$ docker network ls

$ docker network create application-tier --driver bridge
```