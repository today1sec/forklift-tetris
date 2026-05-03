# 배포 가이드 - Tetris-Web

## 옵션 1: 그냥 더블클릭 (테스트용)
- `index.html` 파일 더블클릭
- 브라우저에서 바로 실행됨
- 주소: `file:///C:/AI_Project/ForkliftAI-crew/02_dev/tetris-web/index.html`
- 나만 볼 수 있음

## 옵션 2: 로컬 서버 (개발 중)
명령프롬프트(cmd)에서:
```
cd C:\AI_Project\ForkliftAI-crew\02_dev\tetris-web
python -m http.server 8000
```
브라우저: http://localhost:8000

## 옵션 3: Cloudflare Pages (인터넷 공개) ← 추천
1. https://dash.cloudflare.com 로그인
2. 좌측 메뉴: Workers & Pages → Create
3. Pages 탭 → Upload assets
4. 프로젝트명: `forklift-tetris`
5. `02_dev/tetris-web/` 폴더 통째로 드래그
6. Deploy 클릭
7. 결과 URL: `https://forklift-tetris.pages.dev`

이 URL을 받아서:
- 블로그 본문 "데모: " 자리에 넣기
  → `04_marketing/blog/20260427-ai-crew-test.md` 하단
  → `03_records/blog-ready/20260427-ai-crew-test.md` 하단
- 인스타 caption 본문에 (인스타는 링크 첨부 X 가능 → 프로필 링크로 우회)
- 스레드는 직접 링크 가능

## 옵션 4: GitHub Pages (코드 공개도 같이)
1. GitHub 레포 생성: `forklift-tetris`
2. `index.html` 푸시
3. Settings → Pages → Source: main branch
4. URL: `https://[유저명].github.io/forklift-tetris`

## 추천
- 빠른 공개: 옵션 3 (Cloudflare Pages)
- 코드도 같이 공개: 옵션 4 (GitHub Pages)
- 둘 다: GitHub 푸시 + Cloudflare Pages가 GitHub 연동
