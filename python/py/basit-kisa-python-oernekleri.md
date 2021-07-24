# Basit kısa python örnekleri

Faiz Geliri\(Ana Para ile Birlikte\) Hesaplama

```python
def faizGeliriHesapla(ap,fo):
    faizHesap=ap*fo
    return faizHesap

def faizGelirOrani(anap,faizo):
    faizGelir=anap*faizo-anap
    return faizGelir

anaPara=int(input("Ana Parayı Giriniz:"))
faizOrani=float(input("Faiz Oranını Giriniz:"))
print(faizGeliriHesapla(anaPara,faizOrani))
```

Döngüler, Karşılaştırma Operatörleri ve Mantıksal Operatörler Örneği

```python
serialKey=input("Lütfen Serial KEY Giriniz:")
if serialKey=="AAA":
    print("Oyununuz Orijinal! Tebrikler.")

else:
    print("Oyununuz Orijinal DEĞİL!")

while True:
    cikis=input("Programdan çıkmak için lütfen 'q' tuşuna basınız:")
    if cikis=="q":
        print("Başarıyla çıkış yaptınız.")
        break
```

Basit zar atma uygulaması.

```python
import random

zar1 = random.randrange(1,7)
zar2 = random.randrange(1,7)

print("Zarlar {} ve {} şeklinde gelmiştir.".format(zar1,zar2))
```

