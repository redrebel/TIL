File encoding 확인
: file -bi tmp.txt

(mac에서는 file -I tmp.txt)

현재 파일 밑에서 특정 텍스트를 포함한 파일찾기
grep -R "yield" ./
mdfind -onlyin ./ "ye"
