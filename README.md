# [ZLE.KR](https://zle.kr)

## 주요 기능

### [사용자 등록](https://github.com/OUS-KR/ZLE.KR/issues/new?template=01-user-register-by-issue.yml)

- `ZLE.KR/u/{사용자 아이디}` 주소 기반의 사용자 등록
  - 사용자 예제: [ZLE.KR/u/zle](https://zle.kr/u/zle)
  - [사용자 등록 예제](https://github.com/OUS-KR/ZLE.KR/issues/1)
- `ZLE.KR/@{사용자 아이디}` 형태의 짧은 주소 지원
  - 사용자 예제: [ZLE.KR/@zle](https://zle.kr/@zle)
- 부적절한 아이디 (욕설, 관리자 등)는 제한되어 등록 시 삭제

### [사용자 단축주소 생성](https://github.com/OUS-KR/ZLE.KR/issues/new?template=02-user-short-url-register-by-issue.yml)

- `ZLE.KR/u/{사용자 아이디}/{단축 경로}` 형태의 단축주소 생성
  - 사용자 단축주소 예제: [ZLE.KR/u/zle/links/zle-kr](https://zle.kr/u/zle/links/zle-kr)
  - [사용자 단축주소 등록 예제](https://github.com/OUS-KR/ZLE.KR/issues/2)
  - 동일한 단축 경로 존재 시 덮어쓰기
- `ZLE.KR/@{사용자 아이디}/{단축 경로}` 형태의 짧은 주소 지원
  - 사용자 단축주소 예제: [ZLE.KR/@zle/links/zle-kr](https://zle.kr/@zle/links/zle-kr)
- 단축 경로가 `links`로 시작하면 `ZLE.KR/@{사용자 아이디}/!{links를 제외한 단축 경로}` 형태로 생략 가능
  - 사용자 단축주소 예제: [ZLE.KR/@zle/!zle-kr](https://zle.kr/@zle/!zle-kr)

### [사용자 글 작성](https://github.com/OUS-KR/ZLE.KR/issues/new?template=03-user-article-writing-by-issue.yml)

- `ZLE.KR/u/{사용자 아이디}/{글 경로}` 형태의 글 작성
  - 사용자 글 예제: [ZLE.KR/u/zle/articles/example](https://zle.kr/u/zle/articles/example)
  - [사용자 글 작성 예제](https://github.com/OUS-KR/ZLE.KR/issues/3)
  - 동일한 글 경로 존재 시 덮어쓰기
  - 글 경로 미입력 시 `ZLE.KR/u/{사용자 아이디}/` 페이지 수정
- `ZLE.KR/@{사용자 아이디}/{글 경로}` 형태의 짧은 주소 지원
  - 사용자 글 예제: [ZLE.KR/@zle/articles/example](https://zle.kr/@zle/articles/example)
 
### [사용자 메뉴 설정](https://github.com/OUS-KR/ZLE.KR/issues/new?template=04-user-menu-setting-by-issue.yml)

- 사용자 단축주소 및 글 페이지에 들어갈 메뉴 설정
  - [사용자 메뉴 설정 예제](https://github.com/OUS-KR/ZLE.KR/issues/4)

## 사용 방법

- [Issues 메뉴](https://github.com/OUS-KR/ZLE.KR/issues) 이동
- [New issue 버튼](https://github.com/OUS-KR/ZLE.KR/issues/new/choose) 클릭
- 기능 선택 후 폼 작성

## 기타 기능

### 유튜브 단축주소

- 유튜브 영상: `ZLE.KR/yt/{유튜브 영상 아이디}`
  - 예제: [ZLE.KR/yt/1ZX1vEDTfY4](https://zle.kr/yt/1ZX1vEDTfY4), [ZLE.KR/yt/yebNIHKAC4A](https://zle.kr/yt/yebNIHKAC4A)
- 유튜브 영상 + 시작 시간 옵션: `ZLE.KR/{유튜브 영상 아이디}/{시작 시간}`
  - 예제: [ZLE.KR/yt/1ZX1vEDTfY4/1m6s](https://zle.kr/yt/1ZX1vEDTfY4/1m6s), [ZLE.KR/yt/yebNIHKAC4A/56](https://zle.kr/yt/yebNIHKAC4A/56)
- 유튜브 영상 썸네일: `ZLE.KR/yt/img/{유튜브 영상 아이디}`
  - 예제: [ZLE.KR/yt/img/1ZX1vEDTfY4](https://zle.kr/yt/img/1ZX1vEDTfY4), [ZLE.KR/yt/img/yebNIHKAC4A](https://zle.kr/yt/img/yebNIHKAC4A)
- 유튜브 채널 RSS: `ZLE.KR/yt/rss/{유튜브 채널 아이디}`
  - 예제: [ZLE.KR/yt/rss/UC-Fnix71vRP64WXeo0ikd0Q](https://zle.kr/yt/rss/UC-Fnix71vRP64WXeo0ikd0Q)

#### 마크다운 작성 시 사용 방법

- 유튜브 영상 썸네일 링크: `[![{유튜브 영상 썸네일 텍스트}]({유튜브 영상 썸네일 주소})]({유튜브 영상 주소})`
  - 예제: `[![FIFTY FIFTY (피프티피프티) 'Pookie' Official MV](https://ZLE.KR/yt/img/1ZX1vEDTfY4)](https://ZLE.KR/yt/1ZX1vEDTfY4/1m6s)`
  [![FIFTY FIFTY (피프티피프티) 'Pookie' Official MV](https://ZLE.KR/yt/img/1ZX1vEDTfY4)](https://ZLE.KR/yt/1ZX1vEDTfY4/1m6s)
  - 예제: `[![“Golden” Official Lyric Video | KPop Demon Hunters | Sony Animation](https://ZLE.KR/yt/img/yebNIHKAC4A)](https://ZLE.KR/yt/yebNIHKAC4A/56)`
  [![“Golden” Official Lyric Video | KPop Demon Hunters | Sony Animation](https://ZLE.KR/yt/img/yebNIHKAC4A)](https://ZLE.KR/yt/yebNIHKAC4A/56)

## 주의사항

- 다음과 같은 콘텐츠 포함 시 제재
  - 불법 행위 또는 범죄를 조장하는 내용 (마약, 폭력, 성범죄, 불법 무기 등 관련 정보 유포 등)
  - 타인의 권리를 침해하는 내용 (명예훼손, 저작권 침해, 개인정보 유출, 초상권 침해 등)
  - 욕설, 비방, 혐오 표현 등 비하 또는 공격적인 내용 (특정 인종, 성별, 종교, 지역 등에 대한 혐오 발언 등)
  - 선정적이거나 성인 콘텐츠 (음란물, 성인용 콘텐츠, 성인 서비스 홍보 등)
  - 도박 또는 사행심을 유도하는 콘텐츠 (불법 도박 사이트 홍보, 사설 토토 등)
  - 허위 사실 유포 또는 사기성 콘텐츠 (거짓 정보, 피싱 링크, 투자 사기 등)
  - 광고 및 스팸성 콘텐츠 (반복적 홍보, 무단 상업 게시물, 무관한 링크 삽입 등)