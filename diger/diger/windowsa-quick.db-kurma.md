# Windowsa quick.db Kurma

Youtube videoları:  
[1.link](https://www.youtube.com/watch?v=RzPtrd91z3Q) \| [2.link](https://www.youtube.com/watch?v=c9OXH97n8TE)  
Modülün Kendi Kurulum Rehberi  
[Link](https://github.com/JoshuaWise/better-sqlite3/blob/master/docs/troubleshooting.md)  
Özet:

* 1. Botumuzun klasörüne giriyoruz, boş bir yere shift + sağ tık yapıp Power Shell'i burada aç yazısına tı
* 1. PowerShell'de "npm -g --add-python-to-path install windows-build-tools node-gyp" komutunu çalıştırıyoruz.
* 1. Command \(CMD\)'i kapatıp tekrar açıyoruz.
* 1. Command'a "npm i quick.db" yazıyoruz.  
  
     - üstteki komudu çalıştırdıktan sonra hala yüklenmiyorsa, veya komudu çalıştırırken hata veriyorsa yine PowerShell'den aşağıdaki komudu çalıştırıyoruz:

     ```text
     npm i --global windows-build-tools --vs2015
     ```

     Bu komudu çalıştırdıktan sonra bitmesini bekliyoruz, bitince quick.db yüklenebiliyor olacaktır.  
  
     - Bunu yazdıktan sonra `npm init -y` Yazın ondan sonra yükleyin. Olmazsa package.json silip tekrardan `npm init -y` Yazıp yüklemeyi deneyin.  
     - quick.db yüklemeye çalışırken, "Failed to locate: CL.exe" tarzı bir hata alırsanız, yapmanız gereken şey şu:  
     1. Adım: Bir cmd açıp `npm config set msvs_version 2017 --global` yazınız.  
     2. Adım: Aynı cmd'ye `npm install bcrypt` yazınız.İşlemler bittikten sonra hata giderilmiş olacaktır.

{% hint style="danger" %}
Powershell'e yazdıktan sonra **yüklemesi uzun sürecektir** bitene kadar powershell i kapatmayın
{% endhint %}

{% hint style="danger" %}
Komudu PowerShell'e yazmaya özen gösterin. CMD'de bazen çalışmayabiliyor
{% endhint %}

