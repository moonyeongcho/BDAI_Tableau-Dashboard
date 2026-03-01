
# E-commerce Marketing Analytics

## 1. 프로젝트 개요
이커머스 플랫폼 사용자 행동/마케팅 데이터를 기반으로 유입부터 구매까지 흐름을 시각화한 대시보드입니다.
유입 채널 성과, 퍼널 단계별 전환율, 리텐션, 매출 및 마진, 로열티 등급별 성과를 한 화면에서 빠르게 확인할 수 있습니다. 

## 2. 대시보드 구성 
워크시트 5개 + 대시보드 1개로 구성되어 있습니다.

- Worksheet 1: Acquisition  
  - 유입 채널별 유입 사용자 수 비교
  - 날짜별 유입 트렌드 확인(영역/라인)

- Worksheet 2: Activation  
  - event_type 기반 퍼널 정의
  - 단계별 전환율 계산 및 퍼널 차트로 이탈 구간 확인

- Worksheet 3: Retention  
  - 첫 구매 기준 재구매 여부로 리텐션 정의  
  - 막대 차트로 재구매 지속성 확인

- Worksheet 4: Loyalty  
  - 로열티 등급별 고객 특성 비교
  - 버블 차트: X=평균 주문 금액(AOV), Y=평균 구매 전환율, 크기=고객 수  
  - 평균선 및 추세선 포함

- Worksheet 5: KPI Cards  
  - 총 유입 사용자 수, 구매 전환율, 평균 주문 금액(AOV), 마진율, 재구매율 요약

## 3. 대시보드 레이아웃 및 인터랙션
- 레이아웃: 세로형(스크롤 가능한 구조)  
- 상단(Header): KPI 요약 카드  
- 중앙/하단: 워크시트 1~4 요약 시각화 
- 좌측: 날짜, 로열티 등급 필터

## 4. 배포 및 공유 방식
GitHub 에서는 대시보드가 실행되지 않기 때문에, 아래 링크에 들어가면 동적 대시보드를 확인할 수 있습니다.

Tableau Public link
- https://public.tableau.com/app/profile/moonyeong.cho/viz/MarketingE-CommerceDashboard2/1

## 5. 결과 스크린샷
- assets/dashboard_overview.png
- assets/ws1_acquisition.png
- assets/ws2_activation.png
- assets/ws3_retention.png
- assets/ws4_loyalty.png
- assets/ws5_kpi.png

README에 이미지 표시 예시:
![AARRR Dashboard](assets/dashboard_overview.png)

## 6. 파일 안내
- /assets/ : 대시보드 및 워크시트 스크린샷
- /tableau/ : 태블로 twbx 파일
- (/docs/ : 지표 정의 및 계산식 정리)

## 7. 데이터
- Marketing & E-Commerce Analytics Dataset (Kaggle)
  (sediment://file_000000003e88720b8d9a0aaf9e70b23f)
