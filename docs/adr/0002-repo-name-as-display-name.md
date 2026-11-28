# 0002. 표기 이름을 저장소 이름 PortfolioOpt4ESG 하나로

- 상태: 채택 (2026-11-27)

- **맥락:** 저장소 이름을 `LLM_ESG_POS`에서 PortfolioOpt4ESG로 바꾼 뒤에도 README 제목 괄호, 본문 주어, 결과표 행 이름, 연구 문서, 코드 docstring에 옛 서비스 이름 LEPOS가 현재 이름처럼 남아 있었다. 2026-11-27 작성자가 공개 저장소 이름 기준으로 맞추라고 했다. 게재 논문 제목에는 LEPOS가 없어(Computational Economics 2026, doi:10.1007/s10614-026-11413-9) 결과표 이름을 바꿔도 논문과 어긋나지 않는다.
- **결정:** 세 언어 README(제목·본문 주어·결과표 행·그림 설명), `CLAUDE.md`, `docs/research/RESEARCH.md`(제목·표), `.devcontainer/devcontainer.json`의 name, docstring과 표시 문자열(`app/main.py`, `src/__init__.py`, `src/config.py`, `scripts/score_text.py`, `docs/research/robustness_backtest.py`)을 PortfolioOpt4ESG로 쓴다. README에는 옛 이름 안내 한 줄만 둔다(저장소 옛 이름 `LLM_ESG_POS`, 순서도 등 이전 자료의 옛 서비스 이름 LEPOS).
- **결과:** 파일 이름(`docs/flowchart/lepos_flowchart.drawio`), 순서도 그림과 그 원본 안의 글자, `.gitignore`의 로컬 폴더 이름에는 LEPOS가 남는다. 그림은 이번에 다시 만들지 않는다.
