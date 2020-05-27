**Git 강의 by.김진현 매니저님**

pwd : 현재 내가 어느 폴더에 위치해있는지

cd test : test 폴더로 가라

git init : git에게 현재 내가 위치한 폴더를 관리할 것을 명령

ls -a : ls 만 입력하면 git같은 파일은 안나타나므로 -a를 추가

git commit->vim 에디터 열리면 들어가서 i 눌러서 입력 후 esc 누른 후 저장하고 나올 때->:wq

git commit --amend : 커밋 텍스트 수정

git log : 내가 그동안 기록했던 것 보여줌

git checkout : 이전 버전으로 돌아가고 싶을 때

git remote add origin url : 현재 위치한 폴더를 원격 저장소(origin)의 master 브랜치에 연결

git push origin master(origin 저장소의 master 브랜치) : 원격의 레포(이름 : origin) 와 로컬의 레포를 연결->내가 로컬에서 커밋한 것을 원격에 업로드

HEAD 파일 : 가장 최신 버전

git add . (git add .a): 새로운 파일 혹은 수정 사항을 모두 추가

<u>**작업을 시작하기 전과 커밋을 한 이후에 이 두 가지 경우에 항상 로컬에서는**</u> 

<u>**git pull origin master를 입력해야 한다->지금 로컬에 있는 저장소의 상태를 원격의 저장소 상태로 최신화**</u>

git commit -m "메시지"->vim 안 열고 짧게 메시지 입력할 때

git clone 데레사 강사님 저장소에서 url 복사 붙여놓기

강사님꺼 올리기 rm -rf .git ->ls -a->git init->git status->git add .->git commit->빔 열리면->메시지 입력->강사님 코드를 훔쳐서 나의 버전1을 만듦->깃허브로 가서 새로운 git st폴더 만들기->2번째꺼 복붙 후->git remote add origin 복사한 거 ->git push origin master



쉬는 시간에 -> pwd ->git pull origin master



##3/20(금) 잔디심기

1. md 작성 후, $ git add .
2. $ git commit -m "add"
3. $ git push

---------------------------

###3/31(화) by.최우영 강사님

* GUI기반의 Shell : internet.exe

* ![image-20200331104237849](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331104237849.png)
  * shell에서 $의 의미 : 이 shell이 사용자의 입력을 받을 준비가 되어 있다는 의미
  * shell에서 ~의 의미 : 내가 로그인되어 있는 폴더의 최상단을 의미

* **git 관련 커맨드**

  * pwd(print working directory) : 나의 위치를 '절대경로'로 보여줌(내가 어디있는지 모르거나 길을 잃었을 때 pwd 입력하면 됨)

  * ls(list segmentation) : 현재 위치에서 아래로 접근할 수 있는 파일과 폴더를 보여줌

  * ls에 옵션을 걸어서 내가 하고 싶은 것의 디테일을 추가할 수 있음

    	* ls -l : 모든 폴더?파일?을 상세하게 보여줌
    	* ls -a : 숨김 파일까지 보여줄 수 있음

  * cd(change directory) : 디렉토리 기준으로 하위로 내려가기 위해서

    ![image-20200331110136180](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331110136180.png)

  * cd .. : 상위 폴더로 올라가기

    ![image-20200331111325849](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331111325849.png)

  * mkdir : make directory ex.mkdir dev : dev라는 디렉토리를 만들었음

  * touch : 새 파일 만들기 ex.touch index.html

  * mv(move) 옮길파일 옮길폴더위치: 파일 이동

    ![image-20200331111532134](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331111532134.png)

  * ../.. : 상위 폴더의 또 상위 폴더로 올라가라

    ​			![image-20200331111711815](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331111711815.png)	

  * cp(copy) 복사할대상 복사할위치: 파일 복사

  * rm 삭제할파일 : 파일 삭제

    * rm index.* : index라는 이름의 파일은 모두 삭제해라
    * rm *.java : java확장자의 파일은 모두 삭제하라mk

  * rm -rf(recursive force) uselss : 그 경로(폴더)의 파일을 모두 지운 후->폴더를 지워야 함

    cf) rm -rf / : 이거 하면 모든 파일이 삭제가 되서 절대 쓰면 안됨

    ![image-20200331114038611](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331114038611.png)

  * 이름 바꾸기

     * 이동을 시키면서 이름을 바꾸는 것 : mv 기존파일 변경파일

       ![image-20200331112654295](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331112654295.png)

  * 이 프로그램으로 이 파일을 열어라 : python3 hello.py / vi hello.txt

* cat 파일 : 텍스트 파일 내의 모든 텍스트를 보여줘라

![image-20200331115106433](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331115106433.png)

----------------------------------

#### Vim

* vim은 텍스트 에디터임

* vi hello.txt : vim에디터 프로그램에서 hello.txt  파일 열기

  * ![image-20200331152304312](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331152304312.png)

  -> 이렇게 해서 들어오면 처음 모드가 normal mode(커맨드 입력)임. 이 외에 insert mode, visual mode 2가지가 더 있음-

  ![image-20200331114334026](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331114334026.png)

  

  위 노말모드에서 입력을 위해 인서트 모드로 들어가야함(i 입력)하면 아래와같이 '끼워넣기'

  ->다시 normal mode(명령어 입력 가능)로 돌아가기 : esc

* ![image-20200331114724700](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331114724700.png)

* normal mode에서 shit+: 누르면 명령어 입력 가능
  * :q! : 버리고 나가기
  * :wq : 저장하고 나가기

-----------------------------------------

####Git

