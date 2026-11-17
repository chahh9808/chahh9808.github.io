# 개인 홈페이지 검토 및 정리

최초 검토: 2026-11-06. 후속 수정: 2026-11-17.
대상: `chahh9808.github.io` 로컬 저장소, `chore/content-cleanup` 브랜치.

## 처리한 항목

| 항목 | 처리 및 확인 |
| --- | --- |
| 프로필의 타인 실적·가상 경력 | 숨겨진 타인 논문·수상·프로젝트, GenCoin/X 예제 경력, 가상 기술·언어 숙련도·강좌 수상 내역 제거 |
| 학력 예제 | 예제 학위, `lorem ipsum` 과목, 가짜 학위논문 버튼 제거. 기존 실제 학력 데이터 유지 |
| 비활성 데모 | 페이지와 미디어를 `archive/unused-content/`에 보관. 미디어 8개, 1,735,355바이트를 배포 대상에서 제외하고 원본 SHA-256 일치 확인 |
| 템플릿 설정·코드 | 테마 홍보 README 교체. 타인 후원 계정·데모 스크린샷·템플릿 뉴스 갱신 워크플로·미사용 GitHub 버튼 스크립트·주석 데모 제거 |
| 레이아웃 경고 | 지원하지 않는 `compact`/`list`를 기존 자동 대체값 `card`로 명시. 화면 유지, 경고 7개 제거 |
| 로컬 도구 | `.venv/`를 `.gitignore`에 명시 |
| 공개 소개·검색 정보 | **2026-11-06 소유자 승인.** 기준 URL을 `https://chahh9808.github.io/`로 설정하고 본인 소개로 SEO 설명 교체. `GetResearchDev` 제거. MSRA 소개를 과거 경력으로 수정 |
| ORCID·LinkedIn | **2026-11-17 소유자 결정: 현재 링크 유지.** 재확인 없이 삭제하거나 대체하지 않음 |
| 논문 공동기여 | **2026-11-17 소유자 승인.** IMG2IMU·Sherlock·SNAP·TESLA의 `Equal contribution` 표기 모두 삭제. 저자 목록은 유지 |
| 기관 정보 | **2026-11-17 소유자 승인.** 연구실 링크를 `miil.kaist.ac.kr`, 학교 링크를 `www.kaist.ac.kr`로 정정. KAIST 신입생 프로그램 기관명을 `Korea Advanced Institute of Science and Technology`로 정정 |
| 오타·뉴스 정렬 | `Recieved` → `Received`, `Microsoft Resarch Asia` → `Microsoft Research Asia`, `crimess` → `crimes`. 뉴스 날짜를 내림차순으로 정렬 |
| 논문 목록 개수 | `count: 0`으로 모든 논문 표시. 현재 5개 유지, 이후 추가해도 기본값 5개에 제한되지 않음 |
| 논문 링크 버튼 | 프로젝트에 이미 있던 주소를 논문에도 연결: SNAP Code·Project, IMG2IMU·Beyond Hearing Project |
| 검색 범위 | `pagefind.yml`에서 공통 헤더·푸터·사이드바·목차·검색 UI를 색인에서 제외. 테마 템플릿 수정 없이 처리 |
| 검색 도구 버전 | GitHub Pages·Netlify·로컬 안내를 검증한 Pagefind 1.6.0으로 통일. Netlify 명령의 인자도 `--site`로 통일 |
| 카드 요약 | **2026-11-17 소유자 승인.** SNAP·IMG2IMU·Sherlock의 긴 요약을 승인된 짧은 문구로 교체. 논문 초록은 유지 |
| 미사용 자동화 | **2026-11-17 소유자 확인: 둘 다 미사용.** Netlify 설정·모듈 연결 정보 및 BibTeX 워크플로를 `archive/unused-automation/`로 이동. 활성 Netlify 모듈·체크섬·전용 출력 형식 제거. GitHub Pages 유지 |

다른 사람 이름이라는 이유로 기존 논문의 공저자를 삭제하지 않았습니다. 테마 의존성과 `LICENSE.md`의 원저작자 고지는 유지했습니다.

## 추가 승인 후 반영한 내용

