---
description: İstediğiniz sitenin rssini bulmayı sağlar
---

# Rss Bulma

{% api-method method="get" host="https://api.codare.fun" path="/rss-bul?link=https://bitcoingazete.com/" %}
{% api-method-summary %}
Rss Bul
{% endapi-method-summary %}

{% api-method-description %}
Kolay şekilde rss bulmanızı sağlar
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="link" type="string" %}
Rssini bulmak istediğiniz sitenin linki
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Başarılı şekilde bulundu
{% endapi-method-response-example-description %}

```javascript
{
  "status": true,
  "başlık": "bitcoingazete - bitcoingazete",
  "favicon": "https://i1.wp.com/bitcoingazete.com/wp-content/uploads/2021/05/cropped-logo2.jpg?fit=192%2C192&ssl=1",
  "url": "https://bitcoingazete.com",
  "feedurl": [
    {
      "title": "bitcoingazete » beslemesi",
      "url": "https://bitcoingazete.com/feed/"
    },
    {
      "title": "bitcoingazete » yorum beslemesi",
      "url": "https://bitcoingazete.com/comments/feed/"
    }
  ]
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Rss bulamayınca veya hata oluştuğunda
{% endapi-method-response-example-description %}

```javascript
{
  "status": false,
  "message": "Hata oluştu"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



