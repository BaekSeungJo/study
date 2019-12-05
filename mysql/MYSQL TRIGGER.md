### MYSQL TRIGGER

1. DB 해당 스키마에 존재하는 TRIGGER 조회<br/>
```show triggers```<br/>

2. DB 해당 스키마에 존재하는 특정 트리거 생성 쿼리 조회<br/>
```show create trigger trigger_name```<br/>

3. DB 해당 스키마에 존재하는 특정 트리거 삭제 쿼리<br/>
```show drop trigger trigger_name```<br/>

4. TRIGGER는 DB 테이블에 INSERT, UPDATE, DELETE 쿼리 수행 전(BEFORE), 수행 후(AFTER)에 테이블 하나당 하나씩 생성할 수 있다.<br/>
```BEFORE INSERT ON TABLE_NAME```<br/>
```AFTER INSERT ON TABLE_NAME```<br/> 

5. INSERT, UPDATE 트리거에서는 new로 추가 또는 수정되는 row에 대한 정보를 받아 올 수 있으며, DELETE 트리거에서는 old로 삭제되는 row에 대한 정보를 받아 올 수 있다.<br/>

6. 쿼리 샘플<br/>
```CREATE DEFINER=`username`@`ip` TRIGGER `trigger_name` BEFORE DELETE ON `target_table_name`
 FOR EACH ROW Insert INTO `table_name` (`field`, `field`, `field`) VALUES (old.target_table_field, 'field', old.target_table_fild)```<br/><br/>
 
 
 ```CREATE DEFINER=`username`@`ip` TRIGGER `trigger_name` AFTER INSERT ON `target_table_name`
 FOR EACH ROW Insert INTO `table_name` (`field`, `field`) VALUES (new.target_table_field, 'field')```</br>


	
	