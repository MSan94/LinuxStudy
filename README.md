# LinuxStudy
커맨드 툴 공부


# HEAD
- HEAD -N FILE : N줄 까지 보여줘

# tail
- 문서 내용의 뒷부분 출력
- -c : num byte 만 출력
- -n : num line만 출력
- -f : 추가되는 내용 대기. 추가되는 내용은 append 하여 출력
- -F : 파일이 truncate 되는 경우 re-open 하여 follow 함

# wc
- line/word/byte/ count 출력
- -l : 라인수만 출력
```
wc FILENAME
wc -l FILENAME
cat FILENAME | wc -l  // stdin으로부터 라인수만 흭득
wc -l FILENAME | cut -d ' ' -f 1  // 라인수만 흭득
wc -l FILENAME | awk '{ print $1 }' // 라인수만 흭득
wc *.c // 여러 파일 입력 시 합계 출력

```
