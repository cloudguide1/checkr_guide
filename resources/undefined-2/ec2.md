---
description: 'Inventory Trending Reports: EC2 Instances'
---

# EC2 인스턴스 추세 보고서

EC2에 대한 추세 보고서는 AWS 배포에서 실행 중인 EC2 인스턴스에 대한 시간 경과에 따른 비용 및\
사용량 메트릭을 제공합니다. \
이 보고서에 액세스하려면 왼쪽 탐색 창으로 이동하여 **Resources > Trending > EC2**를 선택합니다.

다음 네 가지 보고서 중에서 선택할 수 있습니다.

* 시간별 EC2 기록
* 인스턴스별 기록
* 요금 유형별 내역
* 기타

## 시간별 EC2 기록 <a href="#time" id="time"></a>

시간별 EC2 기록 보고서에는 지정된 기간 동안 인스턴스에 대한 실행 시간과 청구 비용이 표시됩니다.

이 보고서에 액세스하려면 **Resources > Trending > EC2 > History by Time**을 선택하십시오.

![시간별 EC2 기록 보고서 화면](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706292916/ec-instance-history-by-time-1-1024-x-481.png)

필터를 만드려면 ![](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293104/filter-icon-trend-ec-2-instance-reports.png)를 클릭하세요.

Filter 선택창이 열립니다.

<div align="left"><img src="https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293290/filter-drop-down-menu-1-300-x-179.png" alt="Filter 선택창"></div>

드롭다운 화살표를 클릭하고 다음 필터 중 하나를 선택합니다.

* **AMI**: EC2 인스턴스에서 사용하는 고유한 Amazon Machine Image
* **Availability Zone**: EC2 인스턴스의 지리적 위치
* **AWS Account ID**: 12자리 AWS 계정 ID
* **Instance ID**: EC2 인스턴스의 고유 ID
* **Instance Type (Size)**: 인스턴스 유형의 크기 (예: t1.micro)
* **Platform**: EC2 인스턴스가 있는 운영 체제 (예: Linux)
* **Pricing Type**: EC2 인스턴스와 관련된 가격 유형
* **Tag**: EC2 인스턴스에 적용되는 리소스 태그(예: \[Key = XXX] \[Value = YYY])
* **Tenancy**: default(기본) 또는 dedicated(전용)

필터를 선택한 후 두 번째 드롭다운 메뉴에서 **equal** 또는 **contains**를 선택하고 세 번째 텍스트 필드에 \
검색 키워드를 입력한 다음 **Apply**를  클릭하여 선택 항목별로 데이터를 필터링 합니다.

이 예시에서는 키워드 **US**를 사용하여 **region**을 필터로 선택했습니다.

<div align="left"><img src="https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293475/filter-example-300-x-181.png" alt="필터가 선택된 화면 예시"></div>

필터에 대해 다음 작업을 수행할 수 있습니다.

* **Delete Filter**: 보고서에서 저장된 필터를 제거합니다.
* **Email**: 보고서를 받을 사람과 빈도를 포함하여 이메일 보고서를 구성합니다.
* **Filter**: 선택한 매개변수를 기반으로 보고서를 생성합니다.
* **Reset**: 기본 설정으로 되돌립니다.
* **Save Filter**: 향후 보고서에 이 필터를 사용하려면 저장하십시오.
* **Update Filter**: 기존 필터에 대한 변경 사항을 저장합니다.

사용자 지정 날짜 범위를 구성하려는 경우 시작 및 종료 옵션에서 날짜와 시간을 선택할 수 있습니다. 기본적으로 보고서에는 지난 7일이 표시됩니다. 선택한 필터로 데이터를 그룹화할 수도 있습니다. 옵션을 선택하지 않으면 선택한 시간 범위 동안 실행된 모든 EC2 인스턴스에 대한 시간이 보고서에 표시됩니다.\
\
Group By 섹션에서 [![](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293634/green-plus-icon-2-e-1534876962895.png)](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293634/green-plus-icon-2-e-1534876962895.png) 를 클릭하여 여러 필터 옵션을 추가할 수 있습니다.\
Group By 섹션에서 선택 항목을 제거하려면 [![](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293795/minus-icon-2-e-1534876994216.png)](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293795/minus-icon-2-e-1534876994216.png) 를 클릭합니다.\
\
선택한 후 **Filter**를 클릭합니다 . 필터 옵션에 따라 **CloudCheckr**는 다음 세부 정보가 포함된 보고서를\
생성합니다.

* **Total Number of Hours Running** : 선택한 날짜 범위 동안 모든 EC2 인스턴스가 실행된 총 시간
* **Total Number of Instances Running** : 선택한 날짜 범위 동안 실행 중인 총 EC2 인스턴스 수입니다.
* **Total Cost** : EC2 인스턴스를 실행하는 데 드는 총 비용

또한 실행 시간 및 인스턴스 수에 따라 추가 세부 정보가 표시됩니다.

