---
description: 'Bu api ile belirtiğiniz tarihteki,belirtiğiniz birimin fiyatını gösterir'
---

# Kripto,Borsa Tarihten Fiyatını Çekme Api

{% api-method method="get" host="https://api.codare.fun" path="/kripto/tarih/BTC/USD?tarih=2018-03-29" %}
{% api-method-summary %}
Tarihten fiyatını çekme
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="fiyat" type="string" required=false %}
Tarihteki fiyatı gösterir
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{"fiyat":7106.62}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



