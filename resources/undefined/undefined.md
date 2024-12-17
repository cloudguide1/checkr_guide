---
description: Inventory Reporting
---

# 인벤토리 보고서

**CloudCheckr**는 다음 유형의 인벤토리 보고서를 제공합니다.

* 인벤토리 요약 보고서
* 맞춤형 보고서
* 태그가 지정된 리소스 보고서
* 태그가 지정되지 않은 리소스 보고서
* 추세 보고서
* 다른 AWS 서비스 보고서

## 인벤토리 요약 보고서

인벤토리 요약 보고서는 배포의 일부인 각 AWS 서비스의 스냅샷을 제공합니다. **Summary** 또는 **Detail**\
링크를 클릭하면 총 수, 서비스가 있는 지역, 예상 비용, 상태 및 기타 통계를 볼 수 있습니다.

![Summary 또는 Detail 클릭 후 확인 가능](https://files.helpdocs.io/p1pa4evz6u/articles/aejjy2lhy1/1543594502816/inventory-summary.png)

## 맞춤형 보고서 <a href="#custom_reports" id="custom_reports"></a>

**CloudCheckr**를 사용하면 저장하고 재사용할 수 있는 AWS 리소스에 대한 사용자 맞춤형 보고서를 작성할 수 있습니다. 저장된 사용자 맞춤형 보고서를 실행할 때마다 최신 리소스 데이터로 채워집니다.

자세한 내용은 [맞춤형 보고서](undefined-1.md) 항목을 검토하십시오.

## Map Overlay <a href="#map_overlay" id="map_overlay"></a>

Map Overlay 보고서는 각 리전의 AWS 서비스에 대한 통계를 제공합니다.

드롭다운 메뉴에서 서비스를 선택하고 지역을 클릭합니다.\
**CloudCheckr**는 지도의 오버레이에 자세한 내용을 표시합니다.

<div align="left"><figure><img src="../../.gitbook/assets/map overlay.png" alt=""><figcaption><p>Map Overlay 화면</p></figcaption></figure></div>

## 태그가 지정된 리소스 보고서 <a href="#tagged_resources" id="tagged_resources"></a>

태그가 지정된 리소스 보고서는 AWS에서 사용 중인 모든 태그를 표시하고 각 태그와 연결된 리소스를 식별합니다.

자세한 내용은 [AWS 태깅](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Using_Tags.html) 항목을 참조하십시오.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/aejjy2lhy1/1543591999906/tagged-inventory.png" alt=""><figcaption><p>+ 클릭시 자세한 내용 확인 가능</p></figcaption></figure>

{% hint style="info" %}
이 보고서는 **Name** 태그를 제외합니다.
{% endhint %}

## 태그가 지정되지 않은 리소스 보고서

태그가 지정되지 않은 리소스 보고서에는 리소스 태그가 **없는** AWS 내의 모든 리소스가 표시됩니다.

Resource Name을 클릭하면 자세한 내용을 볼 수 있습니다.

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/aejjy2lhy1/1543590623420/untagged-inventory.png" alt=""><figcaption><p>Resource Name 아래 있는 이름 클릭</p></figcaption></figure>

## 추세 보고서 <a href="#trending" id="trending"></a>

추세 보고서를 사용하면 배포에서 다음 AWS 서비스에 대한 사용량 변동을 확인할 수 있습니다.

* [EC2](../undefined-2/ec2.md)
* S3
* RDS
* Glacier

<figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/aejjy2lhy1/1543590881843/trending-s-3-example.png" alt=""><figcaption><p>S3 Trending 보고서 예시</p></figcaption></figure>

{% hint style="info" %}
이러한 차트의 데이터는 **CloudCheckr** 사용을 시작할 때 매일 채워지기 시작합니다.
{% endhint %}

## 다른 AWS 서비스 보고서 <a href="#other_inventory_reports" id="other_inventory_reports"></a>

**CloudCheckr**의 확인 가능한 다른 AWS 서비스에 대한 보고서 목록을 보려면 **자세히 보기**를 클릭하십시오.

<details>

<summary>자세히 보기</summary>



* EC2

- S3

* RDS

- Certificate Manager

* CloudFormation

- CloudFront

* CloudHSM

- CloudSearch

* CloudWatch Alarm

- Cognito

* Data Pipeline

- Direcct Connect

* DynamoDB

- Elastic Container Service

* EFS

- ElastiCache

* Elastic Beanstalk

- Elastic MapReduce

* Elasticsearch

- Glacier

* IAM

- IoT

* Kinesis

- KMS

* Lambda

- RedShift

* Route 53

- SES

* SipmleDB

- SNS

* SQS

- Storage Gateway

* Support Cases

- SWF

* Workspaces

</details>
