# Version_Control_Sysyem
커맨드 라인 인터페이스 방식(Command Line Interface, CLI)을 통한 깃 활용 실습


## 

```console
git
```

다음은 여러가지 상황에서 자주 사용하는 깃 명령입니다:

작업 공간 시작 (참고: git help tutorial)
   clone     저장소를 복제해 새 디렉터리로 가져옵니다
   init      빈 깃 저장소를 만들거나 기존 저장소를 다시 초기화합니다

변경 사항에 대한 작업 (참고: git help everyday)
   add       파일 내용을 인덱스에 추가합니다
   mv        파일, 디렉터리, 심볼릭 링크를 옮기거나 이름을 바꿉니다
   restore   Restore working tree files
   rm        파일을 작업 폴더에서 제거하고 인덱스에서도 제거합니다

커밋 내역과 상태 보기 (참고: git help revisions)
   bisect    이진 탐색으로 버그를 만들어낸 커밋을 찾습니다
   diff      커밋과 커밋 사이, 커밋과 작업 내용 사이 등의 바뀐 점을 봅니다
   grep      패턴과 일치하는 줄을 표시합니다
   log       커밋 기록을 표시합니다
   show      여러가지 종류의 오브젝트를 표시합니다
   status    작업 폴더 상태를 표시합니다

커밋 내역을 키우고, 표시하고, 조작하기
   branch    브랜치를 만들거나, 삭제하거나, 목록을 출력합니다
   commit    바뀐 사항을 저장소에 기록합니다
   merge     여러 개의 개발 내역을 하나로 합칩니다
   rebase    커밋을 다른 베이스 끝의 최상위에서 적용합니다
   reset     현재 HEAD를 지정한 상태로 재설정화합니다
   switch    Switch branches
   tag       태그를 만들거나, 표시하거나, 삭제하거나, GPG 서명을 검증합니다

협동 작업 (참고: git help workflows)
   fetch     다른 저장소에서 오브젝트와 레퍼런스를 다운로드합니다
   pull      다른 저장소 또는 다른 로컬 브랜치에서 가져오거나 통합합니다
   push      원격 레퍼런스 및 그와 관련된 오브젝트를 업데이트합니다

<br/>


### 깃 환경 설정하기
```console
$ git config --global user.name ""
$ git config --global user.email ""
$ git config --global core.editor "vim"
$ git config --global core.pager "cat"
```

`git config` 명령을 통해 사용자 정보를 설정할 수 있으며 `--global` 옵션 추가 시 현재 컴퓨터에 있는 모든 저장소에서 같은 사용자 정보를 사용하도록 설정한다. `git config --list` 로 설정을 확인할 수 있고 수정이 필요할 경우 `vi ~/.gitconfig`을 통해 파일에서 수정이 가능하다.


<br/>

### 깃 저장소 만들기
- 폴더 생성 후 `git init` 
- 생성한 레포지토리 주소 가져오기 `git clone [repo addr] && cd [repo addr]`

### 버전 만들기


