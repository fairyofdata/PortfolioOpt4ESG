# 결정 기록

결정 하나를 「맥락 → 결정 → 결과」로 짧게 적는다. 새 것이 아래. 뒤집을 때는 지우지 않고 「대체됨(→ D번호)」을 단다.

## D1. 표준 하네스와 공용 CI (2026-11-24)

- **맥락:** 세션 규칙·작업 상황·CI가 저장소마다 달랐다. CI 단계가 다른 저장소들과 거의 같은데 따로 적혀 있었다.
- **결정:** CLAUDE.md에 세션 규칙, 작업 상황은 로컬 `state.md` 하나(`CLAUDE.local.md`가 가져옴, git 밖). CI는 공용 재사용 워크플로 `fairyofdata/Concordia`의 `python-tests.yml@v1`과 `hygiene.yml@v1`을 부른다. `.gitignore`에 `_private/`·`*.private.*`.
- **결과:** CI 단계를 고칠 일은 Concordia 한 곳에서. 대가: Concordia `v1`이 옮겨지면 이 저장소 CI도 따라 바뀐다.

## D2. 표기 이름을 저장소 이름 PortfolioOpt4ESG 하나로 (2026-11-27)

- **맥락:** 저장소 이름을 `LLM_ESG_POS`에서 PortfolioOpt4ESG로 바꾼 뒤에도 README 제목 괄호, 본문 주어, 결과표 행 이름, 연구 문서, 코드 docstring에 옛 서비스 이름 LEPOS가 현재 이름처럼 남아 있었다. 2026-11-27 작성자가 공개 저장소 이름 기준으로 맞추라고 했다. 게재 논문 제목에는 LEPOS가 없어(Computational Economics 2026, doi:10.1007/s10614-026-11413-9) 결과표 이름을 바꿔도 논문과 어긋나지 않는다.
- **결정:** 세 언어 README(제목·본문 주어·결과표 행·그림 설명), `CLAUDE.md`, `docs/research/RESEARCH.md`(제목·표), `.devcontainer/devcontainer.json`의 name, docstring과 표시 문자열(`app/main.py`, `src/__init__.py`, `src/config.py`, `scripts/score_text.py`, `docs/research/robustness_backtest.py`)을 PortfolioOpt4ESG로 쓴다. README에는 옛 이름 안내 한 줄만 둔다(저장소 옛 이름 `LLM_ESG_POS`, 순서도 등 이전 자료의 옛 서비스 이름 LEPOS).
- **결과:** 파일 이름(`docs/flowchart/lepos_flowchart.drawio`), 순서도 그림과 그 원본 안의 글자, `.gitignore`의 로컬 폴더 이름에는 LEPOS가 남는다. 그림은 이번에 다시 만들지 않는다.
