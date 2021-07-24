# Komut Engellemeleri

Kanal Engeli

```javascript
if (message.channel.id !== "ID") return message.channel.send('Bu Komut Bu Kanalda Kullanılamıyor.')
```

Rol Engelli

```javascript
if (!message.member.roles.has('ID')) return message.channel.send('Bu Komutu Kullanamazsın')
```

Rol Engel 2

```javascript
if(!message.member.roles.some(r=>["Destek Ekibi", "Kurucu",].includes(r.name))) 
    return message.reply(
      "**Bu Komutu Kullanmak İçin Destek Yetkilerine Sahip Olmalısın**"
    );
```

Sunucu Sahibi

```javascript
if(message.author.id !== message.guild.owner.user.id) return message.reply('Bu komut sunucu sahibine özeldir!')
```

