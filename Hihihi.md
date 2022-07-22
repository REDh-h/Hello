# basit-sifre-olusturucu-python
basit şifre oluşturucu ve kırıcı python kodu

alfabe = "abcçdefgğhıijklmnoöprsştuüvyz"

kelime_gir = str(input("Lütfen bir kelime girin : "))
kelime_gir = kelime_gir.lower()
print("Girdiğiniz kelime : "+kelime_gir)

kontrol = str(len(kelime_gir))

if kontrol != str(12):
    print("Oluşturdurğunuz şifre 12 karakter değildir lütfen tekrardan deneyin")
elif kontrol == str(12):
   sifreli_kelime = str(alfabe[alfabe.index(kelime_gir[0]) +1] + alfabe[alfabe.index(kelime_gir[1]) +1] + alfabe[alfabe.index(kelime_gir[2]) +1] + alfabe[alfabe.index(kelime_gir[3]) +1] + alfabe[alfabe.index(kelime_gir[4]) +1] + alfabe[alfabe.index(kelime_gir[5]) +1] + alfabe[alfabe.index(kelime_gir[6]) +1] + alfabe[alfabe.index(kelime_gir[7]) +1] + alfabe[alfabe.index(kelime_gir[8]) +1] + alfabe[alfabe.index(kelime_gir[9]) +1] + alfabe[alfabe.index(kelime_gir[10]) +1] + alfabe[alfabe.index(kelime_gir[11]) +1])
   sifresi_cozulmus = str(alfabe[alfabe.index(sifreli_kelime[0]) -1] + alfabe[alfabe.index(sifreli_kelime[1]) -1] + alfabe[alfabe.index(sifreli_kelime[2]) -1] + alfabe[alfabe.index(sifreli_kelime[3]) -1] + alfabe[alfabe.index(sifreli_kelime[4]) -1] + alfabe[alfabe.index(sifreli_kelime[5]) -1] + alfabe[alfabe.index(sifreli_kelime[6]) -1] + alfabe[alfabe.index(sifreli_kelime[7]) -1] + alfabe[alfabe.index(sifreli_kelime[8]) -1] + alfabe[alfabe.index(sifreli_kelime[9]) -1] + alfabe[alfabe.index(sifreli_kelime[10]) -1] + alfabe[alfabe.index(sifreli_kelime[11]) -1] )
else:
    print("Bir Hata Oluştu")

print(kelime_gir +" kelimesinin şifreli hali ==> "+sifreli_kelime)
print(kelime_gir+" kelimesinin şifresi çözülmüş hali ==> "+sifresi_cozulmus)
