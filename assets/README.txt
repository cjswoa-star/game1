100점에 멈춰라! 최신 고정 ASSETS 기준본

01_start.png              852 x 1846
02_game.png               941 x 1672  ← 최신 승인된 '빈 원 + 0/25/50/75/100' 게임판
03_round_result.png       852 x 1846
04_final_result.png       852 x 1846
05_send_complete.png      852 x 1846
06_teacher_dashboard.png  1586 x 992

중요:
현재 기존 HTML의 student-screen은 852:1846 비율이며 .plate에 object-fit:fill이 설정되어 있습니다.
따라서 최신 02_game.png(941:1672)를 그대로 넣으면 세로로 늘어나 원이 타원처럼 보일 수 있습니다.
이는 assets 누락 문제가 아니라 2쪽 이미지의 종횡비와 HTML 프레임 종횡비가 다른 것이 직접 원인입니다.
2쪽만 941:1672 네이티브 비율을 사용하도록 코드를 맞추거나, 02_game 전용 레이아웃을 적용해야 합니다.
