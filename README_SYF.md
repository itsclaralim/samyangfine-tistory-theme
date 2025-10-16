# SYF Tistory Dawn-Style Starter

이 저장소는 티스토리 기본 스킨 위에 **커버/위젯 + CSS만으로 Dawn 스타일의 기업형 레이아웃**을 적용할 수 있도록 만든 스타터 킷입니다.

## 구성
- `/assets/logo.png` : 삼양화인 로고
- `/assets/hero-placeholder.jpg` : 메인 배너용 임시 이미지
- `/snippets/custom.css` : 전체 톤앤무드 CSS (색상/버튼/그리드)
- `/snippets/hero-widget.html` : 상단 헤더 + 히어로 섹션 (HTML 배너 위젯에 붙여넣기)
- `/snippets/cta-buttons.html` : 하단 고정 CTA 버튼
- `/snippets/product-card-guidelines.txt` : 글쓰기 템플릿 & 이미지 가이드

## 사용 방법 (GitHub → Tistory)
1) **GitHub 저장소 만들기**
   - GitHub 로그인 → New repository → 이름 예) `samyangfine-tistory-theme`
   - Public으로 생성 → `Add file > Upload files`로 이 폴더의 파일들을 업로드
   - 업로드 후, 각 파일을 클릭하면 **Raw** 주소가 나옵니다.
     - `logo.png`와 `hero-placeholder.jpg`의 Raw URL을 복사해둡니다.

2) **URL 치환**
   - `/snippets/custom.css` 파일 열기
     - `GITHUB_HERO_URL`을 1번에서 복사한 `hero-placeholder.jpg`의 Raw URL로 바꾸세요.
   - `/snippets/hero-widget.html` 파일 열기
     - `GITHUB_LOGO_URL`을 `logo.png`의 Raw URL로 바꾸세요.

3) **티스토리에 적용**
   - 티스토리 관리자 → **꾸미기 > 스킨 편집 > CSS**
     - `custom.css`의 내용을 **그대로 붙여넣기** 후 저장
   - 티스토리 관리자 → **꾸미기 > 사이드바/위젯**
     - **HTML 배너 위젯**을 맨 위에 추가 → `hero-widget.html` 내용을 붙여넣기
     - (선택) 또 다른 **HTML 배너 위젯**을 하단에 추가 → `cta-buttons.html` 붙여넣기

4) **메뉴 구성**
   - **꾸미기 > 메뉴**에서 다음 메뉴를 생성
     - 홈(`/`), 제품소개(`/category/제품소개`), 회사소개(`/category/회사소개`), 자료요청(`/category/자료요청`), 문의하기(`/category/문의하기`)

5) **제품 카드처럼 보이게 정리**
   - 글 목록은 카드형으로 보이도록 스킨 옵션에서 `카드/그리드` 선택
   - 제품 썸네일을 4:3 비율로 업로드 (가이드 문서 참조)

## 자주 묻는 질문
- **Q. GitHub에 올린 이미지가 안 보여요.**
  - Raw URL이 `https://raw.githubusercontent.com/...` 형태인지 확인하고, 공개 저장소인지 체크하세요.

- **Q. 완전한 커스텀 스킨(업로드 ZIP)으로 만들 수 있나요?**
  - 가능합니다. 다만 티스토리 전용 태그를 사용해야 하므로, 이 스타터로 먼저 스타일을 잡고, 이후 스킨화 작업을 진행하는 것을 추천합니다.