# 🔺 Pyramid Game Simülasyonu

Filmdeki **Pyramid Game** mantığıyla çalışan, arkadaşlarınla oynayabileceğin basit bir ranking oyunu.

## Özellikler

- Kayıt / Giriş (kullanıcı adı + şifre)
- Oda kurma (oda kodu + **Rank şifresi**)
- Odaya katılma
- Gizli oylama (1-2-3 sıralı tercih)
- A → F piramit sıralaması
- F olan kişiye şaka cezası
- Mobil uyumlu (Ana Ekrana Ekle ile uygulama gibi çalışır)

## Nasıl Oynanır?

1. Herkes siteye girip **kayıt olur** / giriş yapar
2. Biri **Oda Kur** der → oda adı + **Rank şifresi** belirler
3. Oda kodu çıkar (6 haneli)
4. Diğerleri oda kodu + Rank şifresi ile katılır
5. Host **Oylamayı Başlat** der
6. Herkes gizli oyunu kullanır (en sevdiği 3 kişi)
7. Sonuçlar çıkar → A'dan F'ye sıralama

## Önemli Not

Bu uygulama **sadece eğlence** amaçlıdır.  
Gerçek hayatta zorbalık / eziyet için kullanılmamalıdır.

## Teknik

- Tamamen tarayıcıda çalışır (localStorage)
- Aynı cihaz / aynı tarayıcı profilinde en iyi çalışır
- Farklı telefonlarda oynamak için aynı Wi-Fi + aynı tarayıcı verisi paylaşımı gerekir (veya daha sonra Firebase eklenebilir)

## Kurulum

Sadece `index.html` dosyasını tarayıcıda açman yeterli.  
GitHub Pages ile yayınlayabilirsin.
