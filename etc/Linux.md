File encoding 확인
: file -bi tmp.txt

(mac에서는 file -I tmp.txt)

현재 파일 밑에서 특정 텍스트를 포함한 파일찾기
$ grep -R "yield" ./
$ mdfind -onlyin ./ "ye"

### 메모리 확인
$ cat /proc/meminfo | grep Mem

### 어디있는지 찾는...
$ which ...

### zsh 사용환경 구성
$ chsh -s `which zsh`  # 현재 쉘을 zsh 쉘로 바꿈
$ chsh -s /bin/zsh     # 위의 명령어와 동일함
테미널 다시 시작
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"  # oh my zsh 다운로드
