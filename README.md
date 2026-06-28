# 부농이네집 — 배포 (AltStore Source)

집 IoT 컨트롤러 앱 **부농이네집**(HomeTwin)의 AltStore 사이드로드 배포용 레포.
**소스코드·시크릿 없음** — 컴파일된 IPA(미서명)와 AltStore manifest만 둔다.
(앱은 HA 주소·토큰을 런타임에 입력받으므로 IPA 바이너리엔 비밀이 없다.)

## 설치 (한 번만)
AltStore → **Browse** 탭 → 우상단 source 추가 → 아래 URL 입력:

```
https://raw.githubusercontent.com/dongKos/hometwin-dist/main/altstore-source.json
```

그 뒤 source 목록에서 **부농이네집** → GET. 재서명은 집 Mac(AltServer)이 같은 Wi-Fi에
켜져 있을 때 자동으로 된다.

## 업데이트
새 버전이 올라오면 AltStore **My Apps** 에 업데이트 배지가 뜬다 → **UPDATE** 한 번.
(전송·파일 선택 불필요.)

## 만료
무료 인증서라 7일 후 만료. AltStore가 집 Wi-Fi에서 자동 갱신(background refresh)하거나,
수동으로 My Apps에서 새로고침하면 된다.
