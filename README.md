# Front

## <데모데이 - 팀 이거먹자>

### GitHub Convention

1. **앱 서비스 기능 확인 및 프로젝트 사용 라이브러리 + 스택 결정**
   - android, node.js, firebase → 추가 Tool & Framework 협의 후 결정

2. **Branch 전략**
   - 맡은 기능 또는 맡은 사람별로 Branch 결정

     1) 사람별로 Branch 개설 후 기능별로 구현  
     2) 아래와 같은 `feat` 별 개설 전략 활용  

     [브랜치 전략 참고](https://inpa.tistory.com/entry/GIT-%E2%9A%A1%EF%B8%8F-github-flow-git-flow-%F0%9F%93%88-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EC%A0%84%EB%9E%B5)

     ![Branch Strategy](https://prod-files-secure.s3.us-west-2.amazonaws.com/b89d707a-2ba4-4daa-9d94-eda7a218c766/e4a18899-5806-45ca-be25-1448b096c81a/image.png)

     ```
     
     master: 라이브 서버에 제품으로 출시되는 브랜치.
     develop: 다음 출시 버전을 대비하여 개발하는 브랜치.
     feature: 추가 기능 개발 브랜치. develop 브랜치에 들어간다.
     release: 다음 버전 출시를 준비하는 브랜치. develop 브랜치를 release 브랜치로 옮긴 후 QA, 테스트를 진행하고 master 브랜치로 합친다.
     hotfix: master 브랜치에서 발생한 버그를 수정하는 브랜치.
     ```

   - **Team 이거먹자 Branch 예시**  
     `main > develop > feat > individual` 형태로 작업을 진행(협의 후 결정)

---

3. **Issue Convention 결정 및 템플릿 작성**
   ### [Issue 작성 가이드](https://puleugo.tistory.com/165#Issue)
   - 담당자(Assignees)를 명시할 것
   - Task list 기능을 적극 활용할 것
   - 기능 관련 Issue라면 GitHub Project와 PR과 연동하여 진행상황 공유
  >> 자세한 내용은 템플릿 참고
---

4. **PR Convention 결정 후 템플릿 작성**
   ### [Pull Request 작성 가이드](https://puleugo.tistory.com/165#Pull-Request)
   - 제목은 '[#기능 번호] 변경 사항' 구조로 작성할 것
   - Issue와 연동할 것

   > **자주 커밋하고 PR은 300자를 넘지 않도록 주의**  
   > (짧은 간격으로 자주 PR)

   - 제목: **[Feat]** 핵심적인 부분만 간략하게 작성
   - 내용: 간결하게 리스트 방식으로 정리
   - 라벨: `FE`, `BE`, `기능추가`, `리팩토링`, `레이아웃`, `에러`
>> 자세한 내용은 템플릿 참고


5. **Commit Convention**
6. **Code Convention**
팀에서 통일된 코드 스타일을 따르기 위해 아래 규칙을 준수합니다.
- 메서드 , 변수명 통합
- solid pattern 결정 후 구조화
---


#### **Java Code Convention example**
- **Oracle Java Code Convention**을 따릅니다.  
  [참고 링크](https://www.oracle.com/java/technologies/javase/codeconventions-contents.html)

## 참고 자료
- [GitHub Flow & Git Flow](https://inpa.tistory.com/entry/GIT-%E2%9A%A1%EF%B8%8F-github-flow-git-flow-%F0%9F%93%88-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EC%A0%84%EB%9E%B5)
- [Branch 전략](https://velog.io/@kw2577/Git-branch-%EC%A0%84%EB%9E%B5)
- [Git Convention Example](https://chlolisher.tistory.com/173)
