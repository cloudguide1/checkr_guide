---
description: Custom Reports
---

# 맞춤형 보고서

**Custom Report Builder**를 사용하여 사용자 맞춤형 보고서를 만들 수 있습니다.\
아래 절차에서는 맞춤형 보고서를 만드는 방법의 예를 안내합니다.

## 절차 <a href="#procedure" id="procedure"></a>

1. 왼쪽 탐색 창에서 **Resources > Custom Reports > Custom Report Builder**를 선택합니다. **Custom Report Builder** 페이지가 열립니다.&#x20;

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/g3octmrm07/1543850721090/custom-report-builder-page.png" alt=""><figcaption><p>Custom Report Builder 화면</p></figcaption></figure>

2. **Report type** 드롭다운 메뉴에서 보고서 유형을 선택합니다. **CloudCheckr**는 이 선택을 기반으로 필터, 열 및 정렬 기준 옵션을 채웁니다. 이 절차에서는 **RDS**를 선택했습니다 .
3. **Report Name** 텍스트 필드에 보고서 이름을 입력합니다. \
   **CloudCheckr**가 보고서를 저장하려면 먼저 이름을 제공해야 합니다.
4. **Filters:** ![](https://files.helpdocs.io/p1pa4evz6u/articles/g3octmrm07/1543851078289/add-new-filter-ico.png) (**Add new filter**)를 클릭합니다.
   * 첫 번째 드롭다운 메뉴에서 보고서를 필터링할 데이터 유형을 선택합니다.
   * 두 번째 드롭다운 메뉴에서 검색 범위를 좁힐 기능을 선택합니다.

| **기능**               | **설명**                                                   | **예시**                                                                                                  |
| -------------------- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| is equal to          | 정확히 일치하는 항목 찾기                                           | **Instance Status is equal to Running**: 실행 중인 모든 EC2 인스턴스를 찾습니다.                                       |
| is not equal to      | <p>정확히 일치하는 항목을<br><strong>제외한</strong> 모든 항목을 찾습니다.</p> | **Region is not equal to EU (Ireland)**: 해당 지역에 없는 모든 리소스를 찾습니다.                                        |
| contains             | 선택 항목을 포함하고 부분 일치를 포함할 수 있는 리소스를 찾습니다.                   | <p><strong>Tag contains Product</strong>: <br>Key = <strong>Product</strong>로 태그가 지정된 모든 리소스를 찾습니다.</p> |
| does not contain     | 선택 항목을 포함 **하지 않고** 부분 일치를 포함할 수 있는 리소스를 찾습니다.           | **Availability Zone does not contain 1c**: 다른 가용 영역의 모든 리소스를 찾습니다.                                      |
| starts with          | 빈 텍스트 필드에 입력한 단어 또는 숫자로 시작하는 리소스 이름을 찾습니다.               | **DB Instance Class starts with db.m5**: db.m5로 시작하는 모든 리소스를 찾습니다.                                      |
| does not starts with | 빈 텍스트 필드에 입력한 키워드로 시작 **하지 않는** 리소스를 선택합니다.              | **DB Instance Class does not start with db.m5**: db.m5로 시작하지 않는 모든 리소스를 찾습니다.                           |
| is empty             | 선택한 필터에 대한 값이 **없는** 리소스를 찾습니다.                          | **Engine is empty set to true**: **engine**에 대한 값이 없는 모든 리소스를 찾습니다.                                     |
| is not empty         | 선택한 필터에 대한 값이 **있는** 리소스를 찾습니다.                          | **Engine is not empty set to true**: **engine**에 대한 값이 있는 모든 리소스를 찾습니다.                                 |

* 빈 텍스트 필드에 함수가 조치를 취할 단어 또는 숫자를 입력하십시오.

{% hint style="info" %}
주의사항:

* 대부분의 필터 유형은 입력할 때 제안 사항을 제공합니다.
* **equal to**를 선택하면 보고서는 텍스트 필드에 입력한 내용과 정확히 일치하는 결과를 반환합니다.
* **contains**를 선택하면 원하는 만큼 문자를 입력할 수 있습니다.
* 필터가 **is less than** 와 **is greater than**면 숫자가 필요합니다.
{% endhint %}

5. **Apply**를 클릭합니다 .
6. 해당하는 경우 **Match All Filters** 체크박스를 선택합니다.

<details>

<summary>더 읽어보기</summary>

기본적으로 활성화된 **Match All Filters**는 선택한 모든 필터 옵션과 일치하는 결과만 반환합니다. 선택하지 않으면 선택한 필터 옵션과 함께 보고서에 결과가 포함됩니다. 예를 들어 회사에서 두 가지 필터 옵션으로 구성된 Windows EC2 인스턴스를 실행하고 있습니다.

* 인스턴스 상태가 중지됨과 같음
* 인스턴스 플랫폼은 Windows와 동일합니다.

**Match All Filters**를 선택한 경우 인스턴스 상태가 중지됨 필터와 일치하지 않기 때문에 **CloudCheckr**는 이 EC2 인스턴스를 반환하지 않습니다.

**Match All Filters**를 선택하지 않은 경우 인스턴스 플랫폼이 Windows 필터와 동일 옵션이므로 **CloudCheckr**는 이 EC2 인스턴스를 반환합니다.

</details>

7. **Columns:** [![](https://files.helpdocs.io/p1pa4evz6u/articles/g3octmrm07/1543851078289/add-new-filter-ico.png)](https://files.helpdocs.io/p1pa4evz6u/articles/g3octmrm07/1543851078289/add-new-filter-ico.png)(**Add New Column**)을 클릭합니다.\
   대화 상자가 열립니다.
8. 표시할 열을 선택하고 **Apply**를 클릭합니다.

{% hint style="info" %}
모든 열의 데이터는 사용자 맞춤형 보고서 세부 정보에서도 사용할 수 있습니다. \
예를 들어 보고서 열로 **Platform**을 선택하지 않은 경우 에도 보고서 세부 정보를 확인하여 \
리소스의 플랫폼을 찾을 수 있습니다.
{% endhint %}

9. **Result to Show** 텍스트 상자에 **CloudCheckr**에서 생성할 결과 수를 나타내는 숫자 값을 입력합니다.

{% hint style="info" %}
**Result to Show**를 비워 두면 보고서는 일치하는 모든 결과를 반환합니다.
{% endhint %}

10. &#x20;**Sort by:** 에서 정렬 옵션을 선택합니다.
    1. 첫 번째 드롭다운 메뉴에서 정렬할 열을 선택합니다.
    2. 두 번째 드롭다운 메뉴에서 결과를 **Ascending**(오름차순) 또는 **Descending**(내림차순)으로 정렬할지 여부를 선택합니다.
11. &#x20;**Build Summary Chart For** 드롭다운 메뉴에서 보고서 차트를 작성할 매개변수를 선택합니다.
12. &#x20;**Save Filter**를 클릭합니다.\
    **CloudCheckr**는 보고서를 성공적으로 저장한 후 페이지 상단에 알림을 표시합니다.
13. 맞춤형 보고서에 액세스하려면: (RDS 기준)

    * 왼쪽 탐색 창에서 **Resources** **> RDS > List of DB instances**를 클릭합니다.

    ![](<../../.gitbook/assets/image (68).png>)

    **CloudCheckr**는 선택한 맞춤형 보고서를 표시합니다.&#x20;

<figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption><p>RDS DB 인스턴스 보고서 화면 예시</p></figcaption></figure>

보고서가 로드되면 보고서를 CSV로 저장하거나, 보고서를 PDF로 다운로드하거나, 보고서를 이메일로 보내거나, 필터를 수정하거나, 필터를 삭제할 수 있습니다.

## 사용 사례

이 예시 사용 사례는 필터 옵션을 사용하여 사용자 지정 대상 결과를 얻는 방법을 보여줍니다.

<table data-header-hidden><thead><tr><th width="141.33333333333331"></th><th></th><th></th></tr></thead><tbody><tr><td><strong>예시</strong></td><td><strong>설명</strong></td><td><strong>Filters</strong></td></tr><tr><td>1</td><td>지난 90일 동안 평균 CPU 사용률이 50% 미만인 미국 서부(오레곤)에서 월 $100 이상의 비용이 드는 모든 실행 중인 Windows 인스턴스를 식별하려면 보고서가 필요합니다.</td><td><ul><li>Status is Equal To Running</li><li>Platform is Equal To Windows</li><li>Instance Cost is Greater Than 100</li><li>Region is Equal To US West (Oregon)</li><li>90 Day Avg CPU is Less Than 50</li></ul></td></tr><tr><td>2</td><td>100만 개 이상의 객체가 있고 미국 외부에 있는 모든 S3 버킷을 표시하는 보고서가 필요합니다.</td><td><ul><li>Objects is Greater Than 1,000,000</li><li>Region Does Not Contain US</li></ul></td></tr><tr><td>3</td><td>us-east-1b 가용 영역에서 실행 중인 비 Linux m1.xlarge 예약 인스턴스를 표시하려면 보고서가 필요합니다.</td><td><ul><li>Pricing Type is Equal To Reserved</li><li>Platform is not Equal to Linux</li><li>Platform is not Equal to Linux</li><li>Type (Size) is Equal to m1.xlarge</li><li>Availability Zone is Equal to us-east-1b</li></ul></td></tr><tr><td>4</td><td>CPU가 50% 이상 급증하지 않은 $200 미만인 특정 VPC 내의 모든 인스턴스를 표시하려면 보고서가 필요합니다.</td><td><ul><li>VPC is Equal To [enter the name of your VPC]</li><li>Cost is Less Than 200</li><li>Peak Utilization is Less Than 50</li></ul></td></tr></tbody></table>
