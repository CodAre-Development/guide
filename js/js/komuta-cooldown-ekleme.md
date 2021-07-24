# Komuta cooldown ekleme

```javascript
 if (talkedRecently.has(message.author.id)) {
           return message.channel.send("`5` Saniye de Bir Kullanabilirsin - " + message.author);
    } else {

           // the user can type the command ... your command code goes here :)

        // Adds the user to the set so that they can't talk for a minute
        talkedRecently.add(message.author.id);
        setTimeout(() => {
        message.delete();
          // Removes the user from the set after a minute
          talkedRecently.delete(message.author.id);
        }, 5000);// Şuan 5 Saniyedir Değiştirebilirsiniz.
    }
```

exports.run Altına koyun. `const talkedRecently = new Set();` Üst kısmına bunu ekleyiniz.

Tüm komutlara yapmak yerine aşşağıdakini kullanabilirsiniz:

```javascript
  if(cmd) {
  const db = require('quick.db')
  const annen = await db.fetch(`asd.${message.author.id}`)
  if(annen) return message.channel.send(`Bir komut daha kullanabilmek için 3 saniye beklemelisin.`)
  if(!annen) {
  db.set(`asd.${message.author.id}`, 'as')}
  setTimeout(async () => {
  db.delete(`asd.${message.author.id}`)
  }, 3000)
  }
```

message.js'ye atılıyor bot sahibini etkilemesini istemiyorsanız const annen'in üstüne şunu ekleyin

```javascript
if(message.author.id === 'sizin idniz') return;
```

