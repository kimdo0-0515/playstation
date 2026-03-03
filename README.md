# 🎮 PlayStation 웹사이트 리뉴얼 프로젝트

> **PlayStation 공식 웹사이트(ko-kr)를 레퍼런스로 삼아, 주요 페이지 흐름과 인터랙션을 재구성한 리뉴얼 프로젝트입니다.**<br>
> 💡 본 프로젝트는 **기획/디자인 가이드 기반 구현 + 퍼블리싱 + 프론트엔드 로직 설계**까지 포함한 팀 프로젝트입니다.

<table>
  <tr>
    <th>리뉴얼 전</th>
    <th>리뉴얼 후</th>
  </tr>
  <tr>
    <th valign="top"><img src="" alt="리뉴얼 전"></th>
    <th valign="top"><img src="" alt="리뉴얼 후"></th>
  </tr>
</table>

#### ⚠️ 주의사항
> 본 프로젝트는 학습 및 포트폴리오 용도로만 사용됩니다.<br>
> PlayStation/SIE와는 무관하며, 사용된 브랜드 리소스의 저작권은 원저작자에게 있습니다.

---

## 📊 프로젝트 진행

### 📝 업무 및 역할
> 기획 30% / 디자인 30% / 퍼블리싱 및 프론트엔드 개발 50%

### 🛠️ 기술 스택

#### Frontend
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

