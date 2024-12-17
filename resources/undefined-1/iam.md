---
description: IAM Summary Report
---

# IAM 요약 보고서

IAM 요약 보고서에는 IAM 내에서 생성된 사용자, 그룹 및 액세스 정책이 표시됩니다.\
\
**계정 합계**

* MFA Enabled on Root Account: AWS 계정의 기본 로그인에 대해 Multi-Factor Authentication(MFA)을 활성화할지 여부입니다.
* Users with MFA: AWS 콘솔에 액세스하기 위해 Multi-Factor Authentication(MFA)을 사용\
  하는 IAM 사용자 수입니다.
* Active Access Keys: 사용자가 API를 호출하거나 명령줄 인터페이스로 작업할 수 있는 총 액세스 키 수입니다.
* Users: AWS 계정에 액세스할 수 있는 총 사용자 수입니다.
* Groups: IAM 내의 총 그룹 수입니다.

**암호 정책:** 모든 IAM 사용자의 암호가 준수해야 하는 규칙입니다.

* Allow Users to Change Password: 비활성화된 경우 IAM 관리자만 사용자의 암호를 변경할 수 있습니다. 활성화하면 모든 사용자가 자신의 암호를 개별적으로 관리할 수 있습니다.
* Minimum Password Length: 암호에 포함해야 하는 최소 문자 수를 설정합니다.
* Require Lowercase Characters: 암호에 소문자를 포함해야 하는지 여부.
* Require Uppercase Characters: 암호에 대문자를 포함해야 하는지 여부.
* Require Numbers: 비밀번호에 숫자가 하나 이상 포함되어야 하는지 여부.
* Require Symbols: 암호에 영문과 숫자가 아닌 특수문자가 하나 이상 포함되어야 하는지 여부.

**Account Alias:** 별칭을 생성하여 회사 이름(또는 기타 친숙한 식별자)을 포함하도록 AWS 로그인용 URL을 구성할 수 있습니다.

{% hint style="info" %}
모든 AWS 계정에는 AWS 계정 ID를 사용하여 기본적으로 생성된 별칭이 있습니다.
{% endhint %}

* 별칭 이름: 생성된 사용자 지정 별칭
* 로그인 URL: AWS 콘솔 로그인 페이지의 URL
