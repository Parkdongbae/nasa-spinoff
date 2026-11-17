# NASA Spinoff 기사 검색 (1976–2026)

NASA Spinoff 책(1976–2026, 2004 제외)을 중학교 수업용 슬라이드로 정리한 통합판 10개와, 그 안의 기사 2,210개를 한 번에 찾는 검색 페이지입니다.

- `index.html`: 검색 페이지입니다. 검색어, 판본, 분야로 찾을 수 있고 랜덤 검색 버튼이 있습니다. 결과를 누르면 해당 판본의 그 슬라이드(`#slide-N`)가 새 탭에 열립니다.
- `search_index.js`: 검색 색인입니다. 기사마다 제목, 영어 원제, 한 줄 요약, 핵심어, 쓰임새, 1000자 요약이 들어 있습니다.
- `NASA_Spinoff_YYYY_YYYY_정리.html`: 5~6년 단위 통합판 10개입니다. 사진까지 들어 있는 단일 HTML이라 인터넷 없이도 열립니다.

## 배포

빌드 단계가 없는 정적 사이트입니다. Vercel에서 이 저장소를 가져올 때 Framework Preset은 `Other`로 두고, Build Command와 Output Directory는 비워 두면 됩니다.

## 색인 다시 만들기

판본 HTML을 다시 만들면 슬라이드 번호가 바뀔 수 있습니다. 그때는 원본 작업 폴더에서 `python -X utf8 work/build_search.py`를 실행해 `search_index.js`를 새로 만든 뒤, 이 저장소에 함께 올립니다.
