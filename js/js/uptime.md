# Uptime

**1-)Glitch için güncel uptime (Glitch admin'i tarafından onaylı)**

```javascript
const express = require('express')
const app = express()

app.get('/', (req, res) => res.send('Bot Aktif!')) // sitenize girdiğinde görebilirsiniz.
app.listen(process.env.PORT, () => console.log('Port ayarlandı: ' + process.env.PORT))
```

**Bilgi:** _Main dosyanıza atmanız gerekmektedir. | Uptime olmuyor ise: npm i express | yazın._\
__**Uyarı:** Paneliniz var ise `=> res.send('Bot Calisiyor!'))` kısmını kaldırmanız ve onun yerine `app.get('/', (req, res)` yazmanız gerekmektedir.

**2-)GLİTCH PROJELERİNİZE 7/24 UPTİME YAPMAK İÇİN SİTE/VDS ARTIK GEREKMİYOR!**\
****[**Link**](https://glitch.com/edit/#!/cortex-uptime-bot)****\
****_Vermiş olduğum proje linkine tıklayıp **Remix** yapın_\[14:28]Botunuzu kullanan her kullanıcı kendi projesine uptime yapma imkanı sağlayacaktır.\
**KOMUTLARI:**\
`+yardım` - Yardım menüsünü gösterir. \
`+ekle` - Belirttiğiniz bağlantıyı sisteme ekler.\
`+say` - Sistemdeki Botları Gösterir.\
**Kurulum:** \
server.js'nin en altındaki client.login('token') değiştirmeniz gerekiyor bu kadar.\
\
**3-)**`Uptime Bot` İstediğiniz kadar link ekleyebildiğiniz, tüm eklediğiniz linkleri görebildiğiniz bir Uptime Bot. Benden izinsiz bir şekilde paylaşılması yasaktır, kullanabilirsiniz. [**Github linki**](https://github.com/thischimp/uptime-bot)****
