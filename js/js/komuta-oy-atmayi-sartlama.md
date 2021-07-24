# Komuta Oy Atmayı Şartlama

```javascript
const DBL = require('dblapi.js')
const dbl = new DBL('TOKEN', client) 


dbl.hasVoted(message.author.id).then(voted => {
      if(voted) {



      //komut
 


     } else {
        message.channel.send("Bu komutu kullanabilmek için 12 saatte bir https://discordbots.org/bot/BOTUNID/vote sitesinden bota oy vermeniz gerekmektedir. Onaylanması birkaç dakika sürebilir, lütfen bekleyin.")
      }
  })
```

"TOKEN" yazan yerdeki tokeni şöyle alabilirsiniz, [https://discordbots.org/api/docs\#mybots](https://discordbots.org/api/docs#mybots) sitesine gidip botunuza basın ve "GENERATE TOKEN" seçeneğine tıklayın. Ardından gelen tokeni "TOKEN" yazan yere yapıştırın.  
Örnek Komut:

```javascript
const tools = require('../functions.js');

exports.run = async (client, msg, args) => {
    if(msg.channel.type == "dm")  return;
  if(msg.channel.type !== "text") return;
  //
  		  const DBL = require('dblapi.js')
      const ayarlar = require('../ayarlar.json')
  const dbl = new DBL('TOKEN', client) 
  
  dbl.hasVoted(msg.author.id).then(voted => {
    if(voted) {
  
  //
    let ask=[
      "Aşkölçer %3 Gösteriyor.",
      "Aşkölçer %6 Gösteriyor.",
      "Aşkölçer %9 Gösteriyor.",
      "Aşkölçer %12 Gösteriyor.",
      "Aşkölçer %18 Gösteriyor.",
      "Aşkölçer %20 Gösteriyor.",
      "Aşkölçer %23 Gösteriyor.",
      "Aşkölçer %26 Gösteriyor.",
      "Aşkölçer %29 Gösteriyor.",
      "Aşkölçer %30 Gösteriyor.",
      "Aşkölçer %40 Gösteriyor.",
      "Aşkölçer %50 Gösteriyor.",
      "Aşkölçer %60 Gösteriyor.",
      "Aşkölçer %70 Gösteriyor.",
      "Aşkölçer %73 Gösteriyor.",
      "Aşkölçer %76 Gösteriyor.",
      "Aşkölçer %79 Gösteriyor.",
      "Aşkölçer %82 Gösteriyor.",
      "Aşkölçer %85 Gösteriyor.",
      "Aşkölçer %88 Gösteriyor.",
      "Aşkölçer %90 Gösteriyor.",
      "Aşkölçer %91 Gösteriyor.",
      "Aşkölçer %92 Gösteriyor.",
      "Aşkölçer %93 Gösteriyor.",
      "Aşkölçer %94 Gösteriyor.",
      "Aşkölçer %95 Gösteriyor.",
      "Aşkölçer %96 Gösteriyor.",
      "Aşkölçer %97 Gösteriyor.",
      "Aşkölçer %98 Gösteriyor.",
      "Aşkölçer %99 Gösteriyor.",
      "Aşkölçer %100 Gösteriyor.",
    ]
      let member = msg.mentions.members.first()
     if(!member)return msg.channel.send({embed: {
   color: Math.floor(Math.random() * (0xFFFFFF + 1)),
   description: ('<:no:697374724946395246> Bir Kullanıcıyı Etiketlemen Gerek! `g!aşkölçer @Lenux`')
       
  }});
  
  
  
    else{
    msg.channel.send({embed: {
   color: Math.floor(Math.random() * (0xFFFFFF + 1)),
   description: (`${member} ${ask[Math.floor(Math.random() * 30)]}.`)
    }})
    }
//
  				} else {
        return tools.embed(msg, ` Bu Komutu Sadece 12 Saatte Bir Oyvererek Kullanabilirsiniz Oyvermek İçin [Oyver](https://discordbots.org/bot/663092359835156506/vote) Yazısına Tıklayarak Oyverebilirsiniz. Oy Verdiyseniz 5 Dakka Bekleyiniz`) 
                             }
        })
          //

  }
  
  exports.conf = {
    enabled: true,
    guildOnly: false,
    aliases: [],
    permLevel: 0
   };
  
  exports.help = {
    name: 'aşkölçer',
    description: 'Aşk Ölçmeni sağlar.',
    type: ' Eğlence',
    usage: 'aşkölçer'
   }
  
```

