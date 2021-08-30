---
description: İstediğiniz sitenin rssini okumayı sağlar
---

# Rss okuma

{% api-method method="get" host="https://api.codare.fun" path="/rss-oku?link=https://bitcoingazete.com/" %}
{% api-method-summary %}
Rss oku
{% endapi-method-summary %}

{% api-method-description %}
Kolay şekilde rss okumanızı sağlar
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="link" type="string" %}
Rssini okumak istediğiniz sitenin linki
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Başarılı şekilde rss okuduğunda
{% endapi-method-response-example-description %}

```javascript
[
  {
    "başlık": "Elon Musk DOGE ‘ye Destek  Tweeti",
    "link": "https://bitcoingazete.com/elon-musk-doge-ye-destek-tweeti/?utm_source=rss&utm_medium=rss&utm_campaign=elon-musk-doge-ye-destek-tweeti",
    "content": "Tesla ve SpaceX’in lideri, Dogecoin hayranı ve varlığın en etkili destekçisi Elon Musk, yeni Doge yükseltmesini mümkün olduğunca çok bilgisayara...\nThe post Elon Musk DOGE ‘ye Destek  Tweeti appeared first on bitcoingazete."
  },
  {
    "başlık": "Analist Poppe : ADA Tüm Zamanların En Yüksek Seviyesine Yakın Konsolide Olurken Cardano için Önemli Destek Seviyeleri",
    "link": "https://bitcoingazete.com/analist-poppe-ada-tum-zamanlarin-en-yuksek-seviyesine-yakin-konsolide-olurken-cardano-icin-onemli-destek-seviyeleri/?utm_source=rss&utm_medium=rss&utm_campaign=analist-poppe-ada-tum-zamanlarin-en-yuksek-seviyesine-yakin-konsolide-olurken-cardano-icin-onemli-destek-seviyeleri",
    "content": "Kripto stratejisti Michaël van de Poppe, hem ABD doları hem de Bitcoin (BTC) karşısında Cardano için kritik destek alanlarını çiziyor....\nThe post Analist Poppe : ADA Tüm Zamanların En Yüksek Seviyesine Yakın Konsolide Olurken Cardano için Önemli Destek Seviyeleri appeared first on bitcoingazete."
  },
  ...
]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Rss okunulamaz ise veya hata oluştuğunda
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



