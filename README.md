# PYTHON-PREDICT-NUMBER-GAME-
###########################################################################
########################## SAYI TAHMİN OYUNU ##############################
###########################################################################










print("SAYI TAHMİN OYUNUNA HOŞGELDİN")
import random
while True:

    tuttuğu_sayı=random.randint(1,100)
    tahmin_hakkı=7
    print("1 ile 100 arası bir sayı tuttum.7 hakkın var tahmin et bakalım .")

    while tahmin_hakkı>0:
        n=int(input("Tahmini Giriniz:"))
        tahmin_hakkı-=1

        if n==tuttuğu_sayı:
            print("TEBRİKLER!Doğru Tahmin.")
            break
        elif n<tuttuğu_sayı:
            print("Daha büyük bir sayıyıyla dene.")
        else:
            print("Daha küçük bir sayıyla dene")
        print("Kalan Tahmin Hakkınız:",tahmin_hakkı)
        
    if  n!=tuttuğu_sayı:
        print("Bilemediniz doğru sayı : ",tuttuğu_sayı,"idi.")
    print("OYUNU TEKRAR OYNAMAK İSTERSEN A YE ÇIKMAK İSTERSEN E YE BAS.")
    tekrar_isteği=(input("A/E")).upper()
    if tekrar_isteği!="A":
        print("HOŞÇAKALLLL")
        break
