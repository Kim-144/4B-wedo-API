---
description: 회원가입
---

# signUpController

{% api-method method="post" host="http://localhost:5000" path="/signup" %}
{% api-method-summary %}
signup
{% endapi-method-summary %}

{% api-method-description %}
서버에 회원가입 요청을 보냅니다.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="email" type="string" required=true %}
가입정보 입력.
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="nickname" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="fullname" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{   
    "id": 8,
    "password": "45l0K4q0jR2z+PTE+/kMlKDsQPUVmjO9KaqjYFz52ag=",
    "full_name": "gwanghyeok",
    "nickname": "kim",
    "email": "im@gwanghyeok.com",
    "updatedAt": "2020-10-04T15:34:00.937Z",
    "createdAt": "2020-10-04T15:34:00.937Z"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=409 %}
{% api-method-response-example-description %}
db 상에 email 데이 이 존재합니다.
{% endapi-method-response-example-description %}

```
{    "message": "중복된 email 입니다."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