#### Library & UI
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=flat-square&logo=jquery&logoColor=white)
![Bootstrap Icons](https://img.shields.io/badge/Bootstrap_Icons-7952B3?style=flat-square&logo=bootstrap&logoColor=white)
![Swiper](https://img.shields.io/badge/Swiper-6332F6?style=flat-square&logo=swiper&logoColor=white)

#### Tool
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)

---

## 🔗 작업 결과물 & 문서 링크

- 🌐 **리뉴얼 웹사이트 배포 링크**  
  👉 [PlayStation](https://kimdo0-0515.github.io/playstation/)

- 📐 **기획서 (Figma)**  
  👉 [기획서 with Figma](https://www.figma.com/design/wxrGeANcFvHwiNfsG1xb6k/-%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98-%EB%A6%AC%EB%89%B4%EC%96%BC-_Team-Astro?node-id=202-765&t=F9SIaogk0ZNBeofr-1)

- 🎨 **디자인 가이드 (Figma)**  
  👉 [디자인 가이드 with Figma](https://www.figma.com/design/wxrGeANcFvHwiNfsG1xb6k/-%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98-%EB%A6%AC%EB%89%B4%EC%96%BC-_Team-Astro?node-id=452-37&t=F9SIaogk0ZNBeofr-1)

- 🖥️ **화면 디자인 (Figma)**  
  👉 [화면 디자인 with Figma](https://www.figma.com/design/wxrGeANcFvHwiNfsG1xb6k/-%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98-%EB%A6%AC%EB%89%B4%EC%96%BC-_Team-Astro?node-id=1613-238&t=F9SIaogk0ZNBeofr-1)

- 📌 **개발 규칙 정의서 (Figma)**  
  👉 [개발 규칙 정의서 with Figma](https://www.figma.com/design/wxrGeANcFvHwiNfsG1xb6k/-%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98-%EB%A6%AC%EB%89%B4%EC%96%BC-_Team-Astro?node-id=2755-2&t=F9SIaogk0ZNBeofr-1)

---

## 🧭 웹사이트 개요

### 📌 프로젝트 소개
PlayStation 메인/스토어 경험을 참고하여  
**메인 페이지의 몰입형 인터랙션**, **스토어 탐색 흐름**, **게임 상세 페이지의 정보 구조**를 리뉴얼했습니다.  
특히 페이지가 많아지는 상황에서도 유지보수하기 쉽도록 **폴더 구조·컴포넌트 include·데이터 렌더링 규칙**을 정리해 적용했습니다.

### 👤 대상 사용자
- PlayStation 콘텐츠/독점작을 둘러보는 일반 사용자
- 게임 상세 정보(미디어/정보/리뷰)를 빠르게 확인하려는 사용자
- PlayStation을 처음 접해보는 잠재적인 고객층 사용자

### 🎯 사용 목적
- PlayStation 주요 섹션(PS5, 액세서리, 뉴스, 스토어, 게임) 탐색
- 게임 리스트 → 상세 페이지 이동(쿼리스트링 기반)
- 미디어 갤러리(이미지/영상)와 게임 상세 정보 등 확인

### ✨ 주요 특징
- 반응형 웹 기반 (PC / Tablet / Mobile)
- **데이터 객체 기반 렌더링** + 쿼리스트링을 통한 상세 페이지 구성
- Swiper를 사용한 다중 슬라이더 및 구간별 인터랙션
- include(header/footer/menu) 기반 공통 UI 재사용
- 공통 import.js를 통한 **CDN/스크립트 로딩 순서 관리**

---

## 💻 실행 환경

- ✅ **Chrome 브라우저 최적화**
- 🌐 CDN 기반 라이브러리 사용  
  → 원활한 실행을 위해 **인터넷 연결 필수**

---

## 🚀 핵심 기능

### 1️⃣ 공통 로더(import.js) 기반 구조
- CDN 라이브러리 **순서 보장 로딩**
- 중복 로드 방지 + 로드 실패 시 콘솔 에러 확인
- body id 기반으로 페이지별 스크립트 자동 연결  
  예: `<body id="gameBody">` → `js/pages/game.js` 로딩

---

### 2️⃣ 게임 리스트 → 게임 상세 페이지
- 리스트 카드 클릭 시 `game.html?id=...` 형태로 이동
- 상세 페이지에서 `URLSearchParams`로 id 읽기
- `games` 데이터 객체에서 해당 id 1개만 찾아 DOM 렌더링  
  (main video / 가격 / 평점 / 미디어 / 캐릭터 / must-play 섹션 등)

---

### 3️⃣ 반응형 Swiper 운용
- PC에서는 기본 레이아웃 중심, Tablet/Mobile에서 Swiper 활성화
- 특정 구간에서 Swiper `destroy()` / 재생성 패턴 적용
- 슬라이드 전환에 따라 **배경 이미지/썸네일/텍스트 동기화**

---

### 4️⃣ 인터랙션(Scroll 진입/상태 제어)
- IntersectionObserver로 섹션 진입 시 애니메이션 트리거(1회 실행)
- hover 기반 카드 인터랙션(PC) + 클릭 기반 UI(모바일) 대응
- 섹션별 UI 상태(active) 제어로 몰입형 전환 연출

---

## 🧠 어려웠던 점 & 해결 방식

### 1️⃣ 페이지가 많아질수록 스크립트 연결 유지보수 문제
**문제**
- 페이지별 스크립트를 조건문으로 계속 추가하면 관리가 어려움

**해결**
- body id 네이밍 규칙(`~~~Body`)을 기준으로 페이지명을 파생
- `import.js`에서 `js/pages/${pageName}.js` 자동 로딩하도록 구조화

---

### 2️⃣ Swiper 동기화(썸네일/메인/배경/텍스트)
**문제**
- 슬라이드 전환 타이밍이 어긋나거나, loop/realIndex 처리로 동기화가 꼬이는 문제 발생

**해결**
- Swiper 이벤트( init / slideChangeTransitionEnd 등 ) 시점 통일
- 필요한 경우 `update()`와 DOM 렌더링 순서를 조정해 초기화 안정화
- 모바일 전용 텍스트 UI는 활성 슬라이드의 pagination 값을 읽어 동기화

---

### 3️⃣ 외부 리소스(영상/이미지) 사용 시 불안정한 재생/로딩
**문제**
- 외부 URL 영상이 네트워크 상황에 따라 끊기거나 로딩이 지연됨

**해결**
- autoplay 정책(muted/playsinline) 준수
- UX 관점에서 썸네일/오버레이 처리 및 사용자가 상태를 인지할 수 있는 구조로 설계

---

## 🗂️ 데이터 구조 & 라우팅

### 1️⃣ 게임 데이터 구조
- `games.js` 내 `window.games = [...]` 형태로 관리
- 게임 id 기준으로 필요한 정보(cover/logo/media/video/review 등) 렌더링

### 2️⃣ 상세 페이지 라우팅 방식
- `game.html?id=...` 형태의 쿼리스트링
- `URLSearchParams` → id 파싱 → `find()`로 해당 게임 객체만 렌더링  
  (상세 HTML 1개 + 데이터 객체 관리 방식)

---

## 🗂️ 프로젝트 폴더 구조

```text
project-root/
├─ index.html
├─ login.html
├─ ps5.html
├─ ps5-pro.html
├─ accessories.html
├─ store.html
├─ game.html
├─ news.html
│
├─ include/
│  ├─ header.html
│  ├─ footer.html
│  └─ mobile-menu.html
│
├─ css/
│  ├─ common/
│  │  ├─ import.css
│  │  ├─ font.css
│  │  ├─ variable.css
│  │  ├─ reset.css
│  │  ├─ component.css
│  │  └─ basic-layout.css
│  └─ pages/
│     ├─ index.css
│     ├─ game.css
│     └─ ...
│
├─ js/
│  ├─ common/
│  │  ├─ import.js
│  │  ├─ header.js
│  │  └─ footer.js
│  ├─ data/
│  │  ├─ global.js
│  │  └─ games.js
│  └─ pages/
│     ├─ index.js
│     ├─ game.js
│     └─ ...
│
└─ assets/
   ├─ icon/
   ├─ img/
   │  ├─ pages/
   │  └─ games/
   └─ video/
      └─ pages/
```

### 📦 사용 라이브러리
- jQuery
- Bootstrap icon
- Swiper
- GSAP

---

## 🙌 프로젝트를 통해 배운 점

- 공통 로더 기반의 스크립트 아키텍처 설계(순서/중복/에러 관리)
- 데이터 중심의 상세 페이지 렌더링(쿼리스트링 + 객체 탐색)
- Swiper를 반응형 구간별로 운용하며 생기는 실전 이슈 대응
- include 기반 공통 컴포넌트 구성으로 UI 일관성과 유지보수성 강화
