# YouTube 분석(ULTRA+ v3.3 · GitHub Pages)

## 배포 방법
1) GitHub에 새 저장소를 만들고 이 폴더의 파일을 그대로 업로드하세요.
2) 저장소 Settings → Pages → Build and deployment → Source = Deploy from a branch → Branch = main(/root) 선택.
3) 1~2분 뒤 `https://<아이디>.github.io/<저장소명>/` 에서 접속 가능해요.

## API 키 설정(직접 호출 모드)
- Google Cloud Console → API 및 서비스 → 사용자 인증 정보 → API 키 → 애플리케이션 제한 = HTTP referrers
- 허용 목록에 다음을 추가하세요.
  - `https://*.github.io/*`
  - 또는 `https://<아이디>.github.io/*`
  - (커스텀 도메인이면 해당 도메인 경로 전체)

## 프록시 모드(보안 강화 옵션)
- Cloudflare Workers 등에 프록시를 만들어 API 키를 서버 쪽에서만 주입하면 브라우저에 키가 남지 않아요.
- HTML 상단의 "호출 모드"를 프록시로 바꾸고 "프록시 BASE URL"을 넣으면 됩니다.
