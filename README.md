# lil_q Game Lab — 공개 사이트

게임별 개인정보처리방침을 모아두는 정적 사이트. **게임 소스와 분리된
저장소**다: GitHub Pages 는 무료 계정에서 공개 저장소만 지원하므로,
게임 코드를 비공개로 두면서 방침 페이지만 공개하려면 이렇게 나눠야 한다.

## 배포

1. GitHub 에 `<사용자명>.github.io` 이름으로 **공개** 저장소를 만든다.
2. 이 폴더를 그 저장소로 push 한다.
3. Settings → Pages → Source 를 `main` / `/ (root)` 로 둔다.

몇 분 뒤 아래 주소로 열린다:

```
https://<사용자명>.github.io/                              ← 랩 소개
https://<사용자명>.github.io/sudoku-mini/privacy.html      ← 1호 방침
```

## 게임을 추가할 때

`<게임-이름>/privacy.html` 폴더를 하나 더 만들고 `index.html` 에 링크를
추가한다. 방침 본문은 `sudoku-mini/privacy.html` 을 복사해 수집 항목표만
그 게임에 맞게 고치면 된다.

## app-ads.txt

루트의 `app-ads.txt` 는 "이 앱들의 광고 수익은 이 AdMob 게시자의 것"이라는
선언이다 (광고 사기 방지). **두 스토어 등록 정보의 '개발자 웹사이트'를
이 사이트 도메인으로 적어야** 구글이 이 파일을 찾아간다. 배포 후 AdMob
콘솔 → 앱 → app-ads.txt 에서 크롤링 상태를 확인할 것 (반영에 며칠 걸림).
