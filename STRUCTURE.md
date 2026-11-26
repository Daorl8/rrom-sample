# STRUCTURE · rrom-sample (v0.1.2 · 최근 게시물 톤 베이지 · 토프 · 진한 브라운 + 가는 대문자 라벨 · 약속 5조항 중심 · 모서리 2px · 배포 예정 rrom-sample.lgt3232.workers.dev)

```
rrom-sample/
├─ index.html                 단일 파일 (CSS · JS 인라인)
├─ wrangler.toml              name = rrom-sample
├─ .assetsignore              img/ · _old/ · 문서 · index_*.html · _deploy 배포 제외
├─ rr-jost-v01.woff2          영문 라벨 · 번호 · 가격 숫자 (Jost 300–500 · ASCII)
├─ rr-pretendard-v03.woff2    한글 · 본문 (Pretendard 300–600 · 본문 300 · 히어로 h1만 600 · 페이지 글자만 → 문구 바꾸면 재생성 + 이름 버전 올리기 R-43)
├─ rr-room.webp               히어로 시술실 1136×789
├─ rr-leg.webp                상담 · 다리 왁싱 900×1191
├─ rr-brow.webp               약속 · 눈썹 900×921
├─ rr-wax.webp                가격 · 왁스 391×749
├─ og-rr.jpg · favicon.png    og = 글자 + 시술실 · 파비콘 = 「R」
├─ img/                       다올 제공 원본 + _원문.md (배포 제외)
└─ CHANGELOG.md / STRUCTURE.md  (로컬 정본 · 업로드 안 함, R-38)
```

## 섹션 제목
섹션 h2 = 영문 `h2.en`(Jost 300 대문자 · CONSULTING · OUR PROMISE · FIRST VISIT · CLASS · RESERVATION) + 한글 제목은 `.sr` 숨김 글자.

## 섹션 순서
헤더 `.top`(sticky · 글자 로고 `.wm` · PC 메뉴 4 · 카카오톡 예약 / 900 미만 `.snav` 4칸 · 헤더 버튼 숨김 `.top .head-cta` R-52)
→ 히어로(라벨 · 위치 · h1 · 칩 · 버튼 3 한 줄 · 시술실 사진)
→ `#care` 상담 원문 + 처음 왁싱 원문 + 다리 사진
→ `#promise` 롬왁싱의 약속 `.pl` 01~05 + 눈썹 사진(900 이상 sticky)
→ `#price` 첫방문 카드 2 + 회원권 한 줄 + 안내 + 왁스 사진
→ `#class` 수강 상자 + 카카오 문의
→ `#visit` 예약 및 문의 + 버튼 + 영업시간 표 + 주소 dl + 구글 지도
→ 푸터(진한 브라운) + 900 미만 `.quick` 하단 바.

## 버튼 · 링크
- 카카오 채널 `https://pf.kakao.com/_VlyGG`: 헤더 · 히어로 · 수강 · 예약 · 푸터 · 하단 바
- 전화 `tel:050713430279`: 히어로 · 예약 · 오시는 길 · 하단 바
- 인스타 `instagram.com/rrom_waxing/` · 네이버 지도 `map.naver.com/p/entry/place/1031756146` · 네이버 플레이스(푸터)

## 모션 (강제 재생)
- `.reveal`(setInterval · 화면 90% 선 · 바닥이면 전부) · 앵커 rAF 스크롤(R-25 · 헤더 + 10px). reduced-motion 분기 없음. 흐르는 띠 없음.

## 폰트 재생성
문구 바꾸면 빠진 글자 검사(LESSONS §26). Pretendard `fonts/Pretendard-1.3.9/public/variable/PretendardVariable.ttf` → `fonttools varLib.instancer wght=300:600` → pyftsubset. Jost `fonts/fonts-main/ofl/jost/Jost[wght].ttf` → `wght=300:500`.
