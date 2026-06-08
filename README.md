# Daurin Website

Landing page statis untuk project Daurin.

**Live site:** https://cristianphi.github.io/Daurin-Webstie/

## Struktur

```
Daurin-Website/
├── index.html
├── downloads/daurin.apk
└── .github/workflows/deploy-pages.yml
```

## Deploy (GitHub Pages)

1. Push semua file ke repo `CristianPhi/Daurin-Webstie`
2. Buka **Settings → Pages**
3. **Build and deployment → Source:** pilih **GitHub Actions**
4. Tunggu workflow **Deploy GitHub Pages** selesai (tab Actions)
5. Buka https://cristianphi.github.io/Daurin-Webstie/

## Download APK (penting!)

Tombol download pakai **GitHub Releases** (lebih stabil untuk file ~54 MB):

```
https://github.com/CristianPhi/Daurin-Webstie/releases/latest/download/daurin.apk
```

### Buat release (sekali saja, ulangi tiap update APK)

1. Buka https://github.com/CristianPhi/Daurin-Webstie/releases
2. Klik **Create a new release**
3. Tag: `v1.0` (atau v1.1, v1.2, dst.)
4. Title: `Daurin v1.0`
5. Drag & drop `downloads/daurin.apk` ke **Release assets**
6. Pastikan nama file asset = **`daurin.apk`**
7. Klik **Publish release**

Tanpa release ini, tombol download di website live **tidak akan jalan**.

## Tes lokal

```powershell
cd "c:\Cristian Philander\Binus\Semester 4\Mobile Hybrid Solution\Daurin-Website"
npx --yes serve .
```

Untuk tes lokal, ganti sementara `href` tombol ke `downloads/daurin.apk`.
