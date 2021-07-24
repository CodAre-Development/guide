# Çİft Prefix Ayarlama

Message.js'da prefix yerine atılacak

```javascript
let prefixes = ["PREFIX_1", "PREFIX_2"]; 
let prefix = "VARSAYILAN_PREFIX"; 
for (var i = 0; i < prefixes.length; i++) { 
if (message.content.startsWith(prefixes[i])) prefix = prefixes[i]; 
} 
```

