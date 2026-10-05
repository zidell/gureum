# 개인 포크 운영 지침

구름 입력기(gureum/gureum)의 개인용 포크(zidell/gureum)다. 원본에 PR을 보내지 않고, 빌드 배포도 하지 않는다.

- 포크 수정은 `enter-after-commit` 브랜치에 둔다. 현재 수정은 `OSXCore/InputReceiver.swift`의 조합 중 엔터 즉시 전송 하나다
- 원본 갱신은 rebase 말고 `merge origin/main`으로 한다. 원본 이슈 #892 댓글에 건 커밋 링크(6e03ee3)가 깨지지 않게 하기 위해서다
- ad-hoc 서명이라 새로 설치할 때마다 손쉬운 사용 권한이 초기화된다. 권한을 다시 켠 뒤 `killall Gureum`으로 재시작해야 반영된다. 재시작하지 않으면 거부 상태가 캐시되어 엔터가 예전처럼 확정만 된다
- `OSX/Version.xcconfig`는 빌드가 자동으로 고치는 파일이라 커밋하지 않는다
