# 짱박이 Jjangbaki - 지하철 문 방향 안내

수도권 지하철 경로를 찾으면 **역마다 어느 쪽 문이 열리는지**, 중간 역에서 **덜 열리는 쪽(짱박 자리)**, 빠른 환승 칸, 탈 열차의 시각을 한눈에 보여 주는 웹 도구입니다.
설치도 가입도 없이 주소만 열면 됩니다. 한국어와 영어로 볼 수 있습니다.

> 📝 소개 글: [네이버 블로그](https://blog.naver.com/henmoogi/224469900397) · [구글 블로거](https://henmoogi.blogspot.com/2026/11/seoul-subway-door-side.html) · 문의·후기는 블로그 댓글로

## 👉 바로 쓰기

**https://henmoogi.github.io/jjangbaki/**

1. 노선도에서 출발역과 도착역을 누르거나, '역 이름으로 찾기'에서 역 이름을 입력합니다.
2. 경로는 **아래에서 위로** 읽습니다. 출발역이 맨 아래, 도착역이 맨 위입니다.
3. 칸마다 '탈 때 / 짱박 자리 / 내릴 때'가 나옵니다. 짱박 자리 쪽 문 앞에 서면 중간 역에서 덜 밀립니다.
4. 오른쪽 위 **EN** 단추로 영어 화면으로 바꿀 수 있습니다. 처음 열 때는 휴대폰·브라우저 언어가 한국어가 아니면 영어로 열립니다.

## 기능

- 수도권 24개 노선 경로 검색(환승, 분기, 2호선 순환, 6호선 응암순환)
- 역마다 내리는 문 방향과 문이 열리는 순서, 덜 열리는 쪽 자리
- 출발 시각을 고르면 시간표로 탈 열차, 기다리는 시간, 다음 열차, 막차, 역마다 서는 시각
- 빠른 환승 칸·문(서울교통공사 자료 범위)
- 역 이름을 누르면 그 이름이 어디서 왔는지(역명 유래)
- 문 방향이 틀렸으면 문 표시를 눌러 고칠 수 있습니다. 고친 값은 **이 기기에만** 저장됩니다.

## 서버로 보내는 것이 없습니다

- 페이지는 HTML 파일 하나(`index.html`)와 노선별 시간표 파일(`tt/`)뿐입니다. 고른 역이나 고친 값은 브라우저 안에만 저장됩니다.
- 외부에서 불러오는 것은 글꼴(Google Fonts)뿐입니다.

## 한계

- 문 방향은 공식 승강장 자료와 노선의 통행 방향으로 계산했지만, 일부 역(130곳)은 아직 커뮤니티 정리 자료입니다. 타 보고 다르면 고쳐 쓰세요.
- 시간표는 평일과 토·휴일 두 가지입니다. 2호선 토·휴일과 2호선 성수·신정 지선, 9호선 급행은 시간표가 없어 어림으로 보여 줍니다. 지연이나 임시 열차는 반영하지 않습니다.
- 경로는 역 사이 거리로 고르고, 그 경로에 맞는 열차를 시간표에서 찾아 붙입니다.
- 철도 운영기관의 공식 서비스가 아닙니다. 개인이 만든 도구입니다.

자료 출처와 이용 조건은 [DATA_SOURCES.md](DATA_SOURCES.md)에 있습니다.

---

## English

**Jjangbaki** shows, for a route on the Seoul metropolitan subway, **which side the doors open at every stop**, the **quiet side** (the side whose doors open least on the way, so fewer people push past you), quick-transfer cars and the times of the train you would catch.
No install, no sign-up: open **https://henmoogi.github.io/jjangbaki/** and tap **EN** at the top right (it opens in English by default when your phone or browser is not set to Korean).

- Pick stations on the map or search by name (English or Korean).
- The route reads **from bottom to top**: your start station is at the bottom.
- Each ride shows Board / Quiet side / Get off, the door order, and train times from the timetable.
- Tap a station name to see where the name comes from. Notes from Seoul Metro and our own short notes are translated; for other stations only the operator's Korean text is available.
- Nothing is sent to a server. Door fixes you make are stored on your device only.
- This is a personal project, not an official service of any rail operator. Data sources and terms: [DATA_SOURCES.md](DATA_SOURCES.md).

## 라이선스 License

코드는 [MIT](LICENSE)입니다. 자료는 각 출처의 이용 조건을 따릅니다([DATA_SOURCES.md](DATA_SOURCES.md)). 무보증입니다.
The code is [MIT](LICENSE) licensed; the data follows the terms of each source. No warranty.
