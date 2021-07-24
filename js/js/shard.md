# Shard

**1.Shard Konusu**  
shard.js diye bir dosya oluşturun, onun içine yapıştırın komutlar değil ve, eğer yukarıda ki çalışmazsa:  
[Link](http://tagacaybin.glitch.me/ubijacuqor.js)  
  
Daha gelişmişini isteyenler:  
[Link](http://tagacaybin.glitch.me/uyefowitay.js)  
  
Ufak bir bilgilendirme, shard.js dosyasını oluşturduktan sonra yapmanız gereken package.json kısmına girip "main" ve "start" kısmında ki main dosyanızın adını shard dosyasının adı olarak değiştirin.  


![](../../.gitbook/assets/image%20%289%29.png)

**2.Shard Konusu  
-**shard.js adında dosya açıp [LİNK](http://tagacaybin.glitch.me/osuhebegap.js) \| bu kodu yazıyoruz.  
**-**bot.js-server.js-index.js her neysem mutlaka içinde client.login\('token'\) kalsın silmeyin.  
**-**package.json'a girip `"main": "shard.js"` ve `"start": "node shard.js"` yapın.

{% hint style="danger" %}
**Glitch proje linki hatalı olduğu için alttan kodu alabilirsiniz.**
{% endhint %}

```javascript
const Discord = require('discord.js');
const ayarlar = require("./ayarlar.json");



const cortexbot = new Discord.ShardingManager('./bot.js', {
    totalShards: "auto", // shard sayısı ya da auto yazılabilir
    token: ayarlar.token // token
});

cortexbot.spawn(); 
// www.cortex.red
cortexbot.on('launch', shard => {
  console.log(`${shard.id} IDli shard başarıyla başlatıldı.`)
});
// www.cortex.red
setTimeout(() => {
    console.log("Cortex: Yeniden başlatılıyor.")
    cortexbot.broadcastEval("process.exit()");
}, 21600000);
```

