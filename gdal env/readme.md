* 사용법


1. 도커 파일을 이용해 도커 이미지를 만든다
docker build --tag gdal_env

2. 도커 컴포즈 파일 실행 시킨다
docker-compose up -d

3. volume에 타일링 시킬 tif 파일을 옮긴다

4. 도커 컨테이너 내부에 접속해서 타일링 명령어를 실행시킨다
docker exec -it gdal_env /bin/bash
cd /home/ubuntu/volume

5. 타일링 된 결과물은 volume 폴더에 생성된다.

