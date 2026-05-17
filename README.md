# Osmanlıca Transkripsiyon ve Sadeleştirme Aracı (Sürüm 5.0)

Bu proje, Osmanlıca metinlerin transkripsiyonel çevirisini yapan ve aynı zamanda günümüz Türkçesine sadeleştiren web tabanlı, tamamen ücretsiz bir yazılımdır. Geliştirilen özel motor sayesinde, sunucu taraflı bağımlılıklara veya CORS engellerine takılmadan doğrudan tarayıcı üzerinde tıkır tıkır çalışır.

## 🚀 Canlı Önizleme
Proje GitHub Pages üzerinde aktiftir. Doğrudan şu adresten deneyebilirsiniz:
👉 <a href="https://akhenaton41.github.io/Osmanlica-Ceviri/" target="_blank">Osmanlıca Çeviri Aracı Canlı Önizleme</a>

## 🛠️ Öne Çıkan Özellikler
- **Çift Yönlü Çıktı Dünyası:** Girilen Osmanlıca metni eş zamanlı olarak hem transkripsiyon alfabesine çevirir hem de günümüz Türkçesiyle sadeleştirir.
- **Akıllı Dosya Okuma Mimarisi:** "Örnek Metinler" ve "Dosyadan Yükle" modülleri, GitHub reponuzdaki veya yerel dosya sisteminizdeki `.txt` ve `.rtf` dosyalarını tarayıcının `FileReader` yetenekleriyle tamamen yerelde okur. Bu sayede hiçbir internet veya güvenlik engeline takılmaz.
- **Canlı Durum İzleme (MutationObserver):** Çeviri çıktılarının yüklendiği alanlar modern DOM izleyicileriyle takip edilir; veri akışı tamamlandığı an yükleme ekranları otomatik olarak gizlenir.
- **Gelişmiş İstatistik Paneli:** Veri bankasındaki transkripsiyonel karakter, Osmanlıca kural, kelime ve rütuş kurallarının sayısını anlık olarak listeler.

## 📁 Klasör Yapısı
```text
Osmanlica-Ceviri/
├── css/
│   ├── buton.css         # Retro / Modern buton tasarımları
│   └── font.css          # Gerekli yazı tipleri ve font yüzleri
├── javascript/
│   ├── jquery.min.js     # Temel DOM kütüphanesi
│   ├── kelimeler.js      # Kelime veri bankası ve kural dizileri
│   └── ocr.js            # Görselden metin çözümleme modülü
├── örnek dosyalar/       # Test edebileceğiniz hazır Osmanlıca metin arşivleri (.txt)
└── index.htm             # Projenin ana giriş ve motor dosyası
