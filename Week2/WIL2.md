## <개발 입문 스터디 2주차 WIL>

## 이번주 스터디 목표
issue, branch, pull request, merge의 기능을 알아보자.

### 이번주 학습 키워드
**issue, branch, pull request, merge**

***

1. **issue**   
issue는 협업 시, 레포지토리의 변경사항을 기록할 수 있는 기능이다. 한마디로 프로젝트를 진행하면서 생기는 문제, issue들을 기록하여, 협업하는 개발자들에게 그 문제를 알려줄 수 있는 편리한 기능이라고 보면 된다.

2. **branch**   
branch는 프로젝트 시 사용하게되는 개별 작업 공간이라고 할 수 있다. 주로 main branch가 주 branch가 된다. 프로젝트를 하면서 기능을 추가하거나, 새로운 기능을 구현하는 등의 작업을 할 때, 새로운 branch를 파서 그 곳에서 작업을 하면 작업의 분리가 가능해져서 편리하다. branch를 여러개 만들어서 여러 단계의 작업을 분류할 수 있게 된다.

3. **pull request**   
프로젝트에서 추가적인 작업을 할 때, 새로운 임시 branch에서 따로 작업을 한 뒤, 그 작업한 것을 main branch로 옮기기 전에 commit, push를 하게 된다. pull request는 merge전에 자신이 push한 내용을 협업자들에게 알려주는 기능을 한다.

4. **merge**   
merge는 말 그대로 합치는 것이다. 새로운 branch에서 commit한 것을 base branch로 합치게 된다. merge는 3가지 종류가 있는데, 3개는 merge commit, squash and merge, rebase and merge이다. merge commit은 새로운 branch에서 한 모든 commit들을 base branch에 추가하는 것이다. squash and merge는 새로운 branch에서 한 모든 commit들을 전부 base branch에 추가하는 것이 아니라, 최종적으로 하나의 commit만 base branch에 추가한다. squash and merge는 새로운 branch에서 한 commit의 base를 재설정하고 base branch에 추가하는 것이다.

### 느낀점
오늘도 github의 여러 기능을 학습하였다. 프로젝트 시 협업하면서 사용해야 할 핵심적인 기능이라는 생각이 든다. 아직은 많이 사용해 본 적이 없어서 낯설고 어려운 기능들이지만, 계속 사용하다보면 익숙해질 것이다. 힘내자!

Pull Request 페이지의 링크입니다:
https://github.com/voyager63/2024-1-Beginner-Study/pull/5