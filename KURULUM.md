# Senza Atelier – Kurulum (bir kereliğine)

## A) GitHub'a yükle
1. github.com'da hesap aç (ücretsiz) → **New repository** → adı: `senza-atelier` → Private seçebilirsin → Create.
2. "uploading an existing file" linkine tıkla → bu klasörün İÇİNDEKİ her şeyi (index.html, admin, data, images) sürükle → **Commit changes**.
3. `admin/config.yml` dosyasını GitHub'da aç → kalem simgesi → `repo:` satırını `KULLANICIADIN/senza-atelier` yap → Commit.

## B) Netlify'ı GitHub'a bağla
1. Netlify → Add new site → **Import an existing project** → GitHub → `senza-atelier` repo'sunu seç → Deploy.
   (Mevcut siteyi silmene gerek yok; domaini yeni siteye taşıyabilirsin: Domain management.)
2. GitHub → Settings → Developer settings → OAuth Apps → **New OAuth App**
   - Homepage URL: `https://SITEN.com`
   - Callback URL: `https://api.netlify.com/auth/done`
   - Oluşan **Client ID** ve **Client Secret**'ı kopyala.
3. Netlify → Site configuration → Access & security → **OAuth** → Install provider → GitHub → ID ve Secret'ı yapıştır.

## C) Amcan nasıl kullanır
1. `https://SITEN.com/admin` adresine gir → **Login with GitHub**.
   (Amcanın ayrı GitHub hesabı varsa: Repo → Settings → Collaborators → Add people.)
2. **Ürünler → Tüm Ürünler → Ürün ekle** → ad, kategori, fiyat yaz, fotoğrafı seç.
3. Üstten **Publish → Publish now**. 1 dakika içinde sitede görünür.
Silmek / fiyat değiştirmek için aynı ekrandan ürünü aç, düzenle, yayınla.
