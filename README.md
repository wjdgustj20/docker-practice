# docker-practice

## helloworld
Docker로 helloworld 파일 실행하기
1. helloworld 파일 생성
2. Dockerfile 생성
3. Dockerfile 빌드 및 실행
    ```
    $ docker build -t helloworld:latest .
    $ docker run helloworld
    $ docker image ls
    ```
  
## dockerhub
Docker Hub에 Dockerfile 업로드하기
1. Dockerfile 생성(base image)
2. Dockerfile 빌드   
    ```
    $ docker build --tag hyunseojeong/practice:1.0.0 .
    ```
3. Docker Hub에 이미지 업로드
    ```
    $ docker login
    $ docker push hyunseojeong/practice:1.0.0
    ```

## webapp
Docker로 웹 애플리케이션 실행하기
1. 간단한 웹 애플리케이션 파일 app.py 생성
2. Docker 컨테이너에 이미지로 패키징
3. Docker image 빌드 및 실행
    ```
    $ docker push hyunseojeong/practice:1.0.0
    $ docker run -p 5001:5000 flask_test
    $ curl localhost:5001
    $ docker ps
    $ docker inspect flask_test
    ```
    
    
