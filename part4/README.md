# linux part 4
## linux wildcard 문자 사용하기

### Filename Matching
* 많은 command들이 파일이름을 argument로 사용
* Wildcard patterns은 여러 개의 파일이름을 쉽게 표현할 수 있게 지원
* Special Characters: *,?,[]

### Wildcard Patterns
* ? Matches any single character 문자 한개중
* *Matches anything(any number of characters) 모든 문자 중
* [..] character classes []안의 문자중
* ex) ls test? test라는 문자 뒤에 한문자 아무거나 있는 파일 출력
### Brace({})확장
* 문자열 생성 허용
* 와일드 카드와 유사하지만 대상 파일 또는 디렉토리가 존재할 필요는 없음
* ex) mkdir {hello, how}