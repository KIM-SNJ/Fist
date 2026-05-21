# 🌧️ Rain World Wiki (Balanced Scale)

> **레인 월드(Rain World)의 유기적인 생태계와 다양한 생명체 정보를 담은 웹 기반 위키 프로젝트입니다.** 본 프로젝트는 플레이어블 캐릭터인 '슬러그캣'과 게임 내 세계관을 구성하는 다양한 생물들의 상호작용, 독특한 생태계 시스템(관계값, 평판, 리니지 시스템, 체력 매커니즘)을 직관적이고 반응형 레이아웃의 웹 페이지로 구현했습니다.

---

## 🎮 게임 정보 (Game Info)

* **개발자 (Developer):** Videocult
* **배급사 (Publisher):** Akupara Games
* **장르 (Genre):** 메트로베니아, 고난이도, 생존

---

## ✨ 주요 특징 및 웹 페이지 구성 (Key Features & Layout)

### 1. 메인 페이지 (`wiki.html`)
* **사이드바(Sidebar):** 게임 기본 정보 및 PC 권장 사양 안내
* **개요(Overview):** 레인 월드의 유기적인 생태계 구성에 대한 개략적인 설명
* **메뉴 그리드(Menu Grid):** 생명체, 아이템, 음식, 업적 카테고리로 이동할 수 있는 직관적인 카드형 UI (Hover 애니메이션 적용)

### 2. 생명체 상세 페이지 (`wiki2.html`)
* **목차(TOC):** 원하는 정보를 빠르게 찾을 수 있는 스티키(Sticky) 네비게이션 바 구현
* **생태계 시스템 상세 구현:**
  * **관계(Relationships):** 무시, 먹고 싶음, 두려움, 공격 등 생물 간의 8가지 행동 반응 및 0.0~1.0 사이의 관계값 매커니즘 설명
  * **평판(Reputation):** 지역 평판, 글로벌 평판, 전체 평판에 따른 도마뱀 '중립화' 및 스캐빈저와의 관계 변화
  * **리니지 시스템(Lineage System):** 특정 굴(Shelter)에서 생물 사망 시 다음 주기에 일정 확률로 다른 종으로 대체 리스폰되는 시스템 설명 (예시 포함)
  * **체력 및 죽음(Health & Death):** 출혈 상태, 즉사 임계값 점검 및 환경적 즉사 판정 요인 정리
* **생명체 분류(Creature Types):** 슬러그 캣, 수비적/중립적/적대적/특별한 생명체 등 카테고리별 시각 자료(Graphic Box) 배치

---

## 💻 기술 스택 (Tech Stack)

* **HTML5:** 웹 페이지 구조 및 시맨틱 태그(`aside`, `main`, `section`) 활용
* **CSS3:** * Flexbox 및 Grid 레이아웃을 통한 균형 잡힌 웹 디자인
  * `position: sticky;`를 활용한 반응형 목차 기능
  * 미디어 쿼리(`@media`) 기반의 모바일/태블릿 반응형 레이아웃 대응 (1150px 이하 해상도 최적화)
  * 네온 스타일의 텍스트 섀도우(`text-shadow`) 및 다크 모드 분위기의 배경 블렌딩 구현

---

## 🖥️ 권장 사양 (System Requirements)

* **운영 체제:** Windows 10 64-bit
* **프로세서:** 6th Gen i5 / 2nd Gen Ryzen (or better)
* **메모리:** 8 GB RAM
* **그래픽:** GeForce 7 Series / Radeon RX400 Series (or better)
* **저장 공간:** 4 GB 사용 가능 공간

---

## 📂 프로젝트 구조 (Directory Structure)

```text
├── wiki.html             # 위키 메인 화면 (개요 및 메뉴)
├── wiki2.html            # 생명체 상세 정보 화면 (목차 및 시스템 가이드)
└── imgs/                 # 웹 페이지에 사용된 이미지 자산 폴더
    ├── back.png          # 배경 이미지
    ├── header.jpg        # 사이드바 메인 이미지
    ├── cat.png           # 슬러그캣 다이어그램
    ├── de.png            # 수비적 생명체 이미지
    ├── mi.png            # 중립적 생명체 이미지
    ├── en.png            # 적대적 생명체 이미지
    └── sp.png            # 특별한 생명체 이미지
