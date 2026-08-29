# مستند صوتی شنود

#استخراج فایل ZIP پروژه

ابتدا فایل ZIP را Extract کنید و سپس محتویات پوشه "mostanad_shonud" را مستقیماً در ریشه Repository گیت‌هاب قرار دهید.

توجه: خود پوشه "mostanad_shonud" نباید به‌عنوان یک پوشهٔ اضافی داخل Repository قرار بگیرد. ساختار Repository باید از این مسیرها شروع شود:

assets/
.github/
android/
lib/
README.md
.gitignore
pubspec.yaml

## فایل‌هایی که خودتان باید اضافه کنید قبل از بیلد

لوگو از قبل اضافه شده (`assets/logo.png`). فقط فایل‌های صوتی (mp3) باقی مانده‌اند — دقیقاً با همین نام‌ها در مسیر `assets/audio/` قرار دهید:

**فصل یک (۱۶ فایل):**
```
mostanad_soti_shonud_part1.mp3
mostanad_soti_shonud_part2.mp3
mostanad_soti_shonud_part3.mp3
...
mostanad_soti_shonud_part16.mp3
```

**فصل دوم (۲ فایل):**
```
mostanad_soti_shonud_s2_part1.mp3
mostanad_soti_shonud_s2_part2.mp3
```

همه‌ی این ۱۸ نام از قبل توی `pubspec.yaml` (بخش assets) نوشته شده‌اند؛ کافی است خود فایل‌ها را با همین اسم‌ها در پوشه بگذارید — نیازی به تغییر کد نیست.
## حجم برنامه
با توجه به این‌که حدود ۳۰۰ مگابایت فایل صوتی اضافه شده و برنامه خودش (بدون صدا) چند مگابایت بیشتر نیست حجم نهایی برنامه حدود ۳۳۰ مگابایت میشود.
## امضا دیجیتال برنامه
با تنظیم Secret های زیر در گیت‌هاب، ورک‌فلو به‌صورت خودکار apk امضاشده تولید می‌کند: `KEYSTORE_BASE64`, `KEYSTORE_PASSWORD`, `KEY_ALIAS`, `KEY_PASSWORD`

