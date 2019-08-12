먼저 Vagrant의 기본 가상화 프로바이더인 VirtualBox를 설치  
https://www.virtualbox.org

Vagrant 설치  
https://www.vagrantup.com/downloads.html

Box 다운로드  
Box란 Vagrant에서 가상 이미지로 사용할 수 있도록 초기 설정된 바이너리  
https://atlas.hashicorp.com/boxes/search


새로운 가상 인스턴스 생성
- mkdir [폴더]: VM 이미지가 위치할 폴더 생성
- vagrant init [이미지] : 초기화
- vagrant up VM 실행
- vagrant half VM poweroff
- vagrant reload : 재기동 Vagrantfile 변경 적용


vagrant 주요command
- vagrant -v : 버전 확인
- vagrant status : 현재 프로젝트의 가상 이미지 상태 요약
- vagrant global-status : 호스트 머신 전체의 Vagrant 가상 이미지들의 상태 확인
- vagrant up : Vagrant 가상 이미지 시작
- vagrant halt : 가상 인스턴스 강제 종료
- vagrant destroy : 가상 이미지 종료 및 기존 이미지 삭제
- vagrant suspend : 가상 인스턴스 실행 상태를 저장하고 종료, 상태 보존
- vagrant resume : 중지된 인스턴스 시작
- vagrant reload : 변경된 VagrantFile 적용
- vagrant ssh : 현재 프로젝트의 가상 이미지에 ssh 접근
