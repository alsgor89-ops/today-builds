# today-builds

하루 만에 뚝딱 만든 작은 웹 프로젝트 모음입니다. 각 프로젝트는 별도의 폴더에 있으며, 빌드 과정 없이 `index.html` 파일 하나로 바로 실행되는 순수 HTML/CSS/JavaScript 앱입니다.

## 프로젝트

### 🍅 [pomodoro-tasks](pomodoro-tasks/index.html) — Focus Flow
뽀모도로 타이머와 할 일 목록을 결합한 생산성 도구입니다.

- 집중 25분 / 짧은 휴식 5분 / 긴 휴식 15분 모드 전환
- 할 일을 선택해 "현재 작업"으로 지정하면 완료한 뽀모도로 횟수가 그 할 일에 누적됨
- 세션 종료 시 벨소리 알림
- 할 일 목록은 `localStorage`에 저장되어 새로고침해도 유지됨

### 🎨 [doodle-synth](doodle-synth/index.html) — Doodle Synth
화면에 그림을 그리면 소리가 나는 드로잉 신디사이저입니다.

- Y 좌표는 음높이, X 좌표는 좌우 패닝을 결정
- 6가지 색상, 4가지 파형(sine / triangle / sawtooth / square) 선택 가능
- 여러 손가락(포인터)으로 동시에 그리고 화음 만들기 가능
- Web Audio API로 실시간 사운드 생성

### ⌨️ [word-cascade](word-cascade/index.html) — Word Cascade
위에서 떨어지는 단어를 타이핑으로 없애는 타이핑 아케이드 게임입니다.

- 키보드로 화면에 보이는 단어를 입력하면 점수 획득
- 단어를 놓치면 목숨 감소(3개), 점수가 오를수록 레벨과 낙하 속도 증가
- 최고 점수는 `localStorage`에 저장

### 🌱 [habit-grid](habit-grid/index.html) — Habit Grid
GitHub 잔디밭 스타일로 습관을 기록하는 트래커입니다.

- 습관을 추가하고 하루 칸을 클릭해 완료 체크
- 현재 연속 기록과 최고 연속 기록을 자동 계산
- 10주치 잔디 그리드를 스크롤로 확인, `localStorage`에 저장

### ✨ [galaxy-particles](galaxy-particles/index.html) — Galaxy Particles
마우스로 조작하는 인터랙티브 파티클 아트 장난감입니다.

- 마우스를 움직이면 입자를 끌어당기거나(attract) 밀어내기(repel)
- 클릭하면 폭발 효과, 입자 개수·색상 테마 조절 가능
- Canvas 2D로 실시간 렌더링

### 🃏 [memory-match](memory-match/index.html) — Memory Match
카드를 뒤집어 짝을 맞추는 메모리 게임입니다.

- 4×4 / 6×6 난이도 선택
- 이동 횟수·시간 기록, 최고 기록은 난이도별로 `localStorage`에 저장
- 카드 뒤집기 3D 애니메이션

## 실행 방법

별도 설치 없이 각 폴더의 `index.html`을 더블클릭하거나 브라우저 창에 드래그하면 바로 실행됩니다.

로컬 서버로 띄우고 싶다면 (Windows PowerShell):

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File serve.ps1 -Port 8765
```

실행 후 브라우저에서 `http://localhost:8765/<프로젝트 폴더>/` 로 접속하면 됩니다.

## 기술 스택

프레임워크나 빌드 도구 없이 순수 HTML / CSS / JavaScript로만 작성했습니다. 외부 의존성이 없어 파일만 있으면 어디서든 바로 열립니다.

## 라이선스

[MIT](LICENSE)
