# Portfolio Web

이미지(PNG) 기반 포트폴리오 웹페이지. 상단 고정 네비게이션에서 각 섹션으로 스크롤 이동.

## 구조
```
portfolio-web/
├─ index.html
├─ vercel.json
├─ .gitignore
└─ images/        (37개 PNG, ASCII 파일명)
```

## 배포 (GitHub + Vercel)

1. 이 폴더에서 git 초기화 후 push
   ```bash
   cd portfolio-web
   git init
   git add .
   git commit -m "portfolio web"
   git branch -M main
   git remote add origin https://github.com/<사용자명>/<레포명>.git
   git push -u origin main
   ```

2. https://vercel.com 접속 → **Add New → Project** → 해당 GitHub 레포 선택
3. Framework Preset은 **Other** (그대로 두면 됨), Root Directory는 이 폴더
4. **Deploy** 클릭 → 배포 완료 후 생성된 링크를 취업사이트에 등록

## 참고
- 이미지 폴더/파일명을 모두 영문(ASCII)으로 정리해 Vercel 경로 인코딩 문제를 방지함
- 이미지 방식이라 줄바꿈/글자깨짐/도형 틀어짐 없음
