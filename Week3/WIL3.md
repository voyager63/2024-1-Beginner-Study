## <개발 입문 스터디 3주차 WIL>

## 이번주 스터디 목표
commit을 삭제하거나 되돌리는 방법을 알아보자.

### 이번주 학습 키워드
**log, status, amend, reset, revert**

***

1. **log**   
git log 명령을 입력하면 내가 했던 commit 기록을 볼 수 있다. 즉, commit id, commit message 등을 확인할 수 있다. --oneline 옵션을 사용하여 git log --oneline을 입력하면 한 개의 커밋 기록을 한 줄에 볼 수 있다.

2. **status**   
git status 명령을 입력하면 파일의 상태를 확인할 수 있다. 즉, 파일이 add 되지 않아서 untracked 상태인지, add 되었지만 아직 commit은 안 되었는지, 모두 commit하여 더 이상 commit할 파일이 없는지 등을 알 수 있다.

3. **amend**   
git commit 명령의 --amend 옵션의 기능은 내가 마지막으로 한 commit의 내용을 수정하는 것이다. amend하게 되면 새로운 commit으로 대체되기 때문에 commit id가 바뀌게 된다. 기본적으로 commit message를 수정할 수 있으며, --no-edit 옵션을 함께 사용하면 commit message를 수정하지 않고 commit을
수정할 수 있다.

4. **reset**   
git reset 명령은 commit 기록을 제거하는 명령이다. git reset '--option' "commit id" 형식으로 사용하면, commit id를 가진 commit부터 이후 commit을 전부 option에 맞게 변경한다. --soft 옵션을 사용하면 해당 commit id의 commit 부터 이후 commit을 전부 staging area로 옮긴다. add는 되어 있는 상태이기 때문에, commit만 하면 바로 commit 된다. --mixed 옵션은 --option을 입력하지 않았을 때 기본적으로 실행되는 옵션이다. --mixed 옵션을 사용하면 해당 commit id의 commit 부터 이후 commit을 전부 working directory로 옮긴다. 즉 untracted 상태, add 되기 이전 상태가 되는 것이다. --hard 옵션을 사용하면 해당 commit id의 commit 부터 이후 commit을 전부 없애버린다.

5. **revert**   
git revert 명령은 git reset 명령과 달리, commit 기록을 없애지 않고, 되돌리는 명령이다. 되돌리기 때문에 새로운 commit을 만들게 된다. git revert "commit id" 형식으로 사용하게 된다. --no-edit 옵션을 사용하면 편집기를 사용하지 않고 바로 되돌릴 수 있다. --no-commit 옵션을 사용하면, commit하지 않고 revert 내용을 staging area에 올릴 수 있다. reset 같은 경우에는 commit 기록을 완전히 제거해버리기 때문에 다른 사람과 함께 작업하는 공간에서는 사용을 지양해야한다. 반면에 revert는 기록을 제거하지 않고, 변경할 경우 기록을 새로 남기기 때문에 reset보다 안전하다고 할 수 있다.

### 느낀점
오늘은 commit을 다루는 방법을 배웠다. commit할 때마다 계속 내가 원하지 않는 기록이 생기는 것이 불편했는데, 오늘 배운 내용을 응용하면 될 것 같다. 또한 프로젝트 시 다른 사람과 함께 작업을 할 때에는 reset은 위험하다는 것을 기억하자!