* ![img](https://camo.githubusercontent.com/6101a2b0f170b0a22db8b1077bfa2c6d7fb172bf/68747470733a2f2f692e737461636b2e696d6775722e636f6d2f4d676156392e706e67)

  * workspace : 내 컴퓨터

  * index : stage라고 불림. 이것 덕분에 각각의 커밋들을 임시로 담을 수 있음

    ex. 이사할 때->주방용품 따로, 식품 따로 

  * 인터넷 연결이 안되어 있어도 개발 가능한 이유는 local repository 때문->인터넷 안되는 상태에서 작업한 후 local repository에서 push로 remote repository로 보냄

* git 본격 시작

  * ```
    $ git config --global user.name "username"
    $ git config --global user.email "github email address"
    $ git config --global core.editor "vim"
    $ git config --list
    ```

    -> 송장으로 치면 보내는 사람에 대한 정보를 알려준 것임

* 프로젝트를 git으로 관리하는 2가지 방법

  * git의 시작을 workspace에서 하는 것 : git init
    * 수신인 : remote repository
    * origin : 일종의 별명임
  * git의 시작을 remote repository에서 하는 것

![image-20200331124926900](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331124926900.png)

* 프리픽스 관련 용어
  * docs : documentation

  * conf : configuration

  * feat : feature
  * bugfix:bug-fix
  * resolve : resolved commit related to git.

* 빔에서 작업하기 -> vi README.md

  ![image-20200331141147216](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331141147216.png)

* commit 나누기

  * 시간 순서에 따라 혹은 연관성에 따라

  * ![image-20200331142420533](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331142420533.png)

    -> 빔을 안 열고도 메세지를 입력할 수 있는데, "를 안 닫고 엔터쳐서 꺽쇠가 나오면 그 아래는 추가로 문장을 입력할 수 있는 것

    -> 엔터를 아무리 쳐도 안 닫힘. 닫으려면 "로 마무리



* 2번째 방법 : remote에서 만들기_클론으로

  ![image-20200331144142357](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331144142357.png)

  * git clone 주소(github에서 clone or download로 복사해온.)

  * repository는 항상 병렬적으로 되어 있어야 함. 

    ![image-20200331153622298](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331153622298.png)

* git checkout -- . : 모든 파일에 대해서 최신 상태로 돌아가라

* .gitignore에 commit을 원치 않는 파일 종류들 추가하기

  1) vi .gitignore

  2) i -> #custom 친 다음에 업로드 원치 않는 파일들 입력, 저장 후 나오기PU

  ex. credential/,  index.html / keyfile.pem / server.java / server.py / useless.js

* ![image-20200331152004349](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331152004349.png)



* TIL : 오늘 배웠던 것 정리 및 TODO

* 강사님 깃허브에 있는 걸 내꺼로 가져오기

  ![image-20200331154024555](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331154024555.png)

####블로그 만들기

* hexo라는 시스템 이용해서

* 블로그 만드는 2가지 방법

  1) html로 한땀 한땀 만들기

  2) markdown스타일(정적인 사이트 생성기)로 만든 후->html로 바꾸는 것

* 포스트 다 작성한 후 hexo clear &&hexo generate : 지금까지 만들었떤 파일을 삭제한 후, 그 작업이 끝나면 html파일로 생성해라->그 다음 hexo server 누르기

![image-20200331175044924](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331175044924.png)

![image-20200331175133619](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331175133619.png)

![image-20200331175146771](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200331175146771.png)



* 로컬 파일->git hub에 업로드하기

  (이미 내 로컬 폴더를 git hub에 연결했다는 가정 하에)

  1) touch hello.md

  2) git add .

  3) git commit -m "메세지" 혹은 vi hello.md에서 커밋 메세지 작성

  4) git push origin master



###팀장 레포 포크해오기

* 팀장꺼 포크해 온 후 ->내 레포로 가서 클론을 해 옴 "git clone 주소"->그 다음 cd로 내 컴퓨터에 폴더 생성->오리진이라는 별칭을 팀장의 레포로 사용해야 함. 이를 위해 나의 레포의 별칭을 만들어 줘야 함->git remote add (forked-repo alias) 포크된 레포 url(여기서 소괄호의 내용을 지우고 괄호를 지워야 함. 대신에 내가 원하는 별칭 입력. 포크된 레포 url은 내 레포에서 클론해오는 것임) ex. git remote add jin https://~~ ->git config --list ->이를 통해 팀장과 나의 레포 별칭을 확인할 수 있음. 팀장의 레포에 origin을 부여해야 함-> git remote set-url origin 팀장레포 url (origin 통일)->git config --list
* add 전, push 전에 항상 pull을 해줘야 한다

------------------------

**4/25(토) 올인원 패키지 강의 정리**

* git push origin master : origin이라는 원격 저장소 이름(자유롭게 변경 가능), master(기본 branch의 이름) 것

## 원격 저장소(다른 사람이 만든 저장소) 받아오기(Clone)

1. 원격 저장소 클론

   * git clone 클론해 올 github의 URL : 현재 내 컴퓨터 폴더(test_clone)에 클론해 온 폴더(gittest)를 새롭게 생성함.->내가 원하는 게 아님

     test_clone/gittest

     ![image-20200425102136571](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200425102136571.png)

   * 그런데 위의 방법이 아닌, 현재 내가 위치한 폴더(test_clone) 자체에 클론을 해오고 싶으면 명령어 뒤에 콤마를 붙이면 됨.

     ![image-20200425102426240](C:\Users\haeri\AppData\Roaming\Typora\typora-user-images\image-20200425102426240.png)

2. 클론해 온 폴더 내의 파일 수정 등의 작업
3. git add .
4. git commit -m "메세지 내용 입력"
5. git push origin master