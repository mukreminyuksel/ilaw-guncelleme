# iLaw Hukuk — uygulama güncellemelerinin dosyaları

Herkese açık `mukreminyuksel/ilaw-guncelleme` deposu (GitHub Pages: `https://mukreminyuksel.github.io/ilaw-guncelleme/`).
Uygulamanın kurmadan gelen güncellemelerinin (v0.13 ve sonrası) dosyaları burada durur. İçeriği elle değiştirilmez;
`node scripts/guncelleme.cjs hazirla` (ana depo) üretir.

- `d/<sha256>.<uzantı>`: paket ve varlıklar, içerik karmasıyla adlandırılır; aynı dosya bir kez yüklenir ve adres hiç değişmez.
- `m/<kanal>/<parmak izi>/<kimlik>.json`: yayımlanan manifestler (geri alma bunlardan üretilir).

Dosyalar herkese açıktır; zaten APK'nın içinde olan uygulama kodudur. Telefon bir güncellemeyi yalnız Mac'teki özel
anahtarla imzalanmışsa kurar (imza ve hangi telefona hangi güncellemenin gideceği sunucudadır); bu depo ele geçirilse
bile imzasız kod telefona kurulamaz. Ayrıntı: ana depoda docs/PLAN_V013.md §2.