* **Min** : 선택한 날짜 범위 동안 모든 날짜/시간 동안 실행되는 최소 시간/인스턴스 수
* **Max** : 선택한 날짜 범위 동안 임의의 날짜/시간 동안 실행된 최대 시간/인스턴스 수
* **Average** : 선택한 날짜 범위 동안 특정 날짜/시간 동안 실행된 평균 시간/인스턴스 수

보고서를 생성하면 필터 옵션에 따라 두 개의 차트가 표시됩니다. 상단에는 하루 동안 모든 인스턴스가 실행된 시간이 표시됩니다.

{% hint style="info" %}
필터링할 때 days 대신 hours를 표시하도록 선택하면 **CloudCheckr**는 이 차트를 표시하지\
않습니다.
{% endhint %}

두 번째 그래프는 각 일/시간 동안 실행된 총 인스턴스 수를 보여줍니다. 그래프의 아무 지점이나 클릭하면 해당 요일/시간 동안 실행된 모든 EC2 인스턴스의 전체 목록을 제공하는 인스턴스별 EC2 기록 보고서로 리디렉션될 수 있습니다.

[![](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293969/csv-butto.png)](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706293969/csv-butto.png)을 클릭하여 보고서의 데이터를 CSV 파일로 내보낼 수도 있습니다.

다음은 첫 번째 그래프의 예입니다.

![마우스로 데이터 확인 가능](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706294112/graph-1-ec-2-instances-by-time-2-1024-x-308.png)

## 인스턴스 별 기록 <a href="#instance" id="instance"></a>

인스턴스 별 EC2 기록 보고서에는 특정 인스턴스의 총 실행 시간과 총 비용이 표시됩니다. 이 보고서에\
액세스하려면 **Resources** **> Trending > EC2 > History by Instance**를 선택하십시오.

![인스턴스별 기록 보고서 화면](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706294318/ec-instance-history-by-pricing-type-1024-x-499.png)

이 보고서의 필터 및 기능은 [시간별 EC2 인스턴스 내역 보고서](ec2.md#time) 와 동일합니다.

목록에서 인스턴스를 클릭하면 해당 특정 인스턴스로 필터링된 시간별 EC2 인스턴스 기록 보고서로 \
리디렉션 됩니다.

## 요금 유형별 내역 <a href="#pricing" id="pricing"></a>

요금 유형별 내역 보고서는 선택한 기간을 기준으로 EC2 인스턴스의 각 요금 유형(EC2 인스턴스, 온디맨드 EC2 인스턴스, 예약 및 스팟)에 대한 추세를 보여줍니다. \
이 보고서에 액세스하려면 **Resources > Trending > EC2 > History by Pricing Type**을 선택합니다.

<figure><img src="../../.gitbook/assets/image (48).png" alt=""><figcaption><p>요금 유형별 내역 보고서</p></figcaption></figure>

**Trends based on the last...days** 드롭다운 화살표를 클릭하여 일 수를 변경합니다.\
옵션에는 7, 30, 90, 180 또는 365가 포함됩니다.

**Filter**를 클릭하여 선택한 일 수를 기준으로 보고서를 생성합니다.

선택한 날짜의 EC2 인스턴스 수를 보려면 그래프의 한 지점 위로 마우스를 가져갑니다.

<div align="left"><img src="https://files.helpdocs.io/articles/hyaa2w1wbm/1539706294617/ec-2-graph-by-date-focal-point-1024-x-338.png" alt="마우스로 데이터 확인 가능"></div>

## 기타 <a href="#other" id="other"></a>

EC2 기타 보고서에는 선택한 기간을 기준으로 EC2 인스턴스와 연결된 다른 데이터 포인트의 추세가 표시됩니다. 이러한 데이터 포인트에는 EBS 볼륨, EBS 볼륨 스토리지, Elastic Load Balancer, 탄력적 IP, 활성 예약 인스턴스, Amazon 머신 이미지 및 EC2 보안 그룹이 포함됩니다.

이 보고서에 액세스하려면 **Resources > Trending > EC2 > Other**를 선택합니다 .

![기타 보고서 화면](https://files.helpdocs.io/articles/hyaa2w1wbm/1539706294794/ec-instance-by-other-1024-x-519.png)

**Trends based on the last...days** 드롭다운 화살표를 클릭하여 일 수를 변경합니다.\
옵션에는 7, 30, 90, 180 또는 365가 포함됩니다.

**Filter**를 클릭하여 선택한 일 수를 기준으로 보고서를 생성합니다.

그래프의 한 지점 위로 마우스를 가져가면 특정 날짜에 선택한 데이터 지점의 숫자를 볼 수 있습니다.

<div align="left"><img src="https://files.helpdocs.io/articles/hyaa2w1wbm/1539706294950/other-data-point-1024-x-247.png" alt="마우스로 데이터 확인 가능"></div>
