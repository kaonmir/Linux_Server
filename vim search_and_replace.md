# 문자열 검색, 바꾸기
#### 기본형 : `:(range)s/src/dst/option`
* range
    * 공백 : 현재 줄을 검색한다.
    * % : 모든 줄을 검사한다.
    * 1, $ : 1번 줄부터 끝 줄까지 검색한다.
    * ., 10: 현재 줄부터 10번 줄까지 검색한다.
    * ., +2: 현재 줄부터 다음 두 줄까지 검색한다.
    * g/^baz: baz로 시작하는 모든 줄을 검색한다.
* s : s는 subtitute한다는 명령어이다.
* src : 찾을 문자열
    * 찾을 문자열을 입력하면 된다.
    * [정규식](https://github.com/kaonmir/Linux_Server/blob/master/%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D.md)을 사용할 수도 있다.
* dst : 바꿀 문자열
    * 바꿀 문자열을 입력하면 된다.
* option
    * g : 범위 내의 모든 문자를 찾는다. (적지 않을 시 한 번만 찾고 종료한다)
    * c : 물어 보고 명령을 실행한다. (y: 실행, n: 다음, a: 모두 바꾼다, q: 종료, l: y+q)
      * **문자를 바꾸지 않으면 검색하는 기능이 된다!**
    * i : 대소문자 구별하지 않는다.    
* 참고 사이트
    * https://vim.fandom.com/wiki/Search_and_replace
    
