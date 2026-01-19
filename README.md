# Say-tahmin-oyunu
import random

print("🎯 Sayı Tahmin Oyununa Hoş Geldin!")
print("1 ile 100 arasında bir sayı tuttum.")

tutulan_sayi = random.randint(1, 100)
tahmin_sayisi = 0

while True:
    tahmin = int(input("Tahminini gir: "))
    tahmin_sayisi += 1

    if tahmin < tutulan_sayi:
        print("⬆️ Daha büyük bir sayı dene.")
    elif tahmin > tutulan_sayi:
        print("⬇️ Daha küçük bir sayı dene.")
    else:
        print(f"🎉 Tebrikler! {tahmin_sayisi} denemede bildin.")
        break
