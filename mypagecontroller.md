---
description: user 정보 확인 합니다.
---

# mypageController

{% api-method method="get" host="http://localhost:5000" path="/mypage" %}
{% api-method-summary %}
mypage
{% endapi-method-summary %}

{% api-method-description %}
서버에 로그인한 유저의 정보를 요청합니다.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{ 
    "id": 1,
    "email": "rrr@rrr.rrr",
    "nickname": "바꾼 닉네임",
    "full_name": "rr",
    "password": "45l0K4q0jR2z+PTE+/kMlKDsQPUVmjO9KaqjYFz52ag=",
    "createdAt": "2020-10-03T13:46:21.000Z",
    "updatedAt": "2020-10-05T02:25:34.000Z"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "세션을 찾지 못했습니다."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



