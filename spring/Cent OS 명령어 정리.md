### Cent OS 명령어 정리

* 현재 디렉토리 내에서 특정 텍스트 포함한 파일 찾기
	* grep -iRl 'test' ./ 

* 특정 파일 내에서 텍스트 찾기
	* grep 'test' filename 

* 서비스 시작 
	* systemctl start name.service
* 서비스 중지
	* systemctl stop name.service
* 서비스가 구동중이었을 경우에만 재시작
	* systemctl reload name.service
* 서비스 구동 여부 확인
	* systemctl status name.service