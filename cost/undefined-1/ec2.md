---
description: EC2 Reserved Instance Summary Report
---

# EC2 예약 인스턴스 요약 보고서

EC2 예약 인스턴스 요약 보고서는 예약 인스턴스(RI) 사용량을 추적하고 RI가 최대한 활용되도록 합니다.

이 보고서에 액세스하려면 왼쪽 탐색 창으로 이동하여 \
**Cost > Reserved Usage > Inventory > EC2 > EC2 Reserved Instance Summary**를 선택합니다.

이 항목에서는 보고서의 각 섹션을 설명하고 AWS RI 사용 권장 사항을 식별합니다.

## Summary <a href="#summary" id="summary"></a>

이 섹션은 AWS 계정의 RI에 대한 높은 수준의 요약 보고서를 제공합니다.\
구매한 RI를 EC2 사용량과 일치시키는 데 도움이 되므로 미사용 RI와 권장 RI를 더 잘 관리할 수 있습니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1543870608781/ri-summary.png" alt=""><figcaption><p>Summary 예시</p></figcaption></figure>

* Total Instance Count for Active Reservations - 모든 활성 예약 인스턴스의 총 인스턴스 수
* Total Active Reservations - 구매하여 사용할 수 있는 예약 인스턴스 수
* Total Retired Reservations - 만료되어 사용할 수 없는 예약 인스턴스 수
* Total Instances Running as Reserved - 구매했지만 실행 중인 EC2 인스턴스에서 사용하지 않는 예약 인스턴스의 수
* Total Instance Count for Unused Reservations - 구매했지만 사용하지 않는 예약 인스턴스의수
* Total On-Demand Instances Not Using Reserved Instance - 온디맨드로 시작되고 예약 인스턴스를사용하지 않는 인스턴스 수

## Reserved Instance Volume Discounts <a href="#reserved_instance_volume_discounts" id="reserved_instance_volume_discounts"></a>

AWS에서 제공하는 예약 인스턴스 볼륨 할인 중 하나에 얼마나 근접했는지 보여줍니다. \
볼륨 할인은 리전당 $250,000의 선불 요금이 발생할 때 트리거됩니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1543870636259/ri-volume-discounts.png" alt=""><figcaption><p>Reserved Instance Volume Discounts 예시</p></figcaption></figure>

* Total Upfront Fees (총 선결제 요금) - 선결제 예약 인스턴스 요금에 지출한 총액
* Region (지역) - 수수료가 발생한 지역
* Upfront Discount (선불 할인) - 달성한 선불 요금의 할인 비율
* Hourly Discount (시간당 할인) - 달성한 시간당 요금의 할인 비율

## Instances by Region <a href="#instances_by_region" id="instances_by_region"></a>

각 리전 내에서 구매한 예약 인스턴스 수를 보여줍니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1543871063215/ri-regio.png" alt=""><figcaption><p>Instances by Region 예시</p></figcaption></figure>

* Region - 예약 인스턴스를 구매한 지리적 위치
* Instances - 해당 지역 내에서 구매한 총 예약 인스턴스

## Instances by Size <a href="#instances_by_size" id="instances_by_size"></a>

크기별로 분류된 인스턴스를 표시합니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1543871893111/ri-size.png" alt=""><figcaption><p>Instances by Size 예시</p></figcaption></figure>

* Size - 인스턴스의 크기입니다. **예시)** t2.micro, m1.small
* Instances - 해당 크기의 총 인스턴스 수

## Instances by Utilization <a href="#instances_by_utilization" id="instances_by_utilization"></a>

선결제 유형별로 분류된 인스턴스를 보여줍니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1543871935356/ri-utilizatio.png" alt=""><figcaption><p>Instances by Utilization 예시</p></figcaption></figure>

* Utilization Type - 선결제 유형
* Instances - 해당 예약 유형의 총 인스턴스 수

{% hint style="info" %}
AWS는 더 이상 Medium 또는 Light 활용 유형을 제공하지 않습니다.\
그러나 **CloudCheckr**는 사용률 차트에 이러한 유형을 계속 표시할 수 있습니다.
{% endhint %}

## Instances by Offering Class <a href="#instances_by_offering_class" id="instances_by_offering_class"></a>

제공 클래스별로 세분화된 인스턴스를 보여줍니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1544039374933/ri-offering-class.png" alt=""><figcaption><p>Instances by Offering Class 예시</p></figcaption></figure>

* Offering Class - 컨버터블 or 스탠다드
* Instances - 해당 오퍼링 클래스의 총 인스턴스 수

## Instances by Scope <a href="#instances_by_scope" id="instances_by_scope"></a>

범위별로 총 예약 인스턴스의 분석을 표시합니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1544039767766/ri-scope.png" alt=""><figcaption><p>Instances by Scope 예시</p></figcaption></figure>

* Region - 지역으로 식별된 총 인스턴스 수
* Availability Zone - 가용 영역으로 식별되는 총 인스턴스 수

## Instances by Account <a href="#instances_by_account" id="instances_by_account"></a>

계정별 총 예약 인스턴스의 분석을 표시합니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/i7tnjkquyg/1544040154125/ri-account.png" alt=""><figcaption><p>Instances by Account 예시</p></figcaption></figure>

* Account - 예약 인스턴스가 연결된 계정
* Instances - 해당 계정에 속한 총 인스턴스 수
