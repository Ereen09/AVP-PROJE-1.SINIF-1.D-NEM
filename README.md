# AVP-PROJE-1.SINIF-1.DÖNEM
Proje Bilgileri

Geliştirici: Nevzat Eren Koyuncu

Bölüm: Bilgisayar Mühendisliği

Dil: C

Proje Türü: Bireysel

Platform: Konsol (Terminal)

Programın Çalışma Mantığı

Program başlangıcında kullanıcıdan bilim insanı adı alınır

Kullanıcıya 9 farklı fizik deneyi içeren bir ana menü gösterilir

Kullanıcı deney seçimini yapar

-1 girildiğinde program güvenli şekilde sonlandırılır

Deneye özel fiziksel parametreler kullanıcıdan alınır

Negatif girilen fiziksel değerler ternary operatörü ile pozitife çevrilir

Hesaplamalar 8 gezegenin yerçekimi ivmesi kullanılarak yapılır

Sonuçlar gezegen isimleriyle birlikte ekrana yazdırılır

Program tekrar ana menüye döner

Kullanılan Gezegenler ve Yerçekimi İvmeleri (m/s^2)

Merkür: 3.70

Venüs: 8.87

Dünya: 9.81

Mars: 3.71

Jüpiter: 24.79

Satürn: 10.44

Uranüs: 8.69

Neptün: 11.15

İçerilen Fizik Deneyleri ve Formüller

Serbest Düşme
Formül:
h = (1/2) * g * t^2
Hesaplanan değer: Alınan yol (metre)

Yukarı Atış (Maksimum Yükseklik)
Formül:
h_max = v0^2 / (2 * g)
Hesaplanan değer: Maksimum yükseklik (metre)

Kütle – Ağırlık Dönüşümü
Formül:
G = m * g
Hesaplanan değer: Ağırlık kuvveti (Newton)

Potansiyel Enerji
Formül:
Ep = m * g * h
Hesaplanan değer: Potansiyel enerji (Joule)

Hidrostatik Basınç
Formül:
P = rho * g * h
Hesaplanan değer: Basınç (Pascal)

Arşimet Kaldırma Kuvveti
Formül:
Fk = rho * g * V
Hesaplanan değer: Kaldırma kuvveti (Newton)

Basit Sarkaç Periyodu
Formül:
T = 2 * pi * sqrt(L / g)
Hesaplanan değer: Periyot (saniye)

Statik İp Gerilmesi
Formül:
T = m * g
Hesaplanan değer: İp gerilmesi (Newton)

Asansör Dinamiği (Hissedilen Ağırlık)
Formül:
N = m * (g + a) veya N = m * (g - a)
Hesaplanan değer: Normal kuvvet (Newton)

Teknik Detaylar

Her deney ayrı bir fonksiyon olarak tanımlanmıştır

Gezegen yerçekimi ivmeleri bir dizi içinde tutulur

Dizilere erişim pointer aritmetiği kullanılarak yapılır

Negatif girişler için ternary operatörü (? :) ile mutlak değer alınır

Sabitler:

PI = 3.141592653589793

GEZEGEN_SAYISI = 8

Derleme ve Çalıştırma
gcc main.c -o fizik_sim -lm
./fizik_sim

Geliştirme Önerileri

Yerçekimi ivmesini sabit yerine dinamik hesaplama
g = G * M / R^2

Eğik atış analizlerinin eklenmesi

Kinetik enerji ve yapılan iş hesaplamalarının eklenmesi

Negatif değer kontrolü için ortak yardımcı fonksiyon yazılması

Kaynaklar

Halliday, Resnick, Walker – Fundamentals of Physics

NASA Solar System Exploration – Planetary Fact Sheet

GeeksforGeeks – Pointers and Arrays in C

Sonuç

Bu proje, temel fizik yasalarını C dilinde modüler ve karşılaştırmalı bir yapı ile uygulamaktadır.
Sekiz gezegen üzerinde aynı deneyleri gerçekleştirmesi, projeyi öğretici ve teknik olarak güçlü hale getirmektedir.
