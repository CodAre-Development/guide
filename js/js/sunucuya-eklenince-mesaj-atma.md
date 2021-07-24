# Sunucuya Eklenince Mesaj Atma

Rastgele Kanala Mesaj

```javascript
client.on('guildCreate', guild => {

    let bigz = guild.channels.filter(c => c.type === "text").random()
    bigz.send("Bu bot BIGGZ#3878 eseridir...");
});
```

Sunucu Sahibine Mesaj

```javascript
client.on("guildCreate", async guild => {
  const biggz = [
    "Bot sunucuna eklendi.Tebrikler dostum.",
    "Bu bot **BIGGZ#3878** tarafından geliştirilmektedir.",
    'iyi günlerde kullan..'
  ];
  guild.owner.send(biggz);
  console.log(`LOG: ${guild.name}. sunucuya katıldım!`);
});
```

Kanala Log Mesajı

```javascript
client.on('guildCreate', async guild => { client.channels.get('ID').send(`${guild}, isimli sunucuya eklendim!`)})

// atıldım
client.on('guildDelete', async guild => { client.channels.get('ID').send(`${guild}, isimli sunucudan atıldım.. :(`)})
 
```

