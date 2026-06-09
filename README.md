# PIXELFORGE ACADEMY 🎮

> 수도권ICT이노베이션스퀘어 · 쉬었음 청년 디지털 맞춤 교육 실습 (2026-06-09)
> 배포: https://restboy2606.github.io/2026-06-09/

레트로 픽셀 게임 개발사 **PIXELFORGE STUDIOS**의 교육 사업부, **PIXELFORGE ACADEMY**의
온라인 AI·AI 리터러시 **동영상 학교** 사이트입니다.
"게임 한 판 깨듯 배운다"는 컨셉으로, 강사님 템플릿(`aebonlee/rest04`)을 베이스로
우리 픽셀게임회사 브랜드를 입혀 재구성했습니다.

## 베이스 / 출처

- 클론 베이스: [`aebonlee/rest04`](https://github.com/aebonlee/rest04) (React + Vite + Tailwind, 온라인 동영상 교육 플랫폼)
- 개발 내역 참고: [`aebonlee/rest03`](https://github.com/aebonlee/rest03)
- 우리 픽셀 컨셉 출처: [`restboy2606/2026-06-08` PIXELFORGE STUDIOS](https://restboy2606.github.io/2026-06-08/)

## 핵심 요구사항 반영

| 요구사항 | 구현 |
|---|---|
| 주컬러 다크블루 + 로열블루 | `navy(#0b1a33)` + `royal(#2b5bff)` |
| 5색 컬러 팔레트 | navy · royal · sky · amber · mint (Tailwind `theme.colors`) |
| 다크 & 라이트 모드 | `<html class="dark">` 토글 + FOUC 방지 스크립트 |
| 모바일 최적화 | 반응형(Tailwind), 모바일 메뉴 패널 |
| 유튜브 2×3 배치 + 페이지화 | `PER_PAGE = 6`, 2열 그리드 + 페이지네이션 |
| 주제별 메뉴 | AI 콘텐츠 제작 / AI 리터러시 / 웹 / 파이썬 / R 탭 + 모듈 필터 |
| OG 메타 태그 | `index.html` og:type/site_name/title/description/url/image |
| OG 이미지 생성 | `scripts/make-og.mjs` (sharp, SVG→PNG 1200×630) → `public/og.png` |

## 기술 스택

- React 18 + Vite 5 + Tailwind CSS 3 + React Router 6
- 폰트: 본문 Pretendard / 브랜드·라벨 Mona(픽셀)
- 배포: GitHub Actions → GitHub Pages

## 픽셀 컨셉

- 운영: PIXELFORGE STUDIOS (레트로 픽셀 게임 개발사, Est. 2025.12.25)
- 브랜드: 픽셀 P 로고 · Mona 픽셀 폰트 · "한 판씩 클리어" 학습 카피
- 연락처: ssujklim@gmail.com (유일한 실제 연락처)

## 자주 쓰는 명령

```bash
npm install        # 의존성 설치
npm run dev        # 개발 서버
npm run og         # OG 이미지 재생성 (public/og.png)
npm run build      # 프로덕션 빌드 (dist)
npm run preview    # 빌드 미리보기
```

## OG 미리보기 디버깅

카카오 공유 디버거에서 확인: https://developers.kakao.com/tool/debugger/sharing
(URL 입력 후 캐시 초기화하여 og:image 갱신)

---

© 2026 PIXELFORGE STUDIOS · 교육 실습 프로토타입 (restboy2606)
