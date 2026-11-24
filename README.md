# 🛒 AI Budget Mate (YOUNG리한 파트너) 🛒

24016008 김서린

팀 프로젝트, 원본: [seulkong/Young_AI-partner](https://github.com/seulkong/Young_AI-partner)

🔗 **사이트 바로가기: https://time-frontend-gamma.vercel.app/**
(GitHub Pages: https://seorin-lab.github.io/time/)

## 📣 프로젝트 소개

대학생이 편의점에서 받을 수 있는 행사(1+1, 2+1), 통신사 멤버십, 카드 할인을 한 번에 계산해 주는 AI 소비 추천 웹사이트이다.
사용자의 통신사, 카드, 소비 성향 정보를 바탕으로 어느 편의점에서 얼마에 살 수 있는지 알려 주며, 0청년·유쓰·Y박스 같은 대학생 전용 혜택도 함께 챙기도록 구성하였다.

## 📣 주요 기능

1. 소비 성향 설정 기능: 헬시플레저, 디저트러버, 브랜드 선호, 트렌드/인기 중 성향을 선택하면 맞춤 상품 추천
2. 행사 상품 조회 기능: CU, GS25의 월별 1+1, 2+1 행사 상품 검색
3. 편의점 비교 기능: 같은 상품을 다른 편의점에서 더 싸게 살 수 있으면 비교 추천
4. 할인가 계산 기능: 행사 할인 → 통신사 할인 → 카드 할인 순서로 적용한 최종 가격 표시
5. 통신사/카드 혜택 기능: 멤버십 등급(VIP/Gold/Silver)과 대학생 전용 혜택 자동 적용, 최적의 카드 추천
6. AI 챗봇 기능: 상품 종류(예: 우유)나 상품명을 입력하면 가장 저렴한 할인 조합 안내
7. 근처 편의점 찾기 기능: 지도로 주변 편의점 위치 표시
8. 영수증 분석 기능: 영수증 사진을 올리면 놓친 할인이나 행사를 AI가 분석
9. 구글 로그인 기능: Google 계정으로 간편 로그인
10. 행사 데이터 수집 기능: 크롤러로 편의점 행사 정보를 자동 수집

## 📣 사용 기술

1. HTML
2. CSS
3. JavaScript
4. Python (FastAPI)
5. 크롤링: requests, BeautifulSoup, pandas
6. 데이터베이스: SQLite (Cloudflare D1)
7. AI: Google Gemini, Anthropic Claude, OpenAI GPT
8. Google OAuth
9. Cloudflare Workers / Pages (팀 프로젝트 배포용)
10. 카카오 지도 JavaScript SDK (근처 편의점 검색)
11. Vercel, GitHub Pages (포트폴리오 사이트 배포용)

## 📣 폴더 안내

1. Young_AI-partner: 팀 저장소의 최종 코드 (커밋 기록 포함, 자세한 설명은 [Young_AI-partner/README.md](./Young_AI-partner/README.md))
2. 루트 파일(index.html, api_server.py, crawling.py 등): 개발 초기 버전

## 📣 포트폴리오 배포 및 개선 내용

팀 프로젝트가 끝난 뒤, 포트폴리오로 공개하기 위해 직접 배포하고 아래 내용을 개선하였다.

1. 사이트 배포: `Young_AI-partner/frontend` 폴더를 Vercel(https://time-frontend-gamma.vercel.app/)과 GitHub Pages(https://seorin-lab.github.io/time/, `gh-pages` 브랜치)에 배포
2. 근처 편의점 검색 복구: 공개 저장소에 노출되어 비활성화된 카카오 REST API 키 대신, 등록한 도메인에서만 작동하는 카카오 지도 JavaScript SDK로 변경
3. 첫 이용 흐름 정리: 시작하기 → 이름 입력 → 설문(소비 스타일, 편의점, 통신사, 카드, 간편결제)을 마쳐야 본 페이지로 이동하도록 수정
4. 설정 변경 개선: '설정 변경하기'로 설문에 들어가면 기존 답이 미리 선택되도록 수정
5. 버그 수정: 프로필에서 통신사와 대학생 전용 요금제가 표시되지 않던 문제 수정
6. 디자인 통일: 시작 페이지와 회원가입 페이지를 설문 페이지와 같은 테마(그라데이션 배경, 반투명 카드, 남보라색 강조)로 변경
7. 화면 개선: 프로필 상자를 배경색으로 구분하고, 챗봇(Young-AI) 버튼을 화면 오른쪽 끝으로 이동

※ 챗봇과 상품 추천 기능은 팀 프로젝트의 Cloudflare Workers 서버를 그대로 사용한다.

## 📣 팀원

1. [seulkong](https://github.com/seulkong)
2. [seorin-lab](https://github.com/seorin-lab)

## 📣 배포 주소

- 사이트
  Vercel: https://time-frontend-gamma.vercel.app/
  GitHub Pages: https://seorin-lab.github.io/time/
- 저장소: https://github.com/seorin-lab/time
- 팀 프로젝트 원본 사이트: https://ai-budget-mate-web.pages.dev/
