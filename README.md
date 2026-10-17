# 작은 우주 탐험 · SPACE CLUB

우주에 관한 10문항을 풀며 배우는 한국어 퀴즈 앱입니당. 정답마다 10점을 받고 해설을 확인할 수 있으며, 탐험을 마치면 최종 점수와 복습 목록이 표시됩니당. 문제 순서 섞기와 틀린 문제만 복습하는 필터도 제공합니당.

## 로컬 실행

저장소를 내려받은 뒤 프로젝트 루트에서 Windows PowerShell로 다음 명령을 실행하면 기본 브라우저에서 열립니당.

```powershell
Start-Process .\index.html
```

다른 운영체제에서는 `index.html`을 브라우저로 직접 열면 됩니당. CSS, JavaScript, SVG가 모두 파일 하나에 포함되어 있어 서버 실행, 패키지 설치, 빌드나 외부 리소스 없이 `file://`로 동작합니당. 답변과 점수는 메모리에만 저장되며 새로고침하면 초기화됩니당.

## GitHub Pages 배포

게시 주소는 [https://mac-guffin.github.io/space-quiz/](https://mac-guffin.github.io/space-quiz/)입니당.

저장소의 **Settings → Pages → Build and deployment → Source**는 **GitHub Actions**로 설정합니당. `.github/workflows/pages.yml`은 PR에서 게시 파일 준비를 확인하고, `main`에 변경 사항이 반영되면 `index.html`만 아티팩트로 만들어 `github-pages` 환경에 배포합니당. 별도 컴파일 단계는 없으며 README나 저장소 설정 파일은 게시하지 않습니당.

**Actions → Deploy to GitHub Pages → Run workflow**에서 `main`을 선택해 수동으로 다시 배포할 수도 있습니당. 배포 결과는 해당 워크플로 실행과 저장소의 **Deployments**에서 확인할 수 있습니당.
