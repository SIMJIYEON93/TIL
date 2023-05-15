## 23.05.15
## Today I Learned
#  git특강 내용 정리

gitbash(CLI)
pwd : 현재 경로확인하기
ls : 현재경로의 파일 및 폴더조회
ls-a : ls+숨김폴더/파일까지 조회
clear :  화면 깨끗하게 하기
ls-al : ls-a를 리스트형태로 출력하기
* 숨김파일이나 폴더=> .폴더명 or .파일명 되어있음
cd <경로> : <경로>로 이동하기
cd.. : 상위디렉터리로 이동
cd. : 현재디렉터리로 이동 
cd~ : 홈디렉터리로 이동
touch <파일명> : 빈파일 만들기
cat<명령어> : 파일안에 내용출력하기
vi <명령어> : 파일안의 내용을 조작할 수 있는 편집기 
(들어가기 'a' or 'i' , 나가기-> :wq
rm 파일명 : 파일명을 삭제하기
mkdir 디렉터리(폴더)이름 : 비어있는 폴더 생성
rmdir 디렉터리 :  비어있는 디렉터리 삭제
rm- rf : 비어있지 않은 디렉터리 삭제



변경사항= 버
git -> 버전(=commit=유의미한 변화가 결과물로 나온것(ex)새로운 기능 추가, 버그삭제))
관리를 위한도구 
git hub -> 원격저장소호스팅 서비스


$ git config-l : git 설정확인
$ git config --global user.name "이름"
$ git config --global user.email 이메일

git init : 로컬저장소 만들기 (내컴퓨터 안에서 버전이 관리됨)(ex) .git 으로 생김)
git status
git add  
git add <스테이지에 추가할 대상> : <>만 스테이지에 추가 
git add . : 지금까지 변경된 것 모두 스테이지에 추가하는 것
git status
git commit : 자세한 커밋 메시지와 함께 커밋하기
커밋메시지 = 제목(+본문)
<커밋메시지>로 커밋하기
git commit --message "<커밋메시지>"
git commit -m "<커밋메시지>" 
git log : 커밋 목록을 조회하는 명령어
git log --oneline : 커밋목록을 한줄로 간단하게 조회하는 명령어
각각의 커밋에 대한 변경사항 목록 조회하기
git log -p
git log --patch
git diff : 내가 최근에 만든 커밋과 현재 작업디렉터리를 비교한것 
(내가 최근 커밋한 후 한 어떤 작업을 했는 지 보여주는 것)
git diff staged : 스테이지와 커밋를 비교하는 명령어
git diff <커밋해시> <커밋해시> : <커밋>끼리 비교하기
* <커밋해시>는 커밋한 순서대로 해야해
브런치 병합
