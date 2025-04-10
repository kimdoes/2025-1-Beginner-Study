## <p style="text-align:center;">개발 입문 스터디 Quiz 1</p>

#### Example
개발 입문 스터디는 무슨 요일인지 적으시오.

- 답: 금요일

### Q1
Git에서 파일의 상태는 크게 untracked와 tracked로 나눌 수 있다.  
그렇다면 tracked에는 어떤 상태가 있는지 모두 적으시오.

- 답: Unmodified, Modified, Staged

### Q2
Git에는 세 가지 영역이 있다.  
세 가지 영역을 모두 나열하시오.

- 답: Staging Area / Local Repo / Remote Repo

### Q3
현재 우리는 ```main```브랜치에 있다.  
```develop```이라는 브랜치를 새로 만들고 이동까지 한번에 할 수 있는 명령어를 적으시오.

- 답: git checkout -b <branchname>

### Q4
Working Directory에 있는 파일들을 모두 Staging Area에 추가할 수 있는 명령어를 적으시오.

- 답: git add .

### Q5
```
1. Create a merge commit
2. Squash and merge
3. Rebase and merge
```
위의 세 가지가 어떤 차이가 있는지 간단히 적으시오.

- 답:
Create a merge commit은 main에 branch와 main을 모두 부모로하는 새 commit을 만든다. branch에 저장된 commit들이 모두 기록에 남는다.
Squash and merge는 branch의 commit들을 모두 합친(Squash) 뒤 main에 병합한다. branch에 기록된 commit은 하나로 합쳐진다.
Rebase and merge는 branch의 commit들이 모두 main으로 합쳐진다.

### Q6
```git log --oneline```으로 commit의 기록을 확인해보니  
첫 줄에 ```a1s2d3f (HEAD -> develop) docs: readme 추가```라는 log가 찍혔다.
알 수 있는 사실을 모두 적으시오.

- 답:
commit ID가 a1s2d3f로 시작한다.
develop 브랜치에서 파일을 "docs: reame 추가"라는 commit 메시지를 통해 commit 했다.

### Q7
```git log --oneline```으로 commit의 기록을 확인해보니 아래와 같은 log를 확인 할 수 있었다.  
```
a1s2d3f (HEAD -> develop) fifth commit
s2d3f4g fourth commit
345hj26 third commit
7g8dg7f second commit
5g568vk first commit
```
이때, fourth commit까지 제거하고 fourth commit과 fifth commit의 변경 사항은
Staging Area에 남아 있길 바란다면 reset을 어떤 옵션과 함께 사용하면 되는지 적으시오.

- 답: git reset --soft 345hj26
hi!
### Q8
```git log --oneline```으로 commit의 기록을 확인해보니 아래와 같은 log를 확인 할 수 있었다.
```
a1s2d3f (HEAD -> develop) fifth commit
s2d3f4g fourth commit
345hj26 third commit
7g8dg7f second commit
5g568vk first commit
```
reset은 너무 위험하니 revert를 사용하려고 하여 ```fifth commit```을 되돌리고 싶다면 
어떤 명령어를 사용하면 되는지 적으시오. 

- 답: git revert a1s2d3f

### Q9
여러 사람이 협업하는 프로젝트에서 커밋을 되돌려야 한다.  
reset과 revert 중에 어떤 것을 선택할 것인지를 그 이유와 함께 적으시오.

- 답: revert
reset를 선택하면 협업 중인 github에서는 변경사항이 생기지만 상대의 local workspace에 변경사항이 적용되지 않아 충돌을 일으킬 수 있기 때문이다.