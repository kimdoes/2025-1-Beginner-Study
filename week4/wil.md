GDG 개발 입문 스터디 4주차 정리내용
=========================================
Git flow

브랜치 종류
- Main
-- main(master) / develop
main이 배포되는 곳곳, develop은 개발한 것이 적용되는 곳
영원히 남는다. 삭제되지 않는한!

- Support
-- feature / release / hotfix
feature - develop에서 분기되어 작성됨. 기능개발하는 브랜치. 브랜치명은 위에 나온 브랜치명 빼고 거의 다 가능함
release - 배포 전 버그를 확인함. develop에서 분기하고 main과 develop으로 병합됨
hotfix - main에서 급하게 수정해야할 사항이 있을 경우 main에서 분기, 이후 develop과 main에 동시 병합

============================================

Github flow
Git flow의 경우 main - develop - feature - release - main이라는 복잡한 과정 때문에 등장한 간결화된 브랜치 흐름

- Main
- feature (수정사항이 있을 경우 여기서 수정 후 main에 병합) 만 사용

convention과 질문이 중요하다!