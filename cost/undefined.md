---
description: CloudCheckr Cost Alerts
---

# 비용 알림

**CloudCheckr**의 비용 알림은 지출 변경 사항을 자동으로 알려줍니다. \
경보가 발동되면 이메일을 통해 알림이 전송됩니다.

## 일반 설정 <a href="#general_setup" id="general_setup"></a>

1. 시작하려면 **Cost > Alerts > Alert Manager(Cost)**&#xB85C; 이동합니다 .
2.  **+ New Alert**를 클릭한 다음 알림 유형을 선택합니다.

    * **Amazon Web Services Costs** (AWS 비용)
    * **Amazon Web Services Costs (percent)** - AWS 비용 (퍼센트)
    * **Amazon Web Services Contract Tracking** (AWS 계약 추적)
    * **New Tag Values** (새 태그 값)
    * **Amazon Web Services Network Usage** (AWS 네트워크 사용량)


3. **Alert Name**을 입력합니다.
4. **Notifications**를 클릭합니다. 알림 상자가 확장되고 구성 옵션이 표시됩니다.

## 경고 설정 <a href="#alert_setup" id="alert_setup"></a>

### **Amazon Web Services Costs**

AWS 비용 알림을 사용하여 지정된 기간 내에 비용이 특정 예산을 초과하면 알림을 받습니다.

1. 예산 금액 및 트리거 임계값을 설정합니다.

<div align="left"><figure><img src="https://files.helpdocs.io/articles/5iwvhy09gb/1539706238948/03-budget-amount-trigger-threshold.png" alt=""><figcaption><p>예산의 50%, 75%, 90%로 설정된 모습</p></figcaption></figure></div>

2. 예산 기간을 설정합니다.
3. 필터를 설정합니다.

<div align="left"><figure><img src="https://files.helpdocs.io/articles/5iwvhy09gb/1539706239179/04-filters.png" alt=""><figcaption><p>화면에서는 필터 없음(No Filters) 설정된 모습</p></figcaption></figure></div>

4. 계정을 선택합니다.
5. **Create Alert**를 클릭합니다.

### **Amazon Web Services Costs (percent)**

AWS 비용(퍼센트) 알림을 사용하여 이전 기간과 비교할 때 비용이 지정된 비율만큼 변동할 때 알림을 받으십시오.

1.  알림 섹션까지 아래로 스크롤합니다.

    <figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/0prs0i3b1f/1608315177130/alert-screen-empty.png" alt=""><figcaption><p>아래 사용 사례를 참조하여 알림 설정 가능</p></figcaption></figure>
2.  다음 사용 사례 중 하나를 지침으로 사용하여 경고를 구성합니다.

    특정 사용 사례에 대한 지침을 보려면 텍스트 상자를 클릭하십시오.

<details>

<summary>사용 사례 1: 일일 운영 비용의 달러 금액이 이전 기간보다 큰 경우 알림 보내기</summary>



이 사용 사례에서 이전 30일 청구 기간의 평균 운영 비용은 $2,500였습니다. 최소 2일 동안 비용 급증이 있을 때 일일 운영 비용이 $2,500 이상으로 $100 이상 증가하면 **CloudCheckr**에서 경고를 보내길 원합니다.

이러한 조건과 일치하는 경고를 구성하려면:

1. 첫 번째 확인란을 선택하고 (일일 금액) 텍스트 필드에 **100을 입력합니다.** (<mark style="color:red;">**1**</mark>)
2. \_\_일 동안 비용이 급증하는 경우 텍스트 필드에 **2를** 입력합니다 . (<mark style="color:red;">**2**</mark>)
3. 이전\_\_일의 평균 비용과 비교한 텍스트 필드에 **30을** 입력합니다 . (<mark style="color:red;">**3**</mark>)
4.

    <figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>사용 사례 2: 일일 운영 비용의 백분율 또는 달러 금액이 이전 기간보다 클 때 경고 보내기</summary>



이 사용 사례에서 이전 30일 청구 기간의 평균 운영 비용은 $2,500였습니다. 최소 2일 동안 비용 급증이 있을 때 일일 운영 비용이 $100 증가하거나 $2,500 이상으로 4% 이상 증가하면 **CloudCheckr**에서 알림을 받기를 원합니다.

이러한 조건과 일치하는 경고를 구성하려면:

