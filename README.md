# YouTube 분석 (ULTRA+ v3.4)
단일 파일(index.html)로 동작하는 유튜브 분석기입니다.

## 공통 사용법
1) 페이지를 열고 상단에 다음을 입력합니다.
   - API 키(직접 호출 모드일 때만 필요)
   - Google Apps Script Web App URL (Sheets 자동 업로드용)
2) '연결 진단'으로 API 확인 → '다중 키워드 실행'으로 수집/분석합니다.
3) 자동 업로드=켜기면 결과가 Google Sheets `Results` 시트에 기록됩니다.

### 보안
- Google Cloud Console → API 키의 애플리케이션 제한: HTTP referrers
- 허용 도메인에 배포 도메인(예: *.github.io, *.netlify.app, *.vercel.app, 커스텀)을 추가하세요.

## GitHub Pages 배포
1. 이 폴더의 파일을 GitHub 새 저장소에 업로드합니다.
2. 저장소를 Public으로 전환합니다 (Settings → General → Change repository visibility → Public).
3. Settings → Pages → Build and deployment
   - Source: Deploy from a branch
   - Branch: main / Folder: /(root) → Save
4. 잠시 후 표시되는 주소( https://<user>.github.io/<repo>/ )로 접속합니다.
