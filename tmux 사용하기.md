## tmux 사용하기
* ssh로 서버에 접속한 후 tmux 명령어를 실행한다.
  * 명령어가 없을 시 `pip apt-get install tmux`나 `yum install tmux`를 입력한다.
* 화면이 약간 바뀌는 걸 느낄 수 있다.
* 이 창에서 작업을 하면 네트워크가 끊겨도 다시 접속한 후 `tmux attach`를 입력하면 복구가 가능하다.

### 이외의 기능들
* 모두 tmux를 실행한 후 `ctrl+b`를 누른 후 입력해야 한다. (prefix Key)
  * `d` : tmux 자체를 빠져나온다.
  * `c` : GNOME 단말의 새 탭을 연다.
  * `n or p` : 탭들을 왔다갔다 한다.
  