1. 첫 번째 확인란을 선택하고 (일일 금액) 텍스트 필드에 **100을 입력합니다.** (<mark style="color:red;">**1**</mark>)
2. \_\_일 동안 비용이 급증하는 경우 텍스트 필드에 **2를** 입력합니다 . (<mark style="color:red;">**2**</mark>)
3. 이전\_\_일의 평균 비용과 비교한 텍스트 필드에 **30을** 입력합니다 . (<mark style="color:red;">**3**</mark>)
4.  두 번째 확인란을 선택하고 (퍼센트 평균 텍스트 필드에 **4를 입력합니다. (**<mark style="color:red;">**4**</mark>**)**



    <div align="left"><figure><img src="../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure></div>

</details>

<details>

<summary>사용 사례 3: 운영 비용의 비율이 이전 기간보다 높을 때 경고 보내기</summary>

이 사용 사례에서 이전 30일 청구 기간의 평균 운영 비용은 $2,500였습니다. 최소 2일 동안 비용 급증이 있을 때 일일 운영 비용이 $2,500 이상으로 4% 이상 증가하면 **CloudCheckr**에서 경고를 보내길 원합니다.

이러한 조건과 일치하는 경고를 구성하려면:

1. \_\_일 동안 비용이 급증하는 경우 텍스트 필드에 **2를** 입력합니다 . (<mark style="color:red;">**1**</mark>)
2. 이전\_\_일의 평균 비용과 비교한 텍스트 필드에 **30을** 입력합니다 . (<mark style="color:red;">**2**</mark>)
3. 두 번째 확인란을 선택하고 (퍼센트 평균 텍스트 필드에 **4를 입력합니다. (**<mark style="color:red;">**3**</mark>**)**
4.

    <figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>사용 사례 4: 비용 변경이 특정 달러 금액 이상인 경우에만 경고 보내기</summary>

이 사용 사례에서 이전 30일 청구 기간의 평균 운영 비용은 $2,500였습니다. 최소 2일 동안 비용 급증이 있을 때 일일 운영 비용이 $100 증가하거나 $2,500 이상으로 4% 이상 증가하면 **CloudCheckr**에서 알림을 받기를 원합니다.

그러나 **CloudCheckr**가 비용의 변화가 백분율 평균을 $75 이상 초과하는 경우에만 경고하기를 원합니다. 이렇게 하면 작은 비용 변동에 대해 원치 않는 알림을 받지 않습니다.

이러한 조건과 일치하는 경고를 구성하려면:

1. \_\_일 동안 비용이 급증하는 경우 텍스트 필드에 **2를** 입력합니다 . (<mark style="color:red;">**1**</mark>)
2. 이전\_\_일의 평균 비용과 비교한 텍스트 필드에 **30을** 입력합니다 . (<mark style="color:red;">**2**</mark>)
3. 두 번째 확인란을 선택하고 (퍼센트 평균 텍스트 필드에 **4를 입력합니다. (**<mark style="color:red;">**3**</mark>**)**
4. 최소 비용 변경 $ 텍스트 필드에 **75를** 입력합니다 . (<mark style="color:red;">**4**</mark>)
5.

    <figure><img src="../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>

</details>

3. 비용을 모니터링할 방법을 선택합니다.
   * By Account - 경고는 모든 비용을 전체적으로 살펴봅니다.
   * By Service - 경고는 서비스별로 그룹화된 비용을 확인합니다.
   * By Specific Tag - 경고는 사용자 정의 태그별로 그룹화된 비용을 확인합니다.
4. **Create Alert**를 클릭합니다.

### **Amazon Web Services Contract Tracking**

비용이 특정 임계값을 초과하거나 미만일 때 알림을 받으려면 계약 추적 알림을 사용하십시오. 이는 자금 낭비 또는 계약에 지정된 금액을 지출하지 않은 것에 대한 벌금을 피하기 위해 특정 날짜까지 약정된 예산을 모두 사용했는지 확인하려는 경우에 특히 유용합니다.

1. 청구 기간에 대한 예산을 설정합니다.
2. **Exceed**(초과) 임계값 에 대한 트리거를 설정합니다 .
3. **Under**(임계값 미만) 에 대한 트리거를 설정합니다 .
4. 예산 기간을 설정합니다.
5. 필터를 선택합니다. (선택 사항)
   * No Filters (기본값)
   * Filter using the following options (옵션을 사용하여 필터링)
   * Use a Saved Filter (저장된 필터 사용)
6. 계정을 선택하십시오. (기본값으로 ALL 선택됨)
7. **Create Alert**를 클릭합니다.

### **New Tag Values**

지정된 태그 키에 대한 새 태그 값에 대한 알림을 받으려면 이 경고를 사용하십시오. 이렇게 하면 기존 태그 지정 전략을 따르지 않는 새로 생성된 리소스를 인식하는 데 도움이 됩니다.

1. 태그 키를 입력합니다.
2. **Create Alert**를 클릭합니다.

### **Amazon Web Services Network Usage**

데이터 전송 비용이 지정된 금액을 초과할 때 알림을 받으려면 이 알림을 사용하십시오.

1. **Usage Type** 임계값을 설정합니다.\
   &#xNAN;_&#x4E;etwork In_ 또는 _Network Out_ 중 하나를 선택합니다.\
   <mark style="color:red;">`greater than`</mark>임계값을 바이트 단위로 선택합니다.
2. **Service**를 설정합니다.
3. **Account**를 설정합니다.
4. **Create Alert**를 클릭합니다.

{% hint style="success" %}
**Notifications**에서 이메일을 여러 개 입력하려면 , 를 사용합니다

**예시)** you@domain.com, me@domain.com

빈칸으로 남기면 기본 계정에 이메일이 발송됩니다.
{% endhint %}



## 알림 편집 <a href="#editing_your_alerts" id="editing_your_alerts"></a>

1. **Cost > Alerts > Alert Manager(Cost)**&#xB85C; 이동합니다.
2. 알림을 클릭하여 편집합니다. 알림 구성 창이 열립니다.
3. 슬라이더 ![](https://files.helpdocs.io/articles/5iwvhy09gb/1539706239837/11-on-off.png) 를 통해 알림을 활성화/비활성화할 수 있습니다.
4. 알림을 삭제하려면 ![](https://files.helpdocs.io/articles/5iwvhy09gb/1539706239996/13-x.png)을 클릭하세요.



## 결과 <a href="#results" id="results"></a>

**Cost > Alerts > Results** 에 있는 결과 화면에서 **CloudCheckr** 계정에 저장된 검색 가능한 결과를\
찾을 수 있습니다.
