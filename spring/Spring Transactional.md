### Spring Transactional

1. @Transactional annotation
	* readOnly : 해당 트랙잭션은 읽기 기능만 수행한다. 
	* readOnly을 true로 설정하고 JPA Hibernate 구현체를 사용할 경우 Flush 모드를 NEVER로 설정하여 PersistenceContext가 Dirty checking을 하지 않아 성능 향상이 된다. 
	* Flush 모드가 NEVER일 경우는 PersistenceContext가 관리하는 데이터의 변경을 관리할 필요가 없을때이며, 따라서 데이터 동기화를 할 필요가 없다. (데이터를 조회만 하는 경우 동기화 불필요) 
	* Flush 모드는 PersistenceContext가 DB와 언제 Sync를 맞출지를 설정하는 옵션이다.
	* Flush 모드의 기본값은 commit할때, 데이터를 읽어올때 Sync를 맞춘다. 
	* 보통 Transactional은 Service 계층에 달며, Repository 계층에 붙이는 것도 좋은 습관이다. (readOnly가 true일 경우 다는게 좋음)