# 성광교회 청년부 주일예배 안내

성광교회 청년부 주일예배를 소개하는 모바일 우선 원페이지 웹사이트입니다.

## 구성

- `index.html` — 메인 페이지 (환영 / 예배를 준비하는 마음 / 예배 순서 타임라인 / 셀 모임)
- `pdf.html` — 인쇄(PDF 저장)용 안내 문서
- `images/` — 웹용으로 최적화된 사진 (최대 1800px, ~0.5MB/장)
- `raw/` — 원본 사진 및 소스 자료 (git 추적 제외)

## 기술

- 순수 정적 HTML — 빌드 과정 없음
- Tailwind CSS (CDN), Pretendard 폰트, Heroicons (inline SVG)

## 로컬에서 보기

```bash
open index.html        # 또는
python3 -m http.server  # http://localhost:8000
```

## 배포 (Vercel)

정적 사이트라 별도 설정 없이 저장소를 연결하면 바로 배포됩니다.

```bash
# Vercel CLI 사용 시
vercel deploy --prod
```

- 메인 페이지: `/`
- PDF용 문서: `/pdf.html`
