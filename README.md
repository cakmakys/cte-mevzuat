# CTE Mevzuat Arşivi

Ceza ve Tevkifevleri Genel Müdürlüğü personeline yönelik mevzuat, yönetmelik, genelge ve tebliğ arşivini sunan kapsamlı ve kullanıcı dostu web sitesi.

## Özellikler

### 📋 Kapsamlı Mevzuat Arşivi
- Kanunlar, Yönetmelikler, Genelgeler ve Tebliğler
- Güncel ve tam metin mevzuat içerikleri
- Kategorilere göre düzenlenmiş yapı

### 🔍 Gelişmiş Arama ve Filtreleme
- Metin tabanlı arama (başlık ve içerik)
- Kategori bazlı filtreleme
- Arama ve filtrelerin birlikte çalışması

### ⭐ Favoriler Sistemi
- Mevzuatları favorilere ekleme/çıkarma
- Favoriler localStorage'da saklanır
- Ayrı favoriler sayfası

### 📱 Responsive Tasarım
- Mobil ve masaüstü uyumlu
- Modern ve temiz arayüz
- Kullanıcı dostu navigasyon

### 🎨 Modern UI/UX
- Shadcn/UI bileşenleri
- Tailwind CSS ile stillendirilmiş
- Lucide ikonları
- Hover efektleri ve geçişler

## Teknolojiler

- **Frontend Framework:** React 18
- **Styling:** Tailwind CSS
- **UI Components:** Shadcn/UI
- **Icons:** Lucide React
- **Build Tool:** Vite
- **Package Manager:** PNPM

## Kurulum

### Gereksinimler
- Node.js 18+ 
- PNPM (önerilen) veya NPM

### Adımlar

1. **Projeyi klonlayın:**
   ```bash
   git clone <repository-url>
   cd cte-mevzuat-sitesi
   ```

2. **Bağımlılıkları yükleyin:**
   ```bash
   pnpm install
   # veya
   npm install
   ```

3. **Geliştirme sunucusunu başlatın:**
   ```bash
   pnpm run dev
   # veya
   npm run dev
   ```

4. **Tarayıcıda açın:**
   ```
   http://localhost:5173
   ```

## Kullanım

### Ana Sayfa
- Tüm mevzuatlar liste halinde görüntülenir
- Her mevzuat kartında kategori, başlık, yayın tarihi ve kısa önizleme bulunur

### Arama
- Üst kısımdaki arama kutusunu kullanarak mevzuat başlığı veya içeriğinde arama yapabilirsiniz
- Arama sonuçları anlık olarak güncellenir

### Filtreleme
- Kategori dropdown'ından istediğiniz kategoriyi seçerek filtreleme yapabilirsiniz
- Kategoriler: Tümü, Kanun, Yönetmelik, Genelge, Tebliğ

### Favoriler
- Her mevzuat kartındaki kalp ikonuna tıklayarak favorilere ekleyebilirsiniz
- Favoriler butonuna tıklayarak sadece favori mevzuatları görüntüleyebilirsiniz
- Favoriler tarayıcınızda saklanır (localStorage)

### Detay Görünümü
- "Devamını oku" linkine tıklayarak mevzuatın tam metnini okuyabilirsiniz
- Detay sayfasında da favori ekleme/çıkarma işlemi yapabilirsiniz

## Proje Yapısı

```
cte-mevzuat-sitesi/
├── public/
│   ├── mevzuat.json          # Mevzuat verileri
│   └── ...
├── src/
│   ├── components/
│   │   └── ui/               # Shadcn/UI bileşenleri
│   ├── App.jsx               # Ana uygulama bileşeni
│   ├── App.css               # Ana stil dosyası
│   └── main.jsx              # Uygulama giriş noktası
├── package.json
├── tailwind.config.js
├── vite.config.js
└── README.md
```

## Veri Yapısı

Mevzuat verileri `public/mevzuat.json` dosyasında JSON formatında saklanır:

```json
{
  "id": "benzersiz-id",
  "kategori": "Kanun|Yönetmelik|Genelge|Tebliğ",
  "başlık": "Mevzuat başlığı",
  "içerik": "Mevzuat tam metni",
  "yayın_tarihi": "YYYY-MM-DD"
}
```

## Geliştirme

### Yeni Mevzuat Ekleme
1. `public/mevzuat.json` dosyasını açın
2. Yukarıdaki veri yapısına uygun yeni mevzuat objesi ekleyin
3. Benzersiz bir `id` kullanmaya dikkat edin

### Stil Değişiklikleri
- Tailwind CSS sınıfları kullanılarak stillendirme yapılmıştır
- Özel stiller için `src/App.css` dosyasını düzenleyebilirsiniz

### Yeni Özellik Ekleme
- React bileşen yapısını takip edin
- Shadcn/UI bileşenlerini tercih edin
- Responsive tasarım prensiplerini gözetin

## Build ve Deploy

### Production Build
```bash
pnpm run build
# veya
npm run build
```

Build dosyaları `dist/` klasöründe oluşturulur.

### Preview
```bash
pnpm run preview
# veya
npm run preview
```

## Lisans

Bu proje Ceza ve Tevkifevleri Genel Müdürlüğü için geliştirilmiştir.

## Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/yeni-ozellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin feature/yeni-ozellik`)
5. Pull Request oluşturun

## Destek

Herhangi bir sorun veya öneriniz için lütfen issue açın.

---

**Geliştirici:** Manus AI  
**Tarih:** 2025  
**Versiyon:** 1.0.0

