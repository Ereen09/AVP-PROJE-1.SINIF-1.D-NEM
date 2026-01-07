# AVP-PROJE-1.SINIF-1.DÖNEM
Proje Bilgileri

1. Proje Bilgileri

Geliştirici: Nevzat Eren Koyuncu

Bölüm: Bilgisayar Mühendisliği

Programlama Dili: C

Uygulama Türü: Konsol (Terminal)

Proje Tipi: Bireysel

2. Genel Çalışma Yapısı

Program, kullanıcı etkileşimine dayalı bir menü sistemi ile çalışır.

Program başlangıcında kullanıcıdan bilim insanı adı alınır

Ana menüde 9 farklı fizik deneyi sunulur

Kullanıcı deney numarasını girerek seçim yapar

-1 girilmesi durumunda program güvenli şekilde sonlandırılır

Deneye ait fiziksel parametreler kullanıcıdan alınır

Negatif girilen değerler ternary operatörü ile mutlak değere çevrilir

Hesaplamalar 8 gezegen için ayrı ayrı yapılır

Sonuçlar gezegen isimleriyle birlikte ekrana yazdırılır

3. Kullanılan Gezegenler ve Yerçekimi İvmeleri

Tüm hesaplamalar aşağıdaki gezegenlerin yüzey yerçekimi ivmeleri (m/s^2) kullanılarak gerçekleştirilir:

Merkür : 3.70

Venüs : 8.87

Dünya : 9.81

Mars : 3.71

Jüpiter : 24.79

Satürn : 10.44

Uranüs : 8.69

Neptün : 11.15

4. Fizik Deneyleri ve Matematiksel Modeller
4.1 Serbest Düşme

Formül:
h = (1/2) * g * t^2

Hesaplanan değer:
Belirli bir sürede alınan yol (metre)

4.2 Yukarı Atış (Maksimum Yükseklik)

Formül:
h_max = v0^2 / (2 * g)

Hesaplanan değer:
Cismin ulaşabileceği maksimum yükseklik (metre)

4.3 Kütle – Ağırlık Dönüşümü

Formül:
G = m * g

Hesaplanan değer:
Ağırlık kuvveti (Newton)

4.4 Potansiyel Enerji

Formül:
Ep = m * g * h

Hesaplanan değer:
Potansiyel enerji (Joule)

4.5 Hidrostatik Basınç

Formül:
P = rho * g * h

Hesaplanan değer:
Basınç (Pascal)

4.6 Arşimet Kaldırma Kuvveti

Formül:
Fk = rho * g * V

Hesaplanan değer:
Kaldırma kuvveti (Newton)

4.7 Basit Sarkaç Periyodu

Formül:
T = 2 * pi * sqrt(L / g)

Hesaplanan değer:
Bir tam salınım süresi (saniye)

4.8 Statik İp Gerilmesi

Formül:
T = m * g

Hesaplanan değer:
İp gerilmesi (Newton)

4.9 Asansör Dinamiği (Hissedilen Ağırlık)

Formül:
N = m * (g + a) veya N = m * (g - a)

Hesaplanan değer:
Normal kuvvet (Newton)

5. Teknik Uygulama Detayları

Her fizik deneyi ayrı bir fonksiyon olarak tanımlanmıştır

Gezegen yerçekimi ivmeleri sabit bir dizi içinde tutulur

Dizilere erişim C pointer aritmetiği ile sağlanır

Negatif değerler için ternary operatörü (? :) kullanılmıştır

Kullanılan sabitler:

PI = 3.141592653589793

GEZEGEN_SAYISI = 8

6. Derleme ve Çalıştırma
gcc main.c -o fizik_sim -lm
./fizik_sim

7. Geliştirme ve İyileştirme Olanakları

Yerçekimi ivmesinin dinamik olarak hesaplanması
g = G * M / R^2

Eğik atış (iki boyutlu hareket) analizlerinin eklenmesi

Kinetik enerji ve yapılan iş hesaplamalarının dahil edilmesi

Ortak bir mutlak değer kontrol fonksiyonu yazılması

8. Kaynaklar

Halliday, D., Resnick, R., Walker, J. – Fundamentals of Physics

NASA Solar System Exploration – Planetary Fact Sheet

GeeksforGeeks – Pointers and Arrays in C Programming

9. Sonuç

Bu çalışma, temel fizik yasalarını C programlama dili ile modüler ve sistematik bir yapıda uygulamaktadır.
Aynı fiziksel olayın farklı gezegenlerdeki sonuçlarını karşılaştırmalı biçimde sunması, projeyi eğitici ve teknik açıdan güçlü kılmaktadır.
