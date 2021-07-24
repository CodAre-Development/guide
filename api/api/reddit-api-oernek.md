# Reddit Api Örnek

{% api-method method="get" host="https://api.codare.fun" path="/reddit/sub=:subreddit/tur=:tür/zaman=:zaman/nsfw=:nsfw" %}
{% api-method-summary %}
Subredditen random post çekme
{% endapi-method-summary %}

{% api-method-description %}
Getletiğiniz de alacağınız çıktılar **aşağıda verilmiştir**.Kullanımı için burdan bakabilirsiniz: LİNK\(tıkla\)
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user" type="string" required=false %}
postu atan kişiyi gösterir
{% endapi-method-parameter %}

{% api-method-parameter name="sub" type="string" required=false %}
posta ait olan subu gösterir
{% endapi-method-parameter %}

{% api-method-parameter name="yorum" type="number" required=false %}
postun yorum sayısını gösterir
{% endapi-method-parameter %}

{% api-method-parameter name="resim" type="string" required=false %}
postun resim linkini gösterir
{% endapi-method-parameter %}

{% api-method-parameter name="oy" type="number" required=false %}
postun upvote sayısını gösterir
{% endapi-method-parameter %}

{% api-method-parameter name="baslık" type="string" %}
postun başlığını göste
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{"baslık":"bu bir başlık","resim":"https://furtsy.wtf/resim/resim-1604693525971.png","oy":42,"yorum":2,"sub":"furtsy","user":"Furtsy"}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

