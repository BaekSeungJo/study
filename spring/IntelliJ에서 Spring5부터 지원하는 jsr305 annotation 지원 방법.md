# IntelliJ에서 Spring5부터 지원하는 jsr305 annotation 지원 방법

1. Preference -> Build, Execution, Deployment -> Complier 선택
2. Add rruntime assertions for nonull-annoted method and parameters checkbox 옆 버튼 클릭
3. 상단이 Nullable annotation, 하단이 NotNull annotation이며 + 버튼으로 intelliJ에서 인식할 annotation을 각각 추가한다.
	* Nullable annotations : org.springframework.lang.Nullable 추가
	* NotNull annotations : org.springframework.lang.NonNull 추가
4. IntelliJ 재부팅