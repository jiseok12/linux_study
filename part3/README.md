# linux part 3
## vi 리눅스 편집기

### 리눅스으 편집기 종류
* vi, vim, emacs, nano 등

### vim 에디터는
* 1976년 빌조이가 초기 BSD 릴리즈에 포함될 편집기로 만들어 현재까지 리눅스에서 가장 많이 사용되는 에디터
* 리눅스 버젼 뿐만 아니라 윈도우 버전도 존재

### vi 편집기 사용법
* vi <파일이름>
* command mode (진입시 처음으로 들어가는 모드)
    * 커맨드만 입력할수 있다
* u 저장 전단계 이동
* . 이전 command 사용  
* p 붂여 넣기
* #<-숫자 입력

~|화면이동키|삭제|복사|치환
--|--|--|--|--|
글자|~|#x|#y|#r
단어|#w,b|#dw|#yw|#cw
문장전체|~|#dd|yy|cc,R
문단의 시작|^|d^|y^|c^
문단의 끝|$|D,d$|u$|c$
파일의 끝|G|dG|



* ex mode
    * :, \,? 키로 진입
    * :e! 편집을 취소 한다
    * :w 저장하기
    * :w <새파일 이름> 현재 파일을 새이름으로 저장
    * :q 종료
    * :q! 강제 종료
    * :r <끼워 넣을 파일> 편집중인 파일에 다름파일을 끼워넣기
    * /<검색할 문자열> 찾기
    * :%s/찾을문자열/변경할문자열/g 찾아서 바꾸기
    * set number 줄 번호 표시
    * set ts=# 원하는 만큼 탭을 뛰운다
* input mode
    * (command mode에서 a,i,o,A,I,O 키로 진입)
    * ESC키 input mode -> command mode
    * o키 command mode(open new line)
    * a키 command mode(append INSERT)
    * i키 command mode(INSERT)
    * A키 문장의 제일 끝 에서 시작
    * I키 문단의 첫번째에서 입력
    * O키 위로 세로운줄을 생성 한다

* ~/.vimrc
    * vi 의 초기 설정을 할수 이다

### 파일 만들기
* echo "내용 입력" > filename
* cat > filename
    * 내용 입력 <ctrl>+<d>