| 항목 | 구체적인 제안 | 상태 |
| --- | --- | --- |
| 논문 날짜 | Beyond Hearing `2026-04-23`(ICLR 개막일), IMG2IMU `2025-09-01`(2025년 9월호 정렬용 대표일), SNAP `2025-12-02`(NeurIPS 개막일). 사이트 게시일·프로젝트 날짜 유지 | 승인 및 반영 완료 |
| Beyond Hearing 저자·기여 | PDF 기준 마지막 네 명을 `Dongyao Chen → Cecilia Mascolo → Sung-Ju Lee → Lili Qiu`로 정정. 첫 네 저자에게 공동기여 표기. 프로젝트·논문 모두 적용 | 승인 및 반영 완료 |
| 푸터·빈 Talks | 푸터 이름 `Me.` → `Hyeongheon Cha.`(기존 콘텐츠 라이선스 유지). 내용 없는 `/event/`는 목록·검색·빌드에서 제외 | 승인 및 반영 완료 |

날짜 제안은 프리프린트 게시일 대신 학회·저널 발행 기준을 사용하는 안입니다. 저널 발행일이 월 단위인 경우 1일은 정렬을 위한 대표일이며 정확한 발행 일자를 뜻하지 않습니다.

## 유지하기로 한 항목과 선택적 개선

- **CV:** 소유자 요청에 따라 현 상태 유지. PDF 수정은 수행하지 않았으며 Git 원본과 바이트가 동일함을 확인했습니다.
- **ORCID·LinkedIn:** 소유자가 현재 링크 유지를 선택했으므로 변경하지 않았습니다.
- **경력·수상 스타일:** 아래 모노톤 디자인 변경 과정에서 반복 인라인 스타일을 공통 CSS로 분리했습니다. 내용은 유지했습니다.

현재 확인 요청에 대한 답변 대기는 없습니다. 커밋·push·배포는 별도 요청 없이 진행하지 않습니다.

## 모노톤 디자인 변경 — 2026-11-17

소유자의 디자인 변경 요청에 따라 적용했습니다.

- 기본 모드를 다크로, 강조색을 무채색 `zinc`로 설정했습니다. 밝은 모드 선택 기능은 유지합니다.
- 메인 소개 영역의 초록색 배경을 무채색으로 변경했습니다. 후속 요청에 따라 곡선 패턴·점무늬·은은한 명암을 더했습니다. 경력·수상·기술 영역의 초록색 제목·선도 무채색으로 변경했습니다.
- 공통 스타일은 `assets/css/custom.css`에서 관리합니다. 홈에 중복되던 인라인 스타일 4개를 분리했습니다.
- 홈 프로젝트 목록은 `layouts/partials/views/project-list*.html`을 사용합니다. 정사각형 `Fill` 크롭 대신 `Fit`으로 원본 비율을 보존하고 `object-fit: contain`으로 이미지 전체를 표시합니다. 데스크톱은 이미지·설명 2열, 모바일은 1열입니다.
- 이미지에 적용되던 확대 호버 효과와 카드 그림자를 제거하고, 제목의 밑줄 및 키보드 포커스로 상호작용을 표시합니다.
- 프로젝트 이미지 8개의 원본·생성 이미지 종횡비를 비교해 보존을 확인했습니다. HTML 73개의 표시 텍스트·링크·앵커는 변경 전과 동일합니다.
- Safari에서 데스크톱 메인·프로젝트, 390px 폭의 모바일 프레임, 밝은 모드, 다크 모드 및 SNAP 검색 결과를 확인했습니다.

로컬 확인 주소: `http://127.0.0.1:1313/?preview=monochrome`.

## 후속 개선 — 이모지·News·소개 패턴

- News 및 프로필 이모지에 적용했던 무채색 필터를 제거해 원래 색상으로 복원했습니다.
- News 16개는 날짜·이모지·본문을 보존한 구조화 항목으로 옮겼습니다. 최근 10개만 기본 표시하고, 나머지 6개는 `Show more`를 눌러 펼치며 `Show less`로 다시 접습니다. 새 항목을 추가해도 10개 기준으로 자동 분리합니다.
- 후속 요청에 따라 펼치기 UI의 숫자·화살표·배경·테두리를 제거해 텍스트만 표시합니다. 키보드 사용 시 포커스 표시는 유지합니다.
- 접기는 네이티브 `details`/`summary`로 구현해 별도 JavaScript 없이 동작합니다. 마우스 클릭으로 펼치기와 스페이스 키로 접기를 Safari에서 확인했습니다.
- 날짜·이모지·본문을 데스크톱에서는 한 줄의 열로, 390px 모바일 폭에서는 날짜를 본문 위로 배치했습니다. 숨겨진 이전 소식도 검색 인덱스에 유지하며, 펼치기 버튼 문구는 검색에서 제외합니다.
- 소개 영역에는 SVG 곡선·점 패턴, 부드러운 명암, 반투명 프로필 카드와 얇은 테두리를 적용했습니다. 패턴은 해시가 붙은 상대 경로로 제공해 로컬과 배포 환경에서 모두 표시됩니다.
- 모바일 및 밝은·어두운 모드에서 소개 영역과 News를 시각 확인했습니다. News 기본 10개·이전 6개, 기존 뉴스 내용·링크·앵커 보존, 배경 리소스 응답, 이전 소식의 검색 포함을 검증했습니다.

