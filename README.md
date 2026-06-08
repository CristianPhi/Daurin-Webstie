# Daurin Website

Landing page statis untuk project Daurin — terpisah dari GenshinImport.

## Struktur

```
Daurin-Website/
├── index.html          ← halaman utama
├── downloads/
│   └── daurin.apk      ← taruh APK di sini
└── README.md
```

## Cara link download (Chrome langsung download)

Tombol **Download APK** di `index.html` sudah di-set ke:

```html
<a href="downloads/daurin.apk" download="Daurin.apk">Download APK</a>
```

Yang perlu kamu lakukan:
1. Build APK dari Flutter (`flutter build apk --release`)
2. Copy ke `downloads/daurin.apk`
3. Host folder ini di server (jangan buka lewat `file://`)

## Tes lokal

```powershell
cd "c:\Cristian Philander\Binus\Semester 4\Mobile Hybrid Solution\Daurin-Website"
npx --yes serve .
```

Buka http://localhost:3000 → klik **Download APK**.

## Hosting gratis

| Platform | Cara |
|----------|------|
| **Netlify** | Drag & drop folder `Daurin-Website` ke netlify.com |
| **GitHub Pages** | Push repo, aktifkan Pages di Settings |
| **Vercel** | Import/upload folder, deploy |

Upload seluruh isi folder (termasuk `downloads/daurin.apk`).

## Ganti file download

Edit `href` dan `download` di tombol `#apk-btn` di `index.html`:

```html
<a href="downloads/nama-file.apk" download="NamaTampilan.apk" ...>
```
