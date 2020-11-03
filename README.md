1. http://git-scm.com 에 접속하여 Git-2.27.0-64-bit를 다운로드하여 설치

2. 설치시 두 번째 대화상자의 선택 옵션에서 Use Git from the Windows Command
Orompt를 선택하여 설치.

3. 설치가 끝나면 git bash를 메뉴에서 실행

4. 기본 버전 명령어 : git --version, 도움말 확인 명령어 : git --help

5. github.com 에 접속하여 로그인

6. git bash 에서 프로젝트 폴더를 만듦 
    ex1) cd d:\;
    ex2) mkdir lhw1
    ex3) cd lhw1
    ex4) mkdir test-code
    ex5) ls -al

7. git bash에서 ssh-keygen 명령으로 암호키를 생성 (test-code파일안에서)

8. 내컴퓨터에서 생성된 키젠이 있는 디렉토리로 이동 id_rsa.pub 파일을 찾아 (메모장)열고 복사

9. 로그인 된 github에서 가장 오른쪽 메뉴의 setting을 선택하고, 왼쪽에 SSH and GPG 메뉴 선택

10. SSH keys 항목의 [new SSH Key] 버튼을 눌러 나오는 창에
title : ssh_key_home
key : id_rsa.pub 파일을 찾아 (메모장)열고 복사 한내용을 붙혀넣기 등록

11. 다시 git bash 의 해당 프로젝트 디렉토리 에서
    git config --global user.name [깃허브아이디]
    git config --global user.email [깃허브등록이메일]

12. git bash 의 해당 프로젝트 디렉토리를 초기화 
git init

13. 프로젝트 개발코드 입력하고 저장 README.md 작성

14. git Bash에서 관리목록으로 추가 git add 파일명 또는 git add . (. < 모든 파일 추가)

15. git의 상태 보기( 빨간색은 아직 add하지 않은 것, 초록색은 add한 것) git status

16. 작업한 내용의 메시지를 기록 git commit -m "커밋할 메시지 입력(작업내용)"

17. 원격 저장소 지정 git remote add origin 해당 레포시토리 주소 (https://github.com/hwzzang105/test-code.git)

18. 원격 저장소에 업로드 git ouosh -u origin master

19. 해당하는 아이디나 이메일, 패스워드를 물어볼 경우 입력하면 업로드 성공
