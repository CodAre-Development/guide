# Seviye Sistemi Level Puanı Arttırma

Maininizedeki \(server.js/main.js/index.js/bot.js\) seviye kodları olan yere

```javascript
if (db.has(`xp1234_${msg.author.id + msg.guild.id}`) === false) {
  var biyo = (250)
  } 
  if (db.has(`xp1234_${msg.author.id + msg.guild.id}`) == true){
    var biyo = db.fetch(`xp1234_${msg.author.id + msg.guild.id}`)
  }
```

bunu ekleyin  


![](../../.gitbook/assets/image%20%288%29.png)

seviye atlandığı yerdeki kodları bunun gibi yapın

```text
db.add(`xp1234_${msg.author.id + msg.guild.id}`, 250)
```

 burada her seviye atlanınca kaç puan artacağını yazın ben 250 olarak belirledim siz değiştireilirsiniz ve komutlara geçelim exports.run un hemen altına

```text
  if (db.has(`xp1234_${msg.author.id + msg.guild.id}`) === false) {
  var biyo = (250)
  } 
  if (db.has(`xp1234_${msg.author.id + msg.guild.id}`) == true){
    var biyo = db.fetch(`xp1234_${msg.author.id + msg.guild.id}`)
  }
```

 bunu ekliyoruz  
buradaki kısmı bunun gibi yapıyoruz

![](../../.gitbook/assets/image%20%2817%29.png)

