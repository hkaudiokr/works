# works-main (사이트관리센터)

이 저장소는 `works.ainsonic.com`으로 배포되는 **사이트관리센터**입니다. `<meta name="robots" content="noindex,nofollow">`로 비공개(검색 미노출) 상태를 유지합니다.

## 서비스 구성 (공식 명칭)

| 서비스명 | 도메인 | 공개 여부 |
|---|---|---|
| 아인소닉 홈페이지 | www.ainsonic.com | 공개 |
| 프로오디오뉴스 | news.ainsonic.com | 공개 |
| 사이트관리센터 | works.ainsonic.com | 비공개 (본 저장소) |

## 역할

- `index.html`의 "업무센터" 카드는 기존 Google Apps Script 관리 화면(URL 변경 없음)으로 연결됩니다.
- 업무센터에서 입력한 공지사항·배너는 정기 작업을 통해 두 공개 사이트(아인소닉 홈페이지의 `notices.json`/`banners.json`, 프로오디오뉴스의 `notices.json`)에 자동 반영됩니다.
- 공개 사이트(아인소닉 홈페이지, 프로오디오뉴스)의 상단 내비게이션에는 본 사이트(사이트관리센터) 링크를 노출하지 않습니다. 기존에도 노출된 적이 없어 그대로 유지합니다.

## 변경 금지 사항

- GAS 관리 링크(exec URL)는 운영 중인 백엔드이므로 임의로 교체하지 않습니다.
- `CNAME`(works.ainsonic.com)은 변경하지 않습니다.
