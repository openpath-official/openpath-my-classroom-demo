# OPENPATH 내 강의장 (풀페이지 데모) — ⚠ ARCHIVED

> **🚨 폐기 상태 (2026-06-11)**
>
> 메디오피아 임종혁 본부장 회신 = **마이페이지 통합 안 채택**.
> 풀페이지 데모 = 작업 X. 작업 결과 보존 (참고용).
>
> **진행 데모** = https://github.com/openpath-official/openpath-learner-portal-demo (마이페이지 통합형)
>
> 이식 list = `docs/reports/2026-06-11_세션_핸드오버_통합안_이식.md`

---

오픈패스 LMS 이관 = 메디오피아 default 풀페이지 진입 가정 데모 (= **결과적으로 채택 X**).

## 보기

브라우저에서 `index.html` 열기 또는 Vercel 배포 URL 확인.

## 구조

- **GNB 사라짐** = openpath.kr 상단 메뉴 X → 자체 minimal 헤더
- **자체 헤더** = OPENPATH 로고 + "내 강의장" 타이틀 + 검색·알림·avatar + "포털 나가기"
- **좌측 LNB** = 검정 Gray10 박스 (Figma 99_컴포넌트 Sidebar/Learner Portal/PC 정합)
  - 학습 메뉴 (대시보드 / 수강 과목 / 출결 현황 / 성적·수료증 / 질의응답)
  - dashed divider
  - 계정 메뉴 (개인 정보 관리 / 결제·환불 내역 / 내 쿠폰 / 1:1 문의)
  - 로그아웃
- **VOD 플레이어** = 풀스크린 몰입 모드 (LNB·GNB 둘 다 숨김)
- **진입**: openpath.kr GNB "내 강의장" → 풀페이지 전환
- **종료**: "포털 나가기" → openpath.kr 메인 복귀

## 두 데모 비교

| Demo | URL | 의미 |
|---|---|---|
| 마이페이지 통합형 | https://openpath-learner-portal-demo-gcsu.vercel.app/ | 듀오톤 제안 안 = 메디 회신 대기 |
| 풀페이지 내 강의장 | (this repo Vercel URL) | 메디 default = fallback |

## 디자인 기반

- openpath.kr 라이브 CSS (global.css)
- Figma `[OPP] 06_Deliver-2026_검수용` (mypage / VOD player / 1:1 문의)
- Figma `[OPP] 02_Learning_v0` 99_컴포넌트 (Sidebar / CourseCard / StatusCard)
- 카드 매트릭스 v1 (VOD 16 / 신청 12 / 원격훈련 12 / 멤버십 1 variant)

## 라이센스

내부 검토용. 외부 공유 금지.
