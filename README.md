# Hertz Motor Stok/Operasyon Uygulaması (GitHub Pages Paketi)

Bu paket, tek sayfalık uygulamanızı GitHub Pages üzerinde çalışacak şekilde hazırlar.

## İçerik
- `index.html`: Uygulamanın ana dosyası (Firebase entegrasyonu eklendi).
- `404.html`: SPA yönlendirme sayfası (GitHub Pages altında path tabanlı yönlendirme için).
- `.nojekyll`: Jekyll işlemeyi devre dışı bırakır.
- `assets/`: Statik varlıklar (örnek logo.svg dahil).

## Yayınlama (GitHub Pages)
1. GitHub'da **yeni bir repository** oluşturun (örn. `hertz-motor-stok`).
2. Bu paketin içeriğini **repo köküne** kopyalayın ve push edin.
3. **Settings → Pages** bölümünde:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` / **root**
   - Kaydedin.
4. 1-2 dakika içinde Pages URL'iniz aktif olur (örn. `https://<kullanici>.github.io/<repo-adi>/`).

> Notlar:
> - Uygulama CDN üzerinden (Firebase, Tailwind, Flatpickr vb.) çalışır; ek build gerekmez.
> - Firebase Analytics bazı tarayıcı/ortamlarda (3rd‑party cookie, http vs.) kısıtlı olabilir; `isSupported()` kontrolü eklidir.
> - Kendi domain’iniz varsa `CNAME` dosyası ekleyerek Pages’a bağlayabilirsiniz.

_Tarih:_ 2025-09-09
