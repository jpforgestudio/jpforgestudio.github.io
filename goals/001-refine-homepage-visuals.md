# Problem

홈페이지를 포함해 이 저장소의 public page들이 좀 촌스러움.

내용이 문제라기보다는, 현재 시각 언어가 SaneFocus의 "조용한 Mac 유틸리티"
느낌보다 generic pastel startup landing page 쪽으로 읽힐 수 있다.

촌스럽게 느껴질 수 있는 이유:

- 배경의 layered radial gradient와 밝은 diagonal gradient가 약간
  early-2020s startup/no-code landing page처럼 보인다.
- hero card의 큰 radius, 반투명 배경, blur, 강한 shadow 조합이
  template-like glassmorphism처럼 보일 수 있다.
- H1이 너무 크고 자간이 강하게 조여 있어서 "Quiet tools"라는 메시지와 달리
  시각적으로 목소리가 크다.
- brand signal이 작은 dot과 텍스트 위주라, polished small Mac app studio보다
  임시 템플릿처럼 느껴질 수 있다.
- "Current app" / "Local-first by default" 카드 구성이 명확하지만 예측 가능한
  landing-page block처럼 보인다.
- 배경, 카드, 그림자가 실제 제품보다 먼저 보여서, SaneFocus의 작고 빠른
  도구 성격보다 장식이 앞설 수 있다.

# Goal

JP Forge Studio 사이트 전체를 더 차분하고, 세련되고, 덜 촌스럽게 다듬는다.

단, 사이트가 loud SaaS landing page처럼 보이면 안 된다. 목표는 트렌디하게
바꾸는 것이 아니라, "작고 조용한 native Mac utility를 만드는 스튜디오"라는
인상을 더 정확하게 주는 것이다.

좋은 방향:

- 더 조용한 background treatment
- 더 절제된 hero composition
- subtler shadow and border
- 덜 과장된 headline scale
- product-first visual hierarchy
- SaneFocus 제품 페이지로 이어지는 더 깔끔한 entry point

피할 것:

- gradient-heavy startup 느낌
- glassmorphism이 메인 아이디어가 되는 디자인
- 앱보다 장식이 먼저 보이는 hero
- 큰 SaaS 제품처럼 보이는 과장된 layout
- 유행을 따라가서 빨리 낡을 visual effect

# Plan

작업은 한 번에 크게 갈아엎지 말고, 공통 스타일과 필요한 HTML만 작고 리뷰
가능한 단위로 변경한다.

Primary files:

- `index.html`
- `styles.css`
- `sanefocus/index.html`
- `sanefocus/support/index.html`
- `sanefocus/privacy/index.html`

Reference:

- `docs/theme-references.md`

Possible improvements:

- 사이트 전체 background를 더 조용하게 만든다.
- hero card와 doc/card의 blur, shadow, radius, border treatment를 줄인다.
- H1/H2 scale, line-height, spacing을 더 차분하게 조정한다.
- SaneFocus preview image와 media grid가 장식이 아니라 제품 proof처럼 보이게 한다.
- 홈의 "Current app" 섹션과 제품 페이지의 card/feature section이 기본 landing
  page block처럼 보이지 않게 다듬는다.
- support/privacy 문서 페이지가 더 신뢰감 있고 읽기 쉬운 document처럼 보이게 한다.
- 모바일에서 hero, section, doc spacing이 어색하지 않은지 확인한다.

Constraints:

- static HTML/CSS 구조를 유지한다.
- framework나 build step을 도입하지 않는다.
- privacy/support/product-page copy는 이번 visual pass와 직접 관련 있을 때만
  건드린다.
- SaneFocus의 calm, local-first, Mac-native tone을 유지한다.

Checks before finishing:

- 모든 public page가 static page로 정상 로드된다.
- desktop/mobile에서 layout overlap이 없다.
- 텍스트가 작은 화면에서 과하게 크거나 답답하지 않다.
- 링크와 product media가 그대로 동작한다.
- 결과물이 덜 촌스러워졌지만 trend-driven으로 보이지 않는다.

# Log

- 2026-05-02: Created goal file and captured the initial visual diagnosis.
- 2026-05-02: Expanded scope from homepage-only to all public pages in the repo.
- 2026-05-02: Applied a shared visual refinement pass in `styles.css`: quieter
  background, subtler cards, calmer heading scale, reduced glassy hero treatment,
  and mobile spacing adjustments across homepage, product, support, and privacy pages.
- 2026-05-02: Added an SVG favicon and linked it from every public page.
