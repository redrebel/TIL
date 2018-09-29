Go언어로 구현되어있음.

Pod 는 쿠버네티스에서 가장 기본적인 배포 단위로, 컨테이너를 포함하는 단위이다.

쿠버네티스의 특징중의 하나는 컨테이너를 개별적으로 하나씩 배포하는 것이 아니라 Pod 라는 단위로 배포하는데, Pod는 하나 이상의 컨테이너를 포함한다.


Kubernetes는 kubectl run, expose, scale 명령으로 바로 사용할 수 있는 간편한 워크플로를 지원합니다.

cluster -->


start
$kubectl apply -f [yml files]

stop
$kubectl delete -f [yml files]



개발팀이 개발과 시스템에 대한 배포/운영을 담당한다면, 데브옵스팀은 개발팀이 이를 쉽게할 수 있는 아랫단의 플랫폼과 자동화를 하는데 목표를 두는 역할로 역할이 명확해지고 있다.

사이드카 패턴(Side car pattern) :
마이크로 서비스 아키텍쳐에서 애플리케이션과 애플리케이션에서 사용하는 주변 프로그램을 같이 배포하는 패턴
https://kubernetes.io/blog/2015/06/the-distributed-system-toolkit-patterns/


2. 컨테이너 딜리버리 파이프라인 : 코드 체크인의 빌드/테스트 주기를 자동화하고 컨테이너 오케스트레이션 시스템에 성공적인 체크인을 배치하는 스시템이다.

구성 관리 시스템은 컨테이너 오케스트레이션 시스템, 컨테이너 딜리버리
파이프라인과 같은 핵심 분산 시스템, 그리고 컨테이너에서 실행되지 않는 데이터 관리 시스템 등의 기타 종속성을 배치하고 라이프 사이클을 관리하는 데 사용된다.

로그 집계 시스템은 컨테이너 오케스트레이션 시스템과 컨테이너 딜리
버리 파이프라인에서 오는 로그를 배출하는 기능을 수행함으로써 계속해서 감사, 포렌식, 예측 분석을 위한 중요한 기능을 제공한다.

모니터링 시스템은 컨테이너 오케스트레이션 시스템에서 나오는 데이터와 다른 외부 데이터 소스를종합한다.

폴 루벤스는 “컨테이너는 소프트웨어를 다른 컴퓨팅 환경으로 옮겨서도 안정
적으로 실행하는 방법을 제시하는 솔루션이다. 컨테이너는 애플리케이션과 모든 종속성, 라이브러리 및 기타 실행에 필요한 바이너리와 구성 파일을 하나의 패키지로 묶은 전체 런타임 환경으로 구성된다”

### Spring cloud Sleuth - Logging
Spring Cloud에서 제공하는 Distributed Tracing 솔루션
- 대부분의 내외부 호출 구간에서 Trace    정보를 생성 및 전달
- Log에 남기거나 수집 서버(Zipkin)에 전송하여 검색/시각화

Spring Cloud Sleuth가 지원하는 Component?
- Zuul, Servlet, RestTemplate, Hystrix, Feign, RxJava

 Spring Cloud Sleuth 사용시 Appliction 로그에 Trace ID(UUID)가 함께 출력
 Trace ID - 하나의 Request에 대해 서버 전체를 걸쳐 동일한 UUID


 Spring Cloud Sleuth with zipkin

### kubernetes Dashboard
https://github.com/kubernetes/dashboard#kubernetes-dashboard   
http://blog.cjred.net/entry/kubernetes-Dashboard-%EC%84%A4%EC%B9%98%EC%99%80-%EB%A1%9C%EA%B7%B8%EC%9D%B8

### Heptio Contour (ingress 서비스)
`kubectl apply -f https://j.hept.io/contour-deployment-rbac`

### Fluentd
Logging


### gcloud console command
$ gcloud container clusters get-credentials cluster-1 --zone us-central1-a

gcloud container clusters list
