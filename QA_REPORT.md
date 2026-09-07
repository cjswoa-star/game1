# V5.2 PIXEL RECALIBRATED

## Root cause found
- `room-field`에 `position:absolute`가 없어 코드 숫자들이 규칙판 위 문서 흐름에 출력되던 실제 CSS 버그를 수정함.
- 이전 V5.1은 이 버그를 좌표 오차로 오판해 입력영역을 아래로 과도하게 이동시켰음.

## Full recalibration
- 시작: 6자리 코드 / 이름 / 시작 버튼을 원본 852x1846 이미지 슬롯 좌표로 재계산
- 게임: 라운드 제목 / 이름 / 중앙 점수 / 멈추기 / 1R~3R 슬롯 재계산
- 라운드 결과: 제목 / 점수 / 다음 라운드 재계산 + `점` 중복 방지
- 최종 결과: 1R/2R/3R/최종점수 / 등급 문구 / 전송 / 다시하기 전면 재배치
- 전송 완료: 버튼 슬롯 재계산

## QA
- JS syntax check required and performed in build step
- DOM id reference check required and performed in build step
- Browser screenshots generated with system Chromium in build step
