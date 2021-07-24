# Embed Mesaj Örneği



```text
const Discord = require('discord.js');

const embed = new Discord.RichEmbed()
	.setColor('#0099ff')
	.setTitle('Başlık kısmı')
	.setURL('https://www.codare.fun')
	.setAuthor('İsim', 'https://i.imgur.com/wSTFkRM.png', 'https://www.codare.fun')
	.setDescription('Buraya açıklama')
	.setThumbnail('https://i.imgur.com/wSTFkRM.png')
	.addField('Alan Başlığı', 'Burda değer var')
	.addBlankField()
	.addField('Satır içi alan başlığı', 'Burada bir değer var', true)
	.addField('Satır içi alan başlığı', 'Burada bir değer var', true)
	.addField('Satır içi alan başlığı', 'Burada bir değer var', true)
	.setImage('https://i.imgur.com/wSTFkRM.png')
	.setTimestamp() //zaman
	.setFooter('burada footer', 'https://i.imgur.com/wSTFkRM.png');

message.channel.send(embed);
```

