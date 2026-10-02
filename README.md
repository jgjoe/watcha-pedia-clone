# Watcha Pedia Clone

**왓챠피디아 모바일 화면을 HTML·CSS만으로 재현한 클론 코딩 — 스타일을 화면과 부품 두 층으로 쪼갰습니다**

[![HTML/CSS](https://img.shields.io/badge/HTML5%20%2B%20CSS3-no%20framework-E34F26?logo=html5&logoColor=white)](#기술-스택)
[![Screens](https://img.shields.io/badge/screens-7%20화면-informational)](#주요-기능)

프레임워크 없이 HTML과 CSS만으로 왓챠피디아의 주요 화면을 재현했습니다.
2023년에 처음 완주한 클론 프로젝트이고, **레이아웃과 스타일 구조를 스스로 잡아 보는 것**이 목적이었습니다.

## 주요 기능

**7개** — 시작/로그인(`index`) · 홈(`friends`) · 평가(`chats`) · 검색(`find`) · 나의 왓챠(`more`) · 왓챠에게 물어봐(`chat`) · 설정(`settings`)

## 설계 판단

- **스타일을 두 층으로 나눴습니다** — 화면마다 다른 것은 `css/screens/`(login·friends·chat·find·more·settings)에, 여러 화면에서 반복되는 것은 `css/components/`(화면 헤더·상태 바·내비게이션 바·뱃지·아이콘 행·유저 카드)에 뒀습니다. 화면이 7개로 늘어도 같은 스타일을 다시 쓰지 않습니다
- **색·간격을 변수로 뺐습니다** — `css/variables.css`에 CSS 커스텀 프로퍼티로 모아, 값을 한 곳에서 바꾸면 전 화면에 반영되게 했습니다
- **reset CSS로 브라우저 기본값을 먼저 지웠습니다** — 브라우저마다 다른 기본 여백·글꼴을 통제하고 시작하는 이유를 이때 이해했습니다
- **Flexbox 레이아웃** — 목록과 카드 정렬을 좌표가 아니라 배치 규칙으로 잡는 방식
- **화면 크기 대응** — 모바일 UI를 재현한 프로젝트라 데스크톱 폭에서는 안내를 띄우도록 `components/no-mobile.css`를 따로 뒀습니다

## 기술 스택

HTML5, CSS3 (아이콘만 Font Awesome CDN, 그 외 프레임워크·전처리기 없음)

## 실행

`index.html`을 브라우저로 열면 됩니다. 모바일 폭 기준으로 만들어 개발자 도구의 모바일 뷰에서 보는 편이 낫습니다.

## 만든 사람

**Jigwan Joe** — Frontend

- GitHub: [@jgjoe](https://github.com/jgjoe)
- Email: jigwan.joe@gmail.com
