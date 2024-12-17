---
description: List of IAM Users Report
---

# IAM 사용자 목록 보고서

IAM 사용자 목록 보고서는 AWS Identity & Access Management(IAM)에서 생성된 각 사용자에 대한 세부 정보를 제공합니다.

이 보고서는 사용자를 사전순으로 나열하고 사용자의 ARN 값, 사용자가 마지막으로 액세스한 시간 및 암호가 마지막으로 변경된 시간을 포함합니다.

보고서에 액세스하려면 왼쪽 탐색 창으로 이동하고 **Resources > IAM > List of Users**를 선택합니다.

<div align="left"><figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/iur13rjlox/1544108899135/list-of-iam-users-report.png" alt=""><figcaption><p>IAM 사용자 목록 보고서 화면</p></figcaption></figure></div>

자세한 내용을 보려면 사용자와 관련된 ![](https://files.helpdocs.io/p1pa4evz6u/articles/iur13rjlox/1544109004042/green-plus-ico.png)를 클릭하십시오.

<div align="left"><figure><img src="https://files.helpdocs.io/p1pa4evz6u/articles/iur13rjlox/1544109065871/iam-user-details-1.png" alt=""><figcaption><p>+ 클릭시 확인 가능한 화면</p></figcaption></figure></div>

테이블은 각 사용자에 대해 사용 가능한 세부 정보를 식별합니다.

<table data-header-hidden><thead><tr><th width="267"></th><th></th></tr></thead><tbody><tr><td><strong>세부 정보</strong></td><td><strong>설명</strong></td></tr><tr><td>Groups</td><td>사용자가 속한 IAM 그룹을 나열합니다.</td></tr><tr><td>Access Keys</td><td>사용자가 프로그래밍 방식으로 AWS를 호출할 수 있도록 하는 사용자의 액세스 키에 대한 세부 정보를 표시합니다. 각 액세스 키의 생성 날짜 및 상태(비활성화 또는 활성)가 포함됩니다.</td></tr><tr><td>MFA Device</td><td>사용자가 로그인을 위해 구성한 MFA(Multi-Factor Authentication) 장치를 보여줍니다. 장치가 활성화되었을 때 장치의 Amazon 리소스 이름(ARN)을 포함하고 장치를 가상<br>또는 하드웨어로 식별합니다.</td></tr><tr><td>Policies</td><td>IAM 사용자에게 연결된 모든 정책을 식별합니다.</td></tr><tr><td>Credentials Report</td><td>사용자 생성 날짜 및 시간, 다음 암호 교체, 액세스 키가 마지막으로 사용된 리전과 같은 IAM 사용자에 대한 세부 정보를 제공합니다.</td></tr></tbody></table>
