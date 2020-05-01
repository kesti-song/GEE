# GEE를 위한 첫 출발

## 1. 깃이란?
깃은 리누스 토발즈가 개발한 버전관리 소프트웨어이다. 버전관리란 쉽게 말해 프로젝트의 어떤 부분도 겹쳐쓰지 않게 프로젝트의 변경을 관리하는 것이라고 할 수 있다.당신과 동료는 같은 페이지에 각자의 수정사항을 각각 업로드할 수 있고, 깃은 두 개의 복사본을 저장한다. 나중에, 당신들은 그대로 어떤 작업도 잃어버리지 않고 변경사항들을 병합할 수 있다. 깃은 이전에 만들어진 모든 변경사항의 “스냅샷”을 저장하기 때문에 이전 시점의 어떤 버전으로 되돌릴 수도 있다.

## 2. git bash 초기설정과 github에 git 명령어를 통해서 파일 올리기
### git bash 초기설정하기
우선 git bash의 전역 user name과 이메일을 설정해 주어야 한다. 깃허브를 쓰고 있다면 계정 닉네임과 이메일대로 초기화를 해주자.

![닉네임설정](https://github.com/J-hoplin1/J-hoplin1.github.io/blob/master/img/git2/1.PNG?raw=true)

설정이 잘 되었는지 확인해보자.

```
$ git config --global --list
```

![설정확인](https://github.com/J-hoplin1/J-hoplin1.github.io/blob/master/img/git2/2.PNG?raw=true)

### 원격저장소(여기서는 github)와 연동하기
연동하고자 하는 디렉토리(로컬저장소)로 이동하자.

```
$ cd "디렉토리 이름"
```
![로컬저장소로 이동](https://github.com/J-hoplin1/J-hoplin1.github.io/blob/master/img/git2/4.PNG?raw=true)

이제 해당 로컬저장소를 초기화 해준다.
```
$ git init
```
![초기화](https://github.com/J-hoplin1/J-hoplin1.github.io/blob/master/img/git2/5.PNG?raw=true)

테스트로 한번 Readme 파일을 만들어서 commit 해보자. 깃배쉬상에서 파일을 생성하기 위해서는 touch 명령어를 써주어야 한다.

```
$ touch Reame.md
```
![touch](https://github.com/J-hoplin1/J-hoplin1.github.io/blob/master/img/git2/6.PNG?raw=true)

이제 생성한 Readme 파일을 브랜치에 add 해주고 commit을 해주자.

```
$ git add Readme.md
$ git commit -m "New Readme"
```
