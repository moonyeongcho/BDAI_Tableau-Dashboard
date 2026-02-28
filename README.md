
# Foodpanda Customer Dashboard (Tableau)

## 1. 프로젝트 개요
푸드판다(Foodpanda)는 음식 배달과 픽업 서비스를 제공하는 글로벌 배달 플랫폼입니다.
본 프로젝트는 푸드판다 주문 데이터 기반으로 주문 매출 트렌드와 주요 고객 지표를 한 화면에서 확인할 수 있는 고객 분석 대시보드를 제작했습니다.
목표는 신규 유입이 지속되는 상황에서 충성 고객 유지와 이탈 위험 고객 파악에 도움이 되는 대시보드를 제공하는 것입니다.

## 2. 대시보드를 통해 확인할 수 있는 것
- 레스토랑 평균 평점과 평균 주문 빈도 관계 (버블 차트)
- 신규 가입 날짜 기준 활성 고객과 비활성 고객 비중 추이 (영역 그래프)
- 고객 연령대 구성비 (도넛 차트)
- 도시별 고객의 평균 로열 포인트롸 평균 주문 빈도 (텍스트 테이블)
- 핵심 KPI(총 주문 유저 수, 고객별 평균 평점, 주문 완료율, 평균 주문 빈도) 시각화
  
## 3. 구성물
워크시트 5개와 고객 대시보드 1개로 구성했습니다.

- Worksheet 1: Restaurant Bubble Chart
  - 평균 평점 vs 평균 주문 빈도 버블 차트
  - 버블 크기: 주문 수
  - 평균선 추가, 마크 도형 변경

- Worksheet 2: Churn share Area Chart
  - 신규 가입 날짜 기준 활성/비활성(이탈) 고객 비중 영역 그래프

- Worksheet 3: Age Donut Chart
  - 고객 연령 비중 도넛 차트
  - 도넛 내부에 총 고객 수 레이블
  - 연령 레이블 및 비중 표시

- Worksheet 4: City x Customer Text Table
  - 도시별 고객(또는 주문) 단위로 평균 로열 포인트, 평균 주문 빈도 텍스트 테이블

- Worksheet 5: KPI cards
  - 총 주문 유저 수
  - 고객별 평균 평점
  - 주문 완료율
  - 평균 주문 빈도

- Dashboard: Customer Dashboard
  - 상단: KPI 카드 4개
  - 중앙/하단: 워크시트 1~4 배치
  - 좌측: 필터 패널(지역, 날짜 연도)

## 4. 인터랙션
- Navigation bar(좌측): Overview / Customer 버튼으로 다른 대시보드 탐색
- Filters(좌측 패널): 지역, 날짜 연도 필터 연동
- Tooltip / Highlight: 차트별 마우스오버, 선택 시 맥락 정보 확인

## 5. 배포 및 공유 방식
GitHub README에서는 대시보드가 동적으로 실행되지 않기 때문에, 아래 방식으로 공유합니다.

- Readme: 링크
- Dashboard File: 스크린샷(정적)
- Interactive link: Tableau Public(또는 Tableau Server) 공개 링크로 제공

Tableau Public link:
- (여기에 공개 링크를 붙여 넣으세요)

## 6. 결과 스크린샷
- assets/tableau/dashboard_overview.png
- assets/tableau/dashboard_customer.png
- assets/tableau/ws1_bubble.png
- assets/tableau/ws2_area.png
- assets/tableau/ws3_donut.png
- assets/tableau/ws4_table.png
- assets/tableau/ws5_kpi.png

## 7. 파일 안내
- /assets/tableau/ : 스크린샷 이미지
- /tableau/ : twbx 또는 작업 파일(공유 가능 범위에서)
- /docs/ : 지표 정의, 계산식 정리(선택)

## 8. 지표 정의(예시 텍스트)
- 주문 완료율: 완료 주문 수 / 전체 주문 수
- 평균 주문 빈도: 고객별 주문 수를 기간으로 정규화한 평균(프로젝트 기준 정의)
- 고객별 평균 평점: 고객이 경험한 주문(또는 레스토랑)의 평점 평균(프로젝트 기준 정의)
- 총 주문 유저 수: 주문 발생 고객 수(중복 제거)