최신 미리보기: `http://127.0.0.1:1313/?preview=refined-v3`.

## 확인한 외부 근거

- Beyond Hearing의 학회 연도는 연구실 공식 프로젝트에 ICLR 2026으로 명시되어 있습니다. [연구실 프로젝트](https://miil.kaist.ac.kr/projects/beyondhearing/)
- Beyond Hearing의 저자 순서 및 첫 네 명의 공동기여는 연구실 공개 PDF 첫 페이지에 명시되어 있습니다. [논문 PDF](https://miil.kaist.ac.kr/pdf/ICLR26_BeyondHearing.pdf)
- IMG2IMU의 최종 게재 정보는 IEEE TMC 24권 9호, 2025년 9월입니다. DOI는 `10.1109/TMC.2025.3556998`입니다. [KAIST 연구 성과 기록](https://pure.kaist.ac.kr/en/publications/from-vision-to-motion-translating-large-scale-knowledge-for-data-/), [연구실 공개 논문](https://nmsl.kaist.ac.kr/pdf/IEEE_Mobile_computing25_IMG2IMU.pdf)
- SNAP은 NeurIPS 2025 공식 proceedings에 등재되어 있습니다. [공식 논문 페이지](https://papers.nips.cc/paper_files/paper/2025/hash/820e42f39773c6cbbd875553db45658f-Abstract-Conference.html)
- ICLR 2026 메인 학회는 4월 23일 시작합니다. [학회 일정](https://iclr.cc/Conferences/2026/Dates)
- 검색 범위는 Pagefind의 `exclude_selectors` 공식 설정을 사용했습니다. [Pagefind 설정 문서](https://pagefind.app/docs/config-options/)

공식 IEEE·OpenReview 페이지 일부는 봇 확인 화면으로 본문을 읽을 수 없었습니다. 해당 항목은 연구실 공개 PDF·프로젝트 및 KAIST 기록으로 대조했습니다. 자료 확인만으로 핵심 사실을 임의 변경하지 않았습니다.

## 검증과 배포 상태

- Hugo Extended 0.126.1 production 빌드 성공, 레이아웃 경고 없음.
- 2026-11-06 정리에서는 승인된 소개문·기준 URL 이외 표시 텍스트·링크·이미지 참조를 비교해 유지 확인.
- 최종 생성 HTML 73개, 검색 문서 45개. 빈 Talks의 본문·리다이렉트 2개와 검색 문서 1개가 제외됨.
- 검색 문서에서 공통 메뉴·푸터가 빠졌으며 홈·SNAP 등 콘텐츠는 유지됨을 확인.
- 활성 배포는 GitHub Pages 워크플로 하나이며 Pagefind 1.6.0 사용. Netlify 전용 `_headers`·`_redirects` 출력 제거.
- Netlify 제거 전·후 HTML 73개의 경로·링크·앵커·인라인 스타일·미디어 참조가 동일하며 홈 표시 텍스트도 동일함을 비교 확인. 내부 링크·파일·앵커 대상 누락 없음. 프로젝트 8개·논문 5개 유지.
- 짧게 바꾼 세 요약의 `abstract`는 Git 원본과 동일. CV는 바이트 단위로 원본과 동일. 보관한 BibTeX 워크플로도 원본과 동일.
- 브라우저 탭 연결은 사용할 수 없었지만, 모노톤 디자인 변경 시 네이티브 Safari를 통해 데스크톱·모바일 폭·테마 전환·검색 UI를 확인함.
- 소스는 `content/`와 `config/`에서 수정. `public/index.html`은 생성 결과이므로 직접 편집하지 않음.
- 소유자가 현재 변경사항 배포를 요청했습니다. `main` 반영·push 후 GitHub Pages 워크플로를 사용합니다. 실행 이력과 결과는 [GitHub Actions](https://github.com/chahh9808/chahh9808.github.io/actions/workflows/publish.yaml)에서 확인할 수 있습니다.
