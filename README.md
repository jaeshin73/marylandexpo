# 제13회 메릴랜드 엑스포 — 웹 파일

이 `web` 폴더 전체를 그대로 호스팅 서버의 공개 폴더(예: `public_html/expo/`)에 올리면 됩니다. 빌드 과정 없음.

```
web/
├── index.html            원페이지 사이트
├── css/styles.css
├── js/main.js            언어 전환 · 부스 필터 · 혈액검사 팝업 · 영상 일시정지
└── assets/
    ├── video/            hero-1080.mp4 (6.0MB), hero-720.mp4 (2.7MB, 모바일), hero-poster.jpg
    └── img/
        ├── logo/         MDEXPO-logo-kr.svg, MDEXPO-logo-en.svg
        ├── gallery/      갤러리 사진 10장 (900px, 장당 40–95KB)
        ├── sponsors/     후원 단체 로고
        └── qr/           사전 등록 QR
```

- 언어: 상단 버튼 또는 `?lang=en|es|ja|zh` (현재 헤더·HERO만 다국어, 본문은 한국어)
- 사전 등록 링크: https://wsk.church/expo
- 서버가 `.mp4`를 `video/mp4`로, 바이트 범위 요청(Range)을 지원해야 영상이 바로 재생됩니다 (대부분 기본 지원).
- 남은 자리표시: 지도 이미지 (오시는 길 섹션)
