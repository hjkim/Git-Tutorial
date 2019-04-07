# First-Time Git Setup

## Git 최초 설정
 Git을 설치하고 나면 Git의 사용 환경을 설정해 주어야 한다. 한번 설정하면 Git을 업그레이드해도 유지된다.
 'git config'라는 도구로 설정 내용을 확인하고 변경할 수 있다. 이때 설정에 사용되는 설정파일은 세 가지이다.
 - **/etc/gitconfig** 파일 : 시스템의 모든 사용자와 모든 저장소에 적용되는 설정이다. *git config --system* 옵션으로 이 파일을 읽고 쓸 수 있다.
 - **~/.gitconfig** 파일 : 특정 사용자에게만 적용되는 설정이다. *git config --global* 옵션으로 이 파일을 읽고 쓸 수 있다.
 - **.git/config** 파일 : Git 디렉토리에 존재하며, 특정 저장소(혹은 현재 작업 중인 프로젝트)에만 적용된다. 각 설정은 역순으로 우선시 된다. 
 즉, *git/config*가 */etc/gitconfig* 보다 우선된다.
 
 ### 사용자 정보
 Git을 설치하고 가장 먼저 해야 하는 것은 사용자 이름과 이메일 주소를 설정하는 것이다. 
 Git은 커밋할 때마다 이 정보를 사용한다. 한 번 커밋한 후에는 정보를 변경할 수 없다.</br>
 
 `git config --global user.naem "Gildong Hong"`</br>
 `git config --global user.email gildonghong@example.com`</br>
 
 다시 말하자면 *--global* 옵션으로 설정한 것은 딱 한 번이면 된다. 해당 시스템에서 해당 사용자가 사용할 때에는 이 정보를 사용한다. 
 만약 프로젝트마다 다른 이름과 메일 주소를 사용하고 싶으면 *--global* 옵션을 빼고 명령을 실행한다.
 
 ## ○ 참고문서
* [시작하기 - Git 최초 설정](https://git-scm.com/book/ko/v1/%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-Git-%EC%B5%9C%EC%B4%88-%EC%84%A4%EC%A0%95)
