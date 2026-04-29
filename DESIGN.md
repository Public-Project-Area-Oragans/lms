# Design System - DevPath AI

## Product Context
- **What this is:** AI 기반 적응형 학습 관리 시스템 + 학습 맥락을 아는 개발자 커뮤니티
- **Who it's for:** 부트캠프 3개월차 ~ 주니어 3년차 한국 백엔드 개발자
- **Space/industry:** EdTech, 한국 개발자 학습 플랫폼
- **Project type:** Web app (React 18 + Tailwind) + Mobile app (Flutter 3.x)

## Aesthetic Direction
- **Direction:** Industrial/Utilitarian
- **Decoration level:** Intentional (코드 블록 스타일의 미묘한 텍스처)
- **Mood:** "진지한 개발자 도구". GitHub/Linear처럼 기능 중심, 신뢰감. 친근하지만 가볍지 않음.
- **Memorable thing:** "내 학습 맥락을 아는 유일한 커뮤니티"

## Typography
- **Display/Hero:** Satoshi (Fontshare) -- 기하학적이지만 따뜻함. 개발자 도구 + 접근성
- **Body:** DM Sans (Google Fonts) -- 깔끔하고 읽기 쉽움. tabular-nums 지원
- **UI/Labels:** DM Sans (same as body)
- **Data/Tables:** DM Sans with font-variant-numeric: tabular-nums
- **Code:** JetBrains Mono (Google Fonts) -- 업계 표준
- **Loading:** Google Fonts CDN (DM Sans, JetBrains Mono) + Fontshare CDN (Satoshi)
- **Scale:**
  - xs: 12px / 0.75rem
  - sm: 13px / 0.8125rem
  - base: 15px / 0.9375rem
  - lg: 18px / 1.125rem
  - xl: 22px / 1.375rem
  - 2xl: 28px / 1.75rem
  - 3xl: 36px / 2.25rem
  - 4xl: 48px / 3rem

## Color
- **Approach:** Restrained (1 accent + neutrals. 색은 드물게, 의미 있을 때만)
- **Primary:** #0F6FEC (Cobalt Blue) -- 신뢰, 전문성, 집중. 링크, 주 CTA, 선택 상태
- **Primary Hover:** #0D5FCC
- **Accent:** #F59E0B (Amber) -- 성취, 평판, 배지 강조. "노력이 인정받는 곳" 느낌
- **Accent Hover:** #D97706
- **Neutrals:**
  - ink: #0A0A0A (primary text)
  - muted: #404040 (secondary text, body)
  - subtle: #737373 (tertiary text, timestamps, labels)
  - border: #E5E5E5 (dividers, card borders)
  - surface: #F5F5F5 (card backgrounds, AI seed area)
  - bg: #FAFAFA (page background)
- **Semantic:**
  - success: #059669 (채택, 완료)
  - warning: #D97706 (주의, AI 검토)
  - error: #DC2626 (에러, 삭제)
  - info: #2563EB (알림, 정보)
- **Dark mode:**
  - bg: #0A0A0A
  - surface: #1A1A1A
  - border: #2A2A2A
  - ink: #F5F5F5
  - muted: #A3A3A3
  - subtle: #737373
  - primary: #4D94F8 (밝게 조정)
  - accent: #FBBF24 (밝게 조정)
  - 채도 10% 감소

## Spacing
- **Base unit:** 4px
- **Density:** Comfortable
- **Scale:**
  - 2xs: 2px
  - xs: 4px
  - sm: 8px
  - md: 16px
  - lg: 24px
  - xl: 32px
  - 2xl: 48px
  - 3xl: 64px

## Layout
- **Approach:** Hybrid (앱은 grid-disciplined, 랜딩은 creative-editorial)
- **Grid:** 12-column, responsive breakpoints:
  - mobile: 1 column (< 640px)
  - tablet: 8 columns (640-1024px)
  - desktop: 12 columns (1024px+)
- **Max content width:** 1200px
- **Border radius:**
  - sm: 4px (buttons, tags, inputs)
  - md: 8px (cards, dropdowns)
  - lg: 12px (modals, large containers)
  - full: 9999px (avatars, pills)

## Motion
- **Approach:** Intentional (상태 전환 + 스켈레톤 로딩)
- **Easing:**
  - enter: ease-out
  - exit: ease-in
  - move: ease-in-out
- **Duration:**
  - micro: 75ms (hover, active states)
  - short: 150ms (dropdowns, tooltips)
  - medium: 300ms (modals, accordions, AI seed toggle)
  - long: 500ms (page transitions, skeleton fade)

## Community-Specific Design Rules
- **AI Seed Answer:** surface 배경(#F5F5F5), 하단 위치, 아코디언 접힘 기본. aria-expanded 필수.
- **Human Answer:** 상단 위치, accent 강조(채택 시). AI보다 시각적 가중치 높게.
- **Reputation Badge:** accent 색상(#F59E0B). DM Sans tabular-nums로 숫자 정렬.
- **Learning Context Card:** surface 배경, border, 답변자에게만 표시.
- **Empty States:** 따뜻한 메시지 + 주 액션 버튼. "결과 없음"은 디자인 실패.
- **맥락 첨부 토글:** 인라인 확장. ARIA checkbox group. 키보드 Tab/Space 조작 가능.

## Decisions Log
| Date | Decision | Rationale |
|------|----------|-----------|
| 2026-04-29 | Initial design system created | Created by /design-consultation based on competitive research (programmers.co.kr, inflearn, OKKY) + "학습 맥락을 아는 커뮤니티" positioning |
| 2026-04-29 | Amber accent for reputation | EdTech에서 드문 선택. "노력이 인정받는 곳" 느낌을 전달하기 위한 의도적 리스크 |
| 2026-04-29 | Industrial/Utilitarian aesthetic | 경쟁사들의 "친근하고 밝은" 패턴과 차별화. GitHub/Linear 같은 개발자 도구 신뢰감 |
