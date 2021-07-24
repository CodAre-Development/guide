# Express Basit Api Yapma

Selamlar bugün express modülü ile api yapımını göstereceğim size ilk başta  projemizi açıyoruz ardından main dosyamız artık server.js mi yoksa bot.js mi o size kalmış oraya geliyoruz

```javascript
const express = require('express');
const app = express();
const http = require('http');
app.use(express.static('public'));
app.listen(8000)
app.get('/', (request, response) => {

 response.json({mesajımız: 'Selam Herkese!'})
})
```

bunu main dosyamız neyse ordakileri silip bu kodu ekliyoruz ardından siteye girdiğimizde bu yazı çıkacaktır

![](../../.gitbook/assets/image%20%282%29.png)

ben örnek olarak random yüz apisi örneği vericem\[00:48\]ilk başta modül kullancaz modülümüz random-text-faces bunu ilk başta constluyoruz

```javascript
const randomTextFaces = require('random-text-faces');
```

sonra ise HTTP GET isteğine JSON tipinde yanıt vericez

```javascript
app.get('/', (request, response) => {
 response.json({yüz: randomTextFaces.get()})
})
```

siteye girdiğinizde çalışcaktır Kodun tamamı;

```javascript
const express = require('express');
const app = express();
const http = require('http');
app.use(express.static('public'));
app.listen(8000)
const randomTextFaces = require('random-text-faces');
app.get('/', (request, response) => {
 response.json({yüz: randomTextFaces.get()})
})
```

modüleri eklemeyi unutmayın  
[Glitch Linki](https://glitch.com/~basit-api-sitesi)

