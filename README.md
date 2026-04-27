# 비트코인 저축 현황 대시보드

나만의 Bitcoin DCA 트래킹 대시보드 — 아이폰 최적화, GitHub Pages 배포용

## 기능

- **과거 보유분 + DCA 통합 현황** — 20~22년 매수분과 월간 DCA를 합산해서 보여줌
- **실시간 BTC 가격** — 60초마다 자동 업데이트 (CoinGecko API)
- **월 1회 입력** — 매달 투자금 + BTC 증가량만 입력하면 끝
- **목표 BTC 진행률** — 목표 수량 설정 & 진행 상황 시각화
- **누적 차트** — 투자금 vs 평가금액 월별 추이
- **데이터 저장** — localStorage에 자동 저장 (앱 재시작해도 유지)

## GitHub Pages 배포 방법

### 1단계 — 저장소 만들기
1. GitHub에서 새 저장소 생성 (예: `bitcoin-dca`)
2. Public으로 설정

### 2단계 — 파일 업로드
파일 4개를 저장소에 업로드:
```
index.html
manifest.json
icon.png
icon-512.png
```

### 3단계 — Pages 활성화
1. 저장소 Settings → Pages
2. Source: Deploy from a branch
3. Branch: main / (root)
4. Save

### 4단계 — 접속
약 1~2분 후 `https://[username].github.io/bitcoin-dca/` 로 접속 가능

## 아이폰 홈 화면에 추가하는 방법

1. 사파리에서 위 주소 접속
2. 하단 공유 버튼(□↑) 탭
3. "홈 화면에 추가" 선택
4. 이름 확인 후 "추가"

앱처럼 전체화면으로 실행됩니다 🎉

## 입력 방법

### 처음 설정 (1회만)
- "과거 보유분 설정" 버튼
- 20~22년 총 투자금 (코인 손실분 포함해서 실제 쓴 돈 전체)
- 현재 BTC 보유량 입력

### 월간 입력 (매달 1회)
- "+ 월간 입력" 버튼
- 이번 달 Strike 투자금 (원화)
- 이번 달 개인지갑 BTC 증가량
- 같은 달 두 번 입력하면 덮어쓰기
