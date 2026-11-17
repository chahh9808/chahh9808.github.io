# Hyeongheon Cha — Personal Website

Hyeongheon Cha의 개인 연구·학술 홈페이지 소스입니다. Hugo Extended 0.126.1과 Hugo Blox Academic CV 테마를 사용합니다.

## 수정할 파일

| 대상 | 소스 |
| --- | --- |
| 프로필·소개·소셜 링크·학력 | `content/authors/admin/_index.md` |
| 홈 섹션·뉴스·경력·수상·기술 | `content/_index.md` |
| 프로젝트 | `content/post/<slug>/index.md` |
| 논문 | `content/publication/<slug>/index.md` |
| 메뉴 | `config/_default/menus.yaml` |
| 사이트 URL | `config/_default/hugo.yaml` |
| 검색·공유 설명·테마·푸터 | `config/_default/params.yaml` |
| 모노톤 화면 스타일 | `assets/css/custom.css` |
| 홈 프로젝트 이미지·목록 레이아웃 | `layouts/partials/views/project-list*.html` |
| News 펼치기·접기 | `layouts/partials/blox/news.html` |
| 소개 영역의 배경 패턴 | `assets/media/hero-contours.svg` |
| CV 다운로드 | `static/uploads/resume.pdf` |

`public/index.html`을 포함한 `public/`은 빌드 결과물입니다. 이 파일을 직접 수정하면 다음 빌드에서 덮어써집니다. `resources/`도 생성 파일입니다.

News는 `content/_index.md`의 `content.items` 맨 위에 최신 항목을 추가합니다. 처음 10개를 표시하고 나머지는 펼쳐볼 수 있습니다. 이모지는 원래 색상을 유지합니다.

## 로컬 확인

저장소 루트에서 기존 로컬 Hugo 바이너리를 사용합니다.

```sh
.tools/hugo-0.126.1/hugo server --disableFastRender --bind 127.0.0.1 --port 1313
```

브라우저에서 `http://127.0.0.1:1313/`을 엽니다. 초안까지 확인하려면 `-D`를 추가합니다. `.tools/`는 Git에서 제외되므로 다른 컴퓨터에서는 Hugo **Extended 0.126.1**과 Go를 준비하고 `hugo` 명령을 사용하세요.

배포용 빌드만 확인할 때:

```sh
.tools/hugo-0.126.1/hugo --environment production --minify
```

검색 인덱스는 Hugo 빌드와 별도입니다. GitHub Pages 워크플로가 사용하는 명령은 `npx --yes pagefind@1.6.0 --site public`입니다. 로컬 검색까지 확인하려면 Node.js/npm을 준비하고 Hugo 빌드 후 이 명령을 실행해야 합니다. `pagefind.yml`은 메뉴·푸터 등 공통 문구를 검색 대상에서 제외합니다.

## 변경과 배포

별도 브랜치에서 수정하고 로컬로 확인합니다. `.github/workflows/publish.yaml`은 `main`에 push할 때 GitHub Pages 배포를 실행하도록 구성되어 있습니다. 로컬 파일 수정만으로는 배포되지 않습니다.

이름·소속·현재 직위·논문 저자·발표 연도·수상·공개 소개 등 핵심 내용은 소유자에게 확인한 뒤 변경합니다.

## 보관 자료와 참고 문서

- `archive/unused-content/`: 비활성 예제 페이지와 해당 미디어. Hugo 콘텐츠 경로 밖에 두어 배포에서 제외합니다.
- [편집 가이드](docs/WEBSITE_EDITING_GUIDE_EN.md)
- [검토 결과와 확인할 항목](docs/WEBSITE_REVIEW_KO.md)

Netlify 설정·모듈 연결 정보와 BibTeX 가져오기 워크플로는 소유자 확인 후 `archive/unused-automation/`에 보관했습니다. 현재 배포 구성은 GitHub Pages입니다. 테마 의존성 및 원저작자 고지가 있는 `LICENSE.md`는 유지합니다.

내용 없는 Talks 섹션은 `content/event/_index.md`의 `_build` 설정으로 비활성화했습니다. 실제 발표를 추가할 때 렌더링과 목록 노출 설정을 함께 복원하세요.
