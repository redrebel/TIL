어노테이션
@EnableBatchProcessing : Spring Batch 기능 활성화 어노테이션. Job 생성에 필요한 핀들을 자동으로 가져온다.



[spring initializr](https://start.spring.io/)에서 H2를 Dependency 선언을 한 후
소스내에서 org.h2.server.web.WebServlet 를 import 하려고 하면 안되는 경우가 있다.

이럴땐 혹시 dependencies 에서 h2 가 compile 로 되어 있는지 확인한다.
default 가 runtimeOnly 이기 때문에 생기는 현상이다.
이런 경우 compile 로 바꾸면 된다.




http://yookeun.github.io/java/2015/06/19/mybatis-batch/
가급적 배치처리에는 Mybatis의 foreach를 사용하는 것이 훨씬 효율적이다.
