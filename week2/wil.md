GDG 개발 입문 스터디 2주차 정리내용
=========================================
Fork, Star, Issue, Branch, Pull Request, Merge에 대해 배움

- Fork
다른 Repo를 나의 Repo로 불러옴. 자유롭게 수정, 업로드 가능, 기존 Repo에 영향을 끼치지 않음

- Star
북마크 개념. 다른 Repo에 Star를 통해 관리할 수 있음

- Issue
Repo에 수정사항이 있을 때 남길 수 있음.
New Issue -> Ttile -> Description을 작성하면 제목이 title이고 description이 내용인 issue가 작성됨
Issue는 새로 만들어질 때마다 자동으로 번호가 부여됨.

- Branch
기존 Repo에 문제가 있을 때 Branch를 통해 수정할 수 있음.
Branch는 기존 Repo에서 한 가지를 만들어내어 코드를 수정한 후 다시 기존 Repo에 붙이는 시스템?
main stream의 한 갈래로 Branch를 만든 후 코드를 수정하여 다시 main stream에 넣어줌.
한강 본류가 main stream이고 당산동쯤 와서 코드가 이상한 것을 알고 샛강 통해 branch를 만들어 수정한 후 노량진쯤에서 다시 합류

-- 현재 열려있는 branch 확인
git branch

-- branch 생성
git branch "<브랜치 이름>"

-- branch 이동
git checkout <브랜치 이름>
ddddd
-- branch push
git push origin <브랜치 이름>

--> 이후 branch를 main과 merge 시켜야함
Merge commit
브랜치와 main을을 공통으로 부모로 삼는 새 브랜치를 만듦.
branch 내에서의 commit이 있을 경우 main 브랜치로 병합됨.
Squash and Merge
Branch 내의 commit을 하나로 통합해 main 브랜치로 병합함.

git push origin main
