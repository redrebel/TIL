http://epicdevs.com/17

A high-throughput distributed messaging system.

LinkedIn 에서 개발된 분산 메시징 시스템
클러스터 내의 broker에 대한 분산 처리는 Apache Zookeeper가 담당.

기존 메시지 시스템(ActiveMQ, RabbitMQ)과의 차이점
- 대용량의 실시간 로그 처리에 특화
- 분산 시스템을 기본으로 설계
- producer가 broker에게 다시의 메시지를 전송할때 batch처리로 효율
- 메시지를 기본적으로 파일시스템에 저장(기존 메시지 시스템은 메모리)
- 
