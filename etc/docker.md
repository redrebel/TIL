## MACOS 기준

docker == container

### DOWNLOAD
1. https://docs.docker.com/docker-for-mac/#download-docker-for-mac 접속
2. Download Docker for Mac > Stable channel > Get Docket for Mac(stable) 클릭
3. 설치 & 실행
4. 설치가 잘 됐는지 확인
  ```
  $ docker --version

	$ docker-compose --version

	$ docker-machine --version

  $ docker info

  $ docker run hello-world
  ```
5. 원하는 도커이미지 검색 & 설치
  ```
  $ docker search [keywork]

  $ docker pull [image name]
  ```
6. 이미지를 확인 & 컨테이너로 생성
  ```
  $ docker images

  $ docker run [옵션]
  ```
7. 컨테이너 중지 & 재실행
  ```
  $ docker stop [container name]

  $ docker start [container name]
  ```
8. 실행중인 컨터이너에 접속
  ```
  $ docker attach [container name]
  또는
  $ docker exec -ti [container name] bash
  ```

9. 출력로그보기
  ```
  $ docker logs [container name]
  ```

https://nolboo.kim/blog/2016/08/02/docker-for-mac/

1. docker가 실행될때 자동으로 컨테이너가 실행되게 하기
```
# 자동실행
docker update --restart always [container name]
# 자동실행 제거
docker update --restart always [container name]
```

1. Dockerfile
  This is a small "program" to create an image.
  `docker build -t [name-of-result]`.
  
