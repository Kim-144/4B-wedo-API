---
description: nickname 수정
---

# signEdit

{% api-method method="post" host="http://localhost:5000" path="/signeditnickname" %}
{% api-method-summary %}
signeditnickname
{% endapi-method-summary %}

{% api-method-description %}
서버에 user.nickname update 요청을 보냅니다.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="nickname" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
 successfully.
{% endapi-method-response-example-description %}

```
{
 1
 }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="http://localhost:5000" path="/signeditpassword" %}
{% api-method-summary %}
signeditpassword
{% endapi-method-summary %}

{% api-method-description %}
서버에 user.password update 요청을 보냅니다.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="newpassword" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{"message": "비밀번호 변경 완료."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

