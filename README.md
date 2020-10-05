---
description: 회원 로그인
---

# signin

{% api-method method="post" host="http://localhost:5000" path="/signin" %}
{% api-method-summary %}
signin
{% endapi-method-summary %}

{% api-method-description %}
서버에 email과 password를 보내고 로그인을 요청합니다.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="email" type="string" required=true %}
가입한 email을 담아옵니다.
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}
가입한 password를 담아옵니다. 
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=302 %}
{% api-method-response-example-description %}
login successfully 
{% endapi-method-response-example-description %}

```
{    "message": "로그인에 성공했습니다."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



