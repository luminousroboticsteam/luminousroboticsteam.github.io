# Luminous Robotics Team — Sitesi

Luminous Robotics Team (Takım 9233) için hazırlanmış statik takım sitesi. GitHub Pages üzerinde ücretsiz barındırılır.

- `index.html` — ana sayfa (takım tanıtımı: hakkımızda, yarışmalar, başarılar, STEM, Kickoff, sponsorluk)
- `takvim.html` — sezon takvimi
- `events.json` — takvim verisi
- `assets/` — logo, fotoğraflar ve favicon dosyaları
- `robots.txt`, `sitemap.xml` — arama motorları için
- `404.html` — sayfa bulunamadı ekranı

## Bu güncellemede neler düzeltildi

- **Mobil menü**: Telefonda artık hamburger (☰) ikonuna basınca tüm bölüm linkleri (Hakkımızda, Yarışmalar vb.) açılıyor — önceden sadece "Takvim" butonu görünüyordu.
- **Paylaşım önizlemesi**: WhatsApp/Instagram'da link paylaşınca artık başlık, açıklama ve kapak fotoğrafı çıkıyor (Open Graph etiketleri eklendi).
- **Favicon**: Tarayıcı sekmesinde ve telefona ana ekrana eklerken artık Luminous logosu görünüyor.
- **Hız**: `fyf-logo.png` ve `first-logo.png` gereksiz büyüktü, küçültüldü; kullanılmayan `award.jpg` silindi; görsellerin çoğuna "lazy load" eklendi (sayfa daha hızlı açılıyor).
- **404 sayfası**: Yanlış bir adrese gidildiğinde artık markaya uygun bir "sayfa bulunamadı" ekranı çıkıyor.
- **robots.txt / sitemap.xml**: Arama motorları için eklendi.

**Yapman gereken tek şey:** Bu klasördeki tüm dosyaları (değişmemiş olanlar dahil) GitHub reponun üzerine tekrar yükleyip Commit changes demek — özellikle `assets/` klasörünü komple yeniden yükle (eski `award.jpg` otomatik silinmez, istersen GitHub'da elle silebilirsin) ve yeni eklenen `404.html`, `robots.txt`, `sitemap.xml` dosyalarını da reponun ana dizinine ekle.

## Kurulum — yeni repo: `luminousroboticsteam.github.io`

Kullanıcı adın artık `luminousroboticsteam` olduğu için, reponu tam olarak `luminousroboticsteam.github.io` adıyla oluşturursan site doğrudan kök adreste (`https://luminousroboticsteam.github.io/`, sonunda ekstra bir klasör adı olmadan) yayınlanır.

1. GitHub'da yeni bir repo oluştur, adı **tam olarak** `luminousroboticsteam.github.io` olacak (büyük/küçük harf önemli değil ama yazım birebir bu olmalı), **Public** olarak.
2. Reponun ana sayfasında **Add file → Upload files** ile bu klasördeki tüm dosya ve klasörleri yükle: `index.html`, `takvim.html`, `events.json`, `README.md`, `assets/` (klasörü olduğu gibi sürükleyip bırak).
3. "Commit changes" ile kaydet.
4. Bu özel isimli repo için GitHub Pages otomatik olarak devreye girer (genelde ekstra bir ayara gerek kalmaz); yine de kontrol etmek istersen **Settings → Pages** sayfasına git, "Branch" olarak `main` ve `/ (root)` seçili olduğundan emin ol.
5. Birkaç dakika içinde site şu adreste yayında olacak: `https://luminousroboticsteam.github.io/`

`events.json` dosyasındaki `"repo"` alanı zaten `luminousroboticsteam/luminousroboticsteam.github.io` olarak ayarlandı, ekstra bir şey yapmana gerek yok — "+ Etkinlik ekle" düğmesi otomatik doğru yere gidecek.

## İçerik güncelleme

- **Takvime etkinlik eklemek/düzeltmek:** `takvim.html` sayfasındaki "+ Etkinlik ekle" düğmesi `events.json` dosyasını GitHub'da açar; ilgili ayın listesine yeni bir satır ekleyip kaydetmen yeterli.
- **Ana sayfadaki metni değiştirmek:** `index.html` dosyasını GitHub'da aç (kalem/pencil ikonuyla düzenleme moduna geç), ilgili yazıyı bul ve değiştir, Commit changes ile kaydet.
- **Fotoğraf değiştirmek:** `assets/` klasörüne git, değiştirmek istediğin dosyayı sil ve yerine aynı isimde yeni bir fotoğraf yükle (örn. `hero.jpg`'yi değiştirmek için yeni fotoğrafı da `hero.jpg` adıyla yükle).

Kodla ilgili bir sorun yaşarsan dosyayı olduğu gibi Claude'a gönderip yardım isteyebilirsin.
