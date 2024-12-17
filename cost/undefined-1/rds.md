---
description: RDS Reserved Instance Reports
---

# RDS 예약 인스턴스 보고서

이 보고서는 AWS 계정 내에서 구매한 RDS 예약 DB 인스턴스에 대한 요약을 제공합니다.

이 보고서에 액세스하려면 왼쪽 탐색 창으로 이동하여 \
**Cost > Reserved Usage > Inventory > RDS > RDS Reserved DB Instance Summary**를 선택합니다.

## 요약 <a href="#summary" id="summary"></a>

이 보고서는 구매한 예약에 대한 통계와 완전히 활용되고 있는지 여부를 제공합니다.

<details>

<summary>더 읽어보기</summary>

* Total Instance Count for Active Reserved DB Instances  - 구매한 총 예약 수입니다.
* Total Active Reserved DB Instances - 구매하여 사용할 수 있는 예약 DB 인스턴스의 수 \
  입니다.
* Total Retired Reserved DB Instances - 만료되어 사용할 수 없는 예약 DB 인스턴스의 수 \
  입니다.
* Total DB Instances Running as Reserved  - 예약 요금을 사용하는 실행 중인 \
  총 DB 인스턴스 수입니다.
* Total number of DB instances - 예약 DB 인스턴스로 청구되는 총 DB 인스턴스 수입니다.
* Total DB Instance Count for Unused Reserved Instances - 구매했지만 실행 중인 RDS DB 인스턴스에서 사용하지 않는 예약 DB 인스턴스의 수입니다.
* Total On-Demand DB Instances Not Using Reserved DB Instance - 온디맨드로 시작되고 예약 요금을 사용하지 않는 DB 인스턴스의 수입니다.

</details>

**Reserved DB Instances By Region**

이 섹션에서는 활성 예약이 있는 AWS 리전을 보여주는 원형 차트를 제공합니다.

**Reserved DB Instances By Size**

이 섹션의 파이 차트는 구매한 예약의 데이터베이스 크기(r3.2xlarge, m3.medium 등)를 보여줍니다.

**Reserved DB Instances By Utilization**

이 원형 차트는 사용 유형(light, medium, or heavy)별로 예약 내역을 보여줍니다.

**List of Reserved DB Instances**

예약 DB 인스턴스 목록에서 RDS 예약 인스턴스를 더 자세히 살펴볼 수 있습니다. 필요한 데이터를 볼 수 있도록 다양한 필터를 제공합니다. 현재 제공되는 필터 및 열은 다음과 같습니다.

* Reservation ID (예약 ID)
* Offering Type (오퍼링 유형)
* Region (지역)
* DB Instance Class (DB 인스턴스 클래스)
* Product Description (제품 설명)
* Multi AZ (멀티 가용영역)
* Duration (지속)
* Time Left (남은 시간)
* Upfront Fee (선결제 옵션)
* Hourly Price (시간당 가격)
* Instance Count (인스턴스 수)
* Instances Used (사용된 인스턴스)

표시할 결과 수와 다양한 정렬 기준 옵션을 제한하도록 선택할 수도 있습니다. \
거의 모든 보고서와 마찬가지로 CSV 또는 PDF로 결과를 내보낼 수 있습니다.

## RDS RI 구매 추천 <a href="#rds_ri_purchase_recommendations" id="rds_ri_purchase_recommendations"></a>

이 보고서는 최적의 예약 DB 인스턴스 사용으로 가능한 비용 절감을 보여줍니다. 구매할 권장 예약 DB 인스턴스의 전체 목록을 제공하고 각각의 비용과 절감액을 보여줍니다. 예약 DB 인스턴스를 구매하면 Amazon RDS DB 인스턴스를 대폭 할인된 가격으로 사용할 수 있습니다. 예약 DB 인스턴스는 더 낮은 시간당 요금에 대한 대가로 선불 요금이 필요합니다. 예약 DB 인스턴스는 사용량을 예측할 수 있는 경우 상당한 절감 효과를 제공합니다. 각 권장 사항에는 인스턴스 및 권장 예약에 대한 중요한 정보가 포함되어 있습니다. 이 보고서에서는 온디맨드 및 예약 인스턴스 비용과 실행 시간을 비교합니다.

액세스하려면 왼쪽 탐색 창으로 이동하여 \
**Cost > Reserved Usage > Recommendations > RDS > Purchase**를 선택합니다.

## 비교 요약 <a href="#comparison_summary" id="comparison_summary"></a>

이 보고서는 예약 인스턴스 요금으로 전환할 경우 절약할 수 있는 금액을 보여줍니다. 현재 사용하는 양을 계산한 다음 예약 인스턴스 가격으로 전환할 경우 예상 사용량을 기준으로 해당 수치가 어떻게 되는지 보여줍니다. 1년과 3년에 걸쳐 비용을 분석하고 다양한 활용 선택에 중점을 둡니다.

액세스하려면 왼쪽 탐색 창으로 이동하여 \
**Cost > Reserved Usage > Inventory > RDS > Comparison Summary**를 선택합니다.

## 비교 세부 정보 <a href="#comparison_detail" id="comparison_detail"></a>

이 보고서에서는 모든 현재 DB 인스턴스를 나열한 다음 이전 보고서의 형식에 따라 예상 사용 비용을 다양한 비용 범주로 분류하여 해당 특정 인스턴스를 예약 요금으로 전환할 경우 절약할 수 있는 금액을 설명합니다.

액세스하려면 왼쪽 탐색 창으로 이동하여 \
**Cost > Reserved Usage > Inventory > RDS > Comparison Details**를 선택합니다.
