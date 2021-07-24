# Mesaj Yazan Üyede Rol Denetleme

* Hey! Siz de "eğer üyede "bla bla" isimli rol varsa komutu kullansın, yoksa kullanamasın" kodunu arayıp bulamayanlardan mısınız?
* Öyle ise, artık buldunuz!
* Tek yapmanız gereken şey, dosyanıza bu kodu eklemek:

  if \(message.member.roles.some\(Rol =&gt; Rol.name === 'Rol İsmi'\)\) {

  }

buda rol id si isteyenler için:

```javascript
if (message.member.roles.some(Rol => Rol.id === 'Rol idsi')) {
}
```

