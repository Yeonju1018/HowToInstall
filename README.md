# 🦖터미널에 사용되는 명령어 모음 (for Mac )
많은 명령어가 있고 다양한 옵션이 있지만 아래 내용만 익혀서 사용해도 충분하다.

### 🐍 파일생성 / 파일내용 보기 / 삭제 
- touch file1.txt. ( 빈 내용의 파일 생성 )
- echo 내용 > file2.txt ( '내용' 를 갖고 있는 파일 생성)
- echo 내용추가 >> file2.txt ( 이미 만들어진 파일에 내용을 추가한다 )
- cat  file2.txt ( 파일의 내용보기)
- rm file1.txt ( 파일삭제 )


### 🐳디렉토리 생성 / 이동 / 삭제 
- mkdir \test  ( test 라는 디렉토리 생성 ,  \ 역슬래쉬 ) 
- mkdir \a\b\c ( ~~여러개의 디렉토리를 한꺼번에 만들때 위의 예처럼 역슬래쉬로 시작하면 디렉토리가 만들어 지는 것이 아니라 파일이 만들어진다~~  )
- mkdir /a/b/c ( ~~그래서  슬래쉬 ( / )를 사용해도 만들어지지 않는다~~)
- mkdir -p a/b/c ( **옵션 -p 를 주고  시작디렉토리명 즉, a 앞에 슬래쉬 또는 역슬래쉬를 사용하지 않는다** )
- rm -d 디렉토리  ( 디렉토리 삭제하되 해당 디렉토리안이 비워있어야 한다 ) ( <u>터미널에서 ls -R 입력하면 디렉토리 하위 내용까지 확인가능</u>)
- rm -r 디렉토리 ( 디렉토리안에 내용이 있어도 삭제, 혹시 경고 메시지 나오면 -r 대신 -rf  사용한다 )
- cd 하위디렉토리명 
- cd (1칸 공백) ..  ( 예, cd .. ) 한 단계 상위 디렉토리로 이동
- cd (1칸 공백)- (이전 디렉토리로 이동, 웹브라우저에서의 뒤로가기 버튼처럼, 상위디렉토리로 이동이 아닌 바로 전에 있던 디렉토리로 이동)
- cd ~ ( root 디렉토리로 이동, ~ 앞에 공백 1개 필요하다. 붙어 있으면 cd~ 요렇게 적으면 명령을 찾을 수 없다고 나온다)

### 🐡터미널 내용 지우기 
<u>clear</u>

### 🦕터미널창에서 현재 디렉토리에 뭐가 있는지 궁금할때 
- ls (한 줄로 간단하게 이름들만 보여준다 )
- ls -l ( 여러줄에 걸쳐서 자세한 내용, 작성된 시간까지 보여준다 )
- ls -al ( ls -l 에서는 보이지 않던 숨겨진 내용까지 모두 보여준다 )
- ls -R ( 디렉토리 하위 내용까지 모두 보여준다)

### 🐉현재 터미널에서 보여지는 내용을 파일파인더로 보고 싶다면 
- open(1칸 공백) . 

### 🦭원하는 파일을 찾고 싶다면 
- find . -name '*.js' ( 현재 디렉토리에서 확장자가 js 인 모든 파일을 찾아달라 )
- find / -name '*.js' ( 루트디렉토리에서 부터 확장자가 js 인 모든 파일을 찾아달라 )
- find  ./test -name "fil*". ( /test 디렉토리안의 fil로 시작하는 모든 파일을 찾아달라) 

🌈 아직 작업중입니다. 시간이 될때마다 올릴 예정입니다. 자료는 있지만 정리해서 올리는데 시간이 걸리네요. 
