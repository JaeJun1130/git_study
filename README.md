# ==stage / repository==
 - stage -> 커밋 대기파일이 가는곳
 - repository -> 커밋이 된 결과물들이 가는곳

# ==git command==

## git init -> git 시작

## git status -> git 상태 확인

## git add -> 파일 수정 이력 기록 준비

## git commit -> 파일 수정 이력 기록

## git log -> commit 이력보기
 - commit 시점 되돌리는 방법
 - 1. git reset --hard [487d25738c85da9a044a873bb9ec2ee2a198b05b] -> git commit 시점 되돌리기
 - 2. git revert 
 - git log --decorate --all --graph --oneline -> git log 그래프 한줄 이쁘게 출력

## git remote add origin [] -> git repository 랑 연결

## git branch jaejun -> git branch 생성
  - git branch -d [] 필요없는 브런치 삭제
## git swich jaejun - > git branch 이동 (git checkout jaejun)

## git tag -a 1.0 -m "first release" master -> master tag 생성

## git rebase
- 1. main 또는 master에가서 git pull origin master 최신화 pull
- 2. feature로 돌아가서 rebase 시작 git rebase -i master
- 3. commit 한 갯수 만큼 pick 생성, 1차 pick은 그대로 두고 그 외 rebase 할 pick은 s (squash) 로 변경
- 4. commit msg 병합화면으로 자동으로 이동됨, 그 후 commit를 하나로 병합 해도 되고 수정해도 됨
- 5. branch로 push -f 강제 푸시 명령어 필수
- rebase 충돌시
- 1. git add .
- 2. git rebase --continue
- 해결안될시
- 3. git rebase --abort로 아에 rebase를 진행하기 전 상황으로 돌아감
# ==git flow==
main
|
develop
|
feature
|
release
|
hotfix

main - develop - feature - develop - release - main - hotfix - main ~~

# ==linux command==

ls -al 숨김파일까지 리스트형태로 다보기
touch [] 0바이트 파일생성
vim [] 파일생성




