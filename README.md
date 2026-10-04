# 🔺 Pyramid Game (Firebase'li)

Filmdeki **Pyramid Game** mantığıyla çalışan, arkadaşlarınla **farklı telefonlardan** oynayabileceğin ranking oyunu.

## Özellikler

- **Kayıt / Giriş** (E-posta + şifre)
- **Oda kurma** → Oda kodu + **Rank Şifresi**
- Gerçek zamanlı (Firebase)
- Gizli oylama (1-2-3 tercih)
- A → F piramit sıralaması
- F olan kişiye şaka cezası
- Mobil uyumlu (Ana Ekrana Ekle)

## Firebase Kurulumu (5 dakika)

1. https://console.firebase.google.com adresine gir
2. **Add project** → isim ver (örnek: pyramid-game)
3. Google Analytics'i kapatabilirsin (isteğe bağlı)
4. Proje oluşunca:
   - Sol menüden **Build → Authentication** → Get started
   - **Sign-in method** → **Email/Password** → Enable → Save
5. Sol menüden **Build → Firestore Database** → Create database
   - **Start in test mode** seç (1 ay açık kalır, sonra kuralları sıkılaştırırsın)
   - Location: `europe-west` veya en yakın
6. Sol üstte **Project Overview** → **</>** (Web) butonuna tıkla
   - App nickname ver → Register app
   - Çıkan `firebaseConfig` objesini kopyala
7. `index.html` dosyasını aç, şu kısmı bul:

```js
const firebaseConfig = {
  apiKey: "BURAYA_API_KEY",
  authDomain: "BURAYA_AUTH_DOMAIN",
  projectId: "BURAYA_PROJECT_ID",
  storageBucket: "BURAYA_STORAGE_BUCKET",
  messagingSenderId: "BURAYA_MESSAGING_SENDER_ID",
  appId: "BURAYA_APP_ID"
};
```

8. Kendi config değerlerini yapıştır → kaydet
9. Dosyayı tarayıcıda aç veya GitHub Pages'e yükle

## Nasıl Oynanır?

1. Herkes siteye girip **Kayıt Ol** / **Giriş Yap**
2. Biri **Oda Kur** → Rank şifresi belirler
3. Oda kodu çıkar
4. Diğerleri **Oda Kodu + Rank Şifresi** ile katılır
5. Host **Oylamayı Başlat** der
6. Herkes kendi telefonundan gizli oyunu kullanır
7. Sonuçlar herkese aynı anda çıkar

## Önemli Not

Bu uygulama **sadece eğlence** amaçlıdır.  
Gerçek hayatta zorbalık için kullanılmamalıdır.

## Teknik

- Firebase Authentication (Email/Password)
- Cloud Firestore (gerçek zamanlı odalar)
- Tamamen client-side
