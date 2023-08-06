# linux part 2

## 리눅스 기본 명령어

### man
* 기본 형식
    * man <옵션> <키원드>

옵션|옵션 설명
--|--|
-k|메뉴얼 목록을 검색
-s|입력한 섹션에서 매뉴얼 검색해서 출력
|(1)User Commands
|(2)System Calls
|(3)Subroutines
|(4)Devices
|(5)File Formats
space|next page
enter|next line
b|backward
q|quit

### ls
* ls <옵션> <파일|디렉토리>
* 특정 디렉토리 안의 파일 목록을 출력

옵션|옵션 설명
--|--|
-a|dot(.)로 시작하는 숨겨진 파일까지모두
-l|파일/디렉토리의 자세의 저보
-R|하위 디렉토리까지 모두 출력
-d|디렉토리 자체를 출력

색갈|설명
--|--|
청록색| 심볼링 링크
초록색| 실행이 가능한 파일
빨강색| 특별한 퍼미션 파일
파란색| 폴더

### mkdir
* mkdir <옵션> <디렉토리_이름>
* 디렉토리를 생성

옵션|설명
--|--|
-m|퍼미션 설정
-p|존재하지 않는 parent directories생성

### rmdir
* rmdir <옵션> <디렉토리_이름>
* empty 디렉토리를 삭제

옵션|설명
--|--|
-p|비어있는 parent directories를 함께 삭제

### cd
* cd <디렉토리명>
* 특정 디렉토리로 이동하는 명령

옵션|설명
--|--|
~|home 디렉토리로 이동
-|Previous directory로 이동

### cp
* cp <옵션> 원본파일이름 목적지파일이름
* 원본파일을 현재 또는 다른 디렉토리에 목적지파일이름으로 복사

옵션|설명
--|--|
-i|복사할 때 overwrite 할것인지 질문
-f|복사할 때 overwrite 질문없이 무조건 덮어쓰기
-r|디렉토리 복사

### mv
* mv <옵션> 원본파일이름 새이름
* 파일의 이름을 바꾸거나 다른 디렉토리로 이동

옵션|설명
--|--|
-i|이름을 바꿀 때 overwrite 할 것인지 질문
-f|이름을 바꿀 때 overwrite 질문없이 무조건 덮어쓰기
