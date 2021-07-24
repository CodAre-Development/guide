---
description: Apiden yapay zekaya soru sormanızı sağlar
---

# Yapay Zekaya Sor Apisi

{% api-method method="get" host="https://api.codare.fun" path="/sorv2/idiniz?soru=merhaba" %}
{% api-method-summary %}
Soru sorma v2
{% endapi-method-summary %}

{% api-method-description %}
Sorduğunuz soruya cevap verir fakat idinize/kullanıcı adınıza göre cevapları idnize/kullanıcı adınıza kaydeder.  
örn:Belirli bir ad belirlerseniz o ide adınızı sorarsanız o ideki/kullanıcı adınızdaki adı söyler
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="soru" type="string" required=false %}
Sorduğunuz soru
{% endapi-method-parameter %}

{% api-method-parameter name="cevap" type="string" required=false %}
Sorduğunuz sorunun cevabını verir
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{"soru":"sahibin kim","cevap":"Furtsy tarafından yaratıldım."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.codare.fun/" path="sor/sorunuz" %}
{% api-method-summary %}
Soru sorma
{% endapi-method-summary %}

{% api-method-description %}
Sorduğunuz soruyu cevaplar
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="soru" type="string" required=false %}
Sorduğunuz soru
{% endapi-method-parameter %}

{% api-method-parameter name="soru" type="string" required=false %}
Sorduğunuz sorunun cevabını verir
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Başarılı
{% endapi-method-response-example-description %}

```javascript
{"soru":"sahibin kim","cevap":"Furtsy tarafından yaratıldım."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.codare.fun/" path="sor/sorunuz" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="soru" type="string" required=false %}
Sorduğunuz soru
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



