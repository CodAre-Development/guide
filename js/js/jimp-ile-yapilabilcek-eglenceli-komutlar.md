# Jimp ile Yapılabilcek Eğlenceli Komutlar

Burada Jimp Modülü ile yapılabilecek eğlenceli komutlar vardır  
`pnpm i jimp` ile indirebilirsiniz  
`const Jimp = require('jimp');` ile tanımlayın  
  
Resmi Siyah Beyaz Yapar:

```javascript
const Discord = require('discord.js');
const Jimp = require('jimp');

exports.run = (client, message, params) => {

  if(params[0]) if(params[0] === 'sunucu-ikon'){
    if(!message.guild) return message.channel.send('Bu sadece sunucularda kullanılabilir.');
    if(!message.guild.iconURL) return message.channel.send('Bu sunucunun ikonu yok.');

    Jimp.read(message.guild.iconURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
        image.greyscale().write('image.png');
        setTimeout(() => {
          message.channel.sendFile('image.png');
        }, 500);
    });
    return;
  }
  if(message.mentions.users.first()) {
      Jimp.read(message.mentions.users.first().avatarURL, function (err, image){
          if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
          image.greyscale().write('image.png');
          setTimeout(() => {
            message.channel.sendFile('image.png');
          }, 500);
      });
  } else{
    Jimp.read(message.author.avatarURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen Yapımcıya Bildirin.');
        image.greyscale().write('image.png');
        message.channel.sendFile('image.png');
    });
  }
};

exports.conf = {
  enabled: true,
  guildOnly: false,
  aliases: [],
  permLevel: 0
};

exports.help = {
  name: 'invertt',
  description: 'Avatarın renklerini ters çevirir.',
  usage: 'invert [@<kişi ismi>]'
};
```

Resmi fade yapar \(solgunlaştırır\):

```javascript
const Discord = require('discord.js');
const Jimp = require('jimp');

exports.run = (client, message, params) => {

  if(params[0]) if(params[0] === 'sunucu-ikon'){
    if(!message.guild) return message.channel.send('Bu sadece sunucularda kullanılabilir.');
    if(!message.guild.iconURL) return message.channel.send('Bu sunucunun ikonu yok.');

    Jimp.read(message.guild.iconURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
        image.fade(0.5).write('image.png');
        setTimeout(() => {
          message.channel.sendFile('image.png');
        }, 500);
    });
    return;
  }
  if(message.mentions.users.first()) {
      Jimp.read(message.mentions.users.first().avatarURL, function (err, image){
          if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
          image.fade(0.5).write('image.png');
          setTimeout(() => {
            message.channel.sendFile('image.png');
          }, 500);
      });
  } else{
    Jimp.read(message.author.avatarURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen Yapımcıya Bildirin.');
        image.fade(0.5).write('image.png');
        message.channel.sendFile('image.png');
    });
  }
};

exports.conf = {
  enabled: true,
  guildOnly: false,
  aliases: [],
  permLevel: 0
};

exports.help = {
  name: 'fade',
  description: 'Avatarın renklerini ters çevirir.',
  usage: 'invert [@<kişi ismi>]'
};
```

Resme blur efekti verir:

```javascript
const Discord = require('discord.js');
const Jimp = require('jimp');

exports.run = (client, message, params) => {

  if(params[0]) if(params[0] === 'sunucu-ikon'){
    if(!message.guild) return message.channel.send('Bu sadece sunucularda kullanılabilir.');
    if(!message.guild.iconURL) return message.channel.send('Bu sunucunun ikonu yok.');

    Jimp.read(message.guild.iconURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
        image.gaussian(1).write('image.png');
        setTimeout(() => {
          message.channel.sendFile('image.png');
        }, 500);
    });
    return;
  }
  if(message.mentions.users.first()) {
      Jimp.read(message.mentions.users.first().avatarURL, function (err, image){
          if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
          image.gaussian(1).write('image.png');
          setTimeout(() => {
            message.channel.sendFile('image.png');
          }, 500);
      });
  } else{
    Jimp.read(message.author.avatarURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen Yapımcıya Bildirin.');
        image.gaussian(1).write('image.png');
        message.channel.sendFile('image.png');
    });
  }
};

exports.conf = {
  enabled: true,
  guildOnly: false,
  aliases: [],
  permLevel: 0
};

exports.help = {
  name: 'blur',
  description: 'Avatarın renklerini ters çevirir.',
  usage: 'invert [@<kişi ismi>]'
};
```

Resmin contrastını değiştirir

```javascript
const Discord = require('discord.js');
const Jimp = require('jimp');

exports.run = (client, message, params) => {

  if(params[0]) if(params[0] === 'sunucu-ikon'){
    if(!message.guild) return message.channel.send('Bu sadece sunucularda kullanılabilir.');
    if(!message.guild.iconURL) return message.channel.send('Bu sunucunun ikonu yok.');

    Jimp.read(message.guild.iconURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
        image.contrast(1).write('image.png');
        setTimeout(() => {
          message.channel.sendFile('image.png');
        }, 500);
    });
    return;
  }
  if(message.mentions.users.first()) {
      Jimp.read(message.mentions.users.first().avatarURL, function (err, image){
          if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
          image.contrast(1).write('image.png');
          setTimeout(() => {
            message.channel.sendFile('image.png');
          }, 500);
      });
  } else{
    Jimp.read(message.author.avatarURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen Yapımcıya Bildirin.');
        image.contrast(1).write('image.png');
        message.channel.sendFile('image.png');
    });
  }
};

exports.conf = {
  enabled: true,
  guildOnly: false,
  aliases: [],
  permLevel: 0
};

exports.help = {
  name: 'contrast',
  description: 'Avatarın renklerini ters çevirir.',
  usage: 'invert [@<kişi ismi>]'
};
```

Resmi o boyurlarda kırpar crop\(50, 50, 50, 50\) kısmındaki sayıları yükseltin kırpma ayarı için ama 50den aşasını tavsiye etmem

```javascript
const Discord = require('discord.js');
const Jimp = require('jimp');

exports.run = (client, message, params) => {

  if(params[0]) if(params[0] === 'sunucu-ikon'){
    if(!message.guild) return message.channel.send('Bu sadece sunucularda kullanılabilir.');
    if(!message.guild.iconURL) return message.channel.send('Bu sunucunun ikonu yok.');

    Jimp.read(message.guild.iconURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
        image.crop(50, 50, 50, 50).write('image.png');
        setTimeout(() => {
          message.channel.sendFile('image.png');
        }, 500);
    });
    return;
  }
  if(message.mentions.users.first()) {
      Jimp.read(message.mentions.users.first().avatarURL, function (err, image){
          if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen yapımcıya bildirin.');
          image.crop(50, 50, 50, 50).write('image.png');
          setTimeout(() => {
            message.channel.sendFile('image.png');
          }, 500);
      });
  } else{
    Jimp.read(message.author.avatarURL, function (err, image){
        if(err) return message.channel.send('Bir hata oluştu: ``'+err+'``\n Lütfen Yapımcıya Bildirin.');
        image.crop(50, 50, 50, 50).write('image.png');
        message.channel.sendFile('image.png');
    });
  }
};

exports.conf = {
  enabled: true,
  guildOnly: false,
  aliases: [],
  permLevel: 0
};

exports.help = {
  name: 'kırp',
  description: 'Avatarın renklerini ters çevirir.',
  usage: 'invert [@<kişi ismi>]'
};
```

