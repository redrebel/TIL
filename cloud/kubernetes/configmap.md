Application 이 사용하는 설정값들을 소스에 하드코딩하거나 이미지안에 넣는게 아니라 kubernetes에 master Node애 configmap을 만들어서 배포(deploy)시 전달되어 Application이 시작할때 참조하여 실행되도록 할 수 있다.

configmap을 생성한다.  
`kubectl create configmap logger --from-literal=log_level=debug`

모든 configmap list 을 확인한다.
`kubectl get configmaps`

configmap의 logger라는 이름의 설정값을 확인한다.
`kubectl get configmap/logger -o yaml`

설정값을 수정 할 수 있다.
`kubectl edit configmap/logger`
