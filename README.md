# 📁 Git Repository
> - ### git이 관리하는 파일이나 폴더를 저장하는 장소   
> - ### 파일을 수정, 커밋하고 프로젝트의 버전을 관리하는 git의 공간   
> - ### 하위에 '.git' 디렉토리가 존재하는 디렉토리
<br/>

- #### 원격 저장소
	  원격으로 저장되어 있는 복제 가능한 저장소를 말함 (협업 프로젝트 원본을 저장하는 저장소)
- #### 로컬 저장소
	  내 PC의 '.git' 디렉토리가 존재하는 디렉토리
  	  (git 저장소로 지정했거나 원격 저장소의 작업물을 복제해오는 저장소)
    
   
   
# 📋 Git 관리 공간

- ### Working Directory (= Work Tree)
	  내가 작업할 프로젝트 디렉토리, 즉 내 로컬 저장소를 말함
- ### Staging Area (= Index)
	  파일이 수정된 후 추가되었지만 커밋은 되지 않은 파일들이 존재하는 가상공간
 
	  git 파일이 원격 저장소에 저장되는 과정은 [수정 ▶ 추가 (= 등록 = stage = 스테이징) ▶ 커밋]
  
	  Staging Area는 가상 공간이므로 파일이 이 공간에 있더라도 실제로는 로컬 저장소에 존재함.
  	  즉 실수를 방지하기 위한 공간
- ### Git Repository (= Repository)
	  커밋한 파일들이 저장되는 공간
 
 	  협업 프로젝트의 작업물 공유 목적이나 작업물 백업 용도로 사용하는 공간
----
# 📖 Git 명령어

- #### 로컬 저장소 초기화
	  git init
+ #### 현재 상태 확인
  	  git status
* #### 새로운 파일을 Staging Area에 추가
	  git add
  	  git add . (로컬 저장소 내의 모든 파일을 추가)
- #### Staging Area의 파일을 commit
	  git commit -m "Write Any Comment"
- #### commit한 파일을 원격 저장소에 업로드
	  git push origin main
  	  git push -u origin main (로컬 저장소와 원격 저장소를 연동시킴)
