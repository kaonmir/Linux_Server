## tmux 사용하기
* ssh로 서버에 접속한 후 tmux 명령어를 실행한다.
  * 명령어가 없을 시 `pip apt-get install tmux`나 `yum install tmux`를 입력한다.
* 화면이 약간 바뀌는 걸 느낄 수 있다.
* 이 창에서 작업을 하면 네트워크가 끊겨도 다시 접속한 후 `tmux attach`를 입력하면 복구가 가능하다.

### 이외의 기능들
* 모두 tmux를 실행한 후 `ctrl+b`를 누른 후 입력해야 한다. (prefix Key)
#### 탭 열고 닫기
* `d` : tmux 자체를 빠져나온다.
* `c` : GNOME 단말의 새 탭을 연다.
* `n or p` : 탭들을 왔다갔다 한다.
* `커맨드에 exit 명령어 입력` : 탭을 하나 없앤다.
#### 화면 분할하기
* `" 이나 %` : 화면 가로/세로 분할
* `화살표` : 분할한 화면들을 왔다갔다 한다.
* `[` 하고 나서
    * `화살표` : 화면을 스크롤한다.
    * `q` : 스크롤을 종료한다.
* `alt 누르면서 화살표` : 화면 비율을 조작한다.
* `커맨드에 exit 명령어 입력` : 화면 분할을 한 조각을 없앤다.
