GDG 개발 입문 스터디 1일차 정리내용
======================================
* 처음세팅
git config --global user.name "UserName"
git config --global user.email "UserEmail"

git init

* 파일등록
git remote add origin "repository address"
git branch -M main
git push -u origin main

* 파일 수정 후 업로드
git add .
git commit -m "commit message"
git push origin main

* 기타
    * Working Directory에서 git add를 통해 staging area에 업로드
    * Staging Area에서 git commit을 통해 Local Repo에 업로드
    * Local Repo에서 git push를 통해 Remote Repo에 업로드 (깃허브)
    * GDG에서는 터미널을 git bash로 열어서 했는데 powershell로 해도 큰 상관이 없다.

* 새 Reop에 올리기
    * git remote remove origin
    * 다시 올릴 땐 파일등록 과정 거치면 됨