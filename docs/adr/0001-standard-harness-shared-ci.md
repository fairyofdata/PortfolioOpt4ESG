# 0001. 표준 하네스와 공용 CI

- 상태: 채택 (2026-11-24)

- **맥락:** 세션 규칙·작업 상황·CI가 저장소마다 달랐다. CI 단계가 다른 저장소들과 거의 같은데 따로 적혀 있었다.
- **결정:** CLAUDE.md에 세션 규칙, 작업 상황은 로컬 `state.md` 하나(`CLAUDE.local.md`가 가져옴, git 밖). CI는 공용 재사용 워크플로 `fairyofdata/Concordia`의 `python-tests.yml@v1`과 `hygiene.yml@v1`을 부른다. `.gitignore`에 `_private/`·`*.private.*`.
- **결과:** CI 단계를 고칠 일은 Concordia 한 곳에서. 대가: Concordia `v1`이 옮겨지면 이 저장소 CI도 따라 바뀐다.
