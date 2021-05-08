GitHub repository URL : 

# Git & Github 사용법

## 1. Github 사용을 위한 사전 지식  
### (1) 커밋(commit)과 푸시(push)
- 커밋 (commit) : 파일을 추가하거나 변경 내용을 저장소에 저장하는 작업
- 푸시 (push) : 파일을 추가하거나 변경 내용을 원격 저장소에 업로드하는 작업  

### (2) 로컬 저장소와 원격 저장소
- 로컬 저장소 : 자신의 컴퓨터에 있는 파일이나 디렉토리를 저장하는 장소
- 원격 저장소 : 서버등 네트워크에 있는 파일이나 디렉토리를 저장하는 장소, 기본적으로 로컬 저장소에서 작업을 수행하고 그 결과를 원격 저장소에 저장함, 다른 사람들과 공유 가능

### (3) 브랜치 (branch)
- 소프트웨어의 여러 버전 관리 기능
- 하나의 프로젝트를 여러 갈래로 나누어 관리 가능함
- 일종의 독립된 작업을 진행하기 위한 작업 공간  
![브랜치 설명](branches.png)

### (4) Git의 3가지 상태
- Committed : 로컬 저장소에 데이터가 안전하게 저장됨
- Modified : 아직 로컬 저장소에 수정한 파일을 커밋하지 않음
- Staged : 현재 수정한 파일을 곧 커밋할 것임을 의미함


## 2. Github 사용법  
### (1) Git 다운로드  
- Git SCM 접속 후 운영체제에 맞는 설치 파일 다운로드
- Git SCM URL : https://git-scm.com/  

### (2) Git Bash에서 깃 버전 확인
    git --version
![verson](verson.png)

### (3) Git 사용자 등록 및 확인
- Git 설치 후, 사용 환경 설정 필요
- git config 명령어로 이름, 이메일 설정하고 변경 가능  

      git config --global user.name "name"
      git config --global user.email "email address"
![name](name.png)
- 프로젝트 마다 다른 설정 원한다면, --global 빼기  

      git config --list
![config](config.png)
- 사용자 확인 가능

## 3. Git 저장소 생성
- 첫번 째 방법 : 버전 관리를 하지 않는 로컬 저장소를 Git 저장소로 활용
- 두번 째 방법 : 다른 곳에서 Git 저장소를 Clone하여 활용  

### (1-1) 로컬 저장소로 활용할 폴더 생성
![newfile](newfile.png)
- GitHub_ch 폴더 생성

### (1-2) 해당 폴더로 위치 이동
- cd 명령어 사용  

      cd [로컬 저장소 경로]
![cd](cd.png)

- 마우스 우클릭으로 Git Bash Here 실행
![newfile2](newfile2.png)

### (1-3) Git 원격 저장소 생성
- 버전 관리를 하지 않는 기존 프로젝트를 Git으로 관리하기 위해 위의 과정을 거쳐 프로젝트의 디렉토리로 이동한 상태
- git init 명령어 실행
- 버전 관리를 하고 싶은 폴더에서 초기화 상태로 만드는 준비를 하는 명령어
- 현재 디렉토리 기준 .git이라는 하위 디렉토리 Git 저장소 생성  

      git init
![init](init.png)

------------
### (2-1) 복제할 원격 저장소 clone 주소 복사
### (2-2) git clone 명령어 사용
- (1) 번은 버전관리를 하지 않는 기존 프로젝트를 Git으로 관리하는 방법, 이 방법은 기존 저장소를 복사하는 방법
- 다른 프로젝트에 참여 혹은 Git 저장소를 복사할 때 사용
- 로컬 저장소, Github에 있던 원격 저장소를 복사 가능  

      git clone [URL]
![clone](clone.png)

## 4. Git 명령어
#
