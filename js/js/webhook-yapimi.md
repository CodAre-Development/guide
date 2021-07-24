# Webhook Yapımı

Örnek:

```javascript
const Discord = require('discord.js');

const hook = new Discord.WebhookClient('webhook id', 'webhook token');

hook.send('Merhaba Dünya!');
```

