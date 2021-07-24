---
description: Bu api ile belirtiğiniz birimlerin değerini v.b bilgileri çekebilirsiniz.
---

# Kripto,Borsa Api

{% api-method method="get" host="https://api.codare.fun" path="/kripto/usd/try" %}
{% api-method-summary %}
Belirtiğinizi çekmek
{% endapi-method-summary %}

{% api-method-description %}
Apiden belirtiğinizi çekersiniz
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
"fiyat":8.129870129870131,
"medyan":8.127247303236116,
"sonhacim":1748.20372223043,
"son24saathacmi":375461309.61114466,
"günaçılışı":8.0999000999001,
"günyüksek":8.097902097902098,
"gündüşük":8.141858141858144,
"açılış24saate":8.186813186813188,
"yüksek24saate":8.099,
"düşük24saate":8.198602794411178,
"market":"CCCAGG",
"sonmarket":"Kraken",
"saatlikhacim":4730886.686746494,
"saataçılış":8.133866133866134,
"saatyüksek":8.12887112887113,
"saatdüşük":8.135864135864137,
"üstkatmanhacmi24saate":375461309.61114466,
"değişiklik24saate":-0.0569430569430569,
"değişiklikgünde":0.02997002997003051,
"değişikliksaate":-0.003996003996002528,
"çevrilen":"USDT",
"arz":0,
"piyasadeğeri":0,
"piyasadeğericezası":0,
"toplamhacim24saate":0,
"toplamüstkatmanhacmi24saate":0,
"resim":"https://www.cryptocompare.com//media/35309345/no-image.png"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



