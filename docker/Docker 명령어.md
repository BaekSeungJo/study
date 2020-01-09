### Docker 명령어 ###

1. Docker 이미지 가져오기<br/>
	```docker pull [이미지 이름]:[태그]```
	
2. Docker 이미지 리스트 확인<br/>
``` docker images ```

3. Docker 모든 컨테이너 목록 확인<br/>
``` docker ps -a ```

4. Docker 컨테이너 삭제<br/>
``` docker rm container_id```

5. Docker 컨테이너 실행 
``` docker run -d -p 1521:1521 -p 81:81 -v /Users/baegsungjo/Projects/jpa/db:/opt/h2-data -e H2_OPTIONS='-ifNotExists' --name=MyH2Instance oscarfonts/h2

6. DOcker 컨테이너 재시작<br/>
``` docker restart container_id ```<br/>

* -p : local 포트 : docker 포트 맵핑
* -d : 데몬 모드
* -v : 디렉토리 맵핑
* -e : 환경변수 설정 
* --name : 컨테이너 이름 
	