### PM2 명령어 

1. 앱 시작 명령어<br/>
```pm2 start app.js --name 'app_name' --log-date-format 'YYYY-MM-DD HH:mm:ss.SSS'```

2. 앱 리스트 조회<br/>
``` pm2 list ```

3. 앱 상세 정보 확인<br/>
``` pm2 show app_name ```

4. 앱 중지<br/>
``` pm2 stop app_name ```

5. 중지된 앱 재시작<br/>
``` pm2 restart app_name ``` 

6. 앱 삭제<br/>
``` pm2 delete app_name```
