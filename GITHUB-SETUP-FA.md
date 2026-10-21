# راهنمای گام‌به‌گام ثبت NetBond در گیت‌هاب (مرحلهٔ ۲)

همهٔ فایل‌های لازم برای مخزن، کنار همین راهنماست. شما فقط کلیک می‌کنید؛
هیچ خط فرمانی لازم نیست.

## ۰) قبل از هر چیز: چه چیزی عمومی می‌شود و چه چیزی هرگز نه

| ✅ عمومی (داخل همین کیت) | ❌ هرگز آپلود نکنید |
|---|---|
| README.md / README.fa.md | netbond_license_private.key |
| LICENSE | keygen.py / seller_desk.py / SellerDesk.bat |
| assets/ (آیکون + پوسترها) | keys_issued.log / SELLER_RUNBOOK.md |
| docs/ (راهنماهای ۴ زبان) | **netbond-1.6.5.zip (نسخهٔ کامل!)** |
| RELEASE-NOTES.md | پوشهٔ private/ و NetBond-Seller-Kit.zip |

تنها فایل اجرایی عمومی = **zip آزمایشی** که به‌صورت Release ضمیمه می‌شود.
نسخهٔ کامل فقط پس از پرداخت تحویل می‌شود؛ این ستون فقرات کسب‌وکار شماست.
(سورس‌کد هم عمومی نمی‌شود؛ مخزن = ویترین + دانلود آزمایشی + مستندات.)

## ۱) ساخت حساب (۵ دقیقه)
1. browser: `github.com` → **Sign up**
2. ایمیل واقعی + رمز قوی + نام کاربری پیشنهادی: `netbond-app` (یا هر نام
   خالی). تأیید ایمیل را انجام دهید.
3. (اختیاری ولی توصیه‌شده) Settings → Password and authentication →
   Two-factor authentication را روشن کنید: این حساب گاوصندوق ویترین شماست.

## ۲) ساخت مخزن
1. بالا-راست علامت **+** → **New repository**
2. Repository name: `netbond`
3. **Public** (ویترین باید دیده شود)
4. تیک «Add a README» را **نزنید** (README خودمان را آپلود می‌کنیم)
5. **Create repository**

## ۳) آپلود کیت
1. در صفحهٔ مخزن خالی، روی لینک **uploading an existing file** کلیک کنید.
2. پوشهٔ `github-kit` (همین کیت Extract‌شده) را باز کنید و **همهٔ محتوا**
   (فایل‌ها + پوشه‌های assets و docs) را با ماوس بکشید و داخل صفحهٔ آپلود
   رها کنید؛ مرورگر ساختار پوشه‌ها را حفظ می‌کند.
3. پایین صفحه commit message: `NetBond 1.6.5 public kit` → **Commit changes**

## ۴) ویترین (About)
ستون راست مخزن، چرخ‌دندهٔ کنار **About**:
- Description: `Multi-uplink internet bonding for Windows - Wi-Fi + Ethernet + hotspot as one fast pipe. No VPS, no cloud.`
- Website: فعلاً خالی؛ از مرحلهٔ ۳ آدرس صفحهٔ فروش را می‌گذاریم.
- Topics (اینتر بزنید): `internet-bonding` `proxy` `windows`
  `network-aggregation` `bandwidth` `speedify-alternative` `tap`
- Save

## ۵) اولین Release (همان‌جا خریدار trial را می‌گیرد)
1. ستون راست → **Releases** → **Draft a new release**
2. **Choose a tag** → تایپ `v1.6.5` → Create new tag
3. Release title: `NetBond 1.6.5 - hardware-locked perpetual licences`
4. متن: کل محتوای `RELEASE-NOTES.md` را کپی/پیست کنید.
5. **Attach binaries**: فایل `netbond-1.6.5-trial48.zip` (از پوشهٔ release
   خودتان؛ نه zip کامل!) را بکشید و رها کنید.
6. **Publish release**

## ۶) پین و انتشار
- صفحهٔ پروفایل → ستونRepositories → ستاره‌دار کردن مخزن و **Pin** تا بالای
  پروفایل بماند.
- لینک مخزن را نگه دارید: از مرحلهٔ ۳ دکمهٔ Buy صفحهٔ فروش و بعدتر
  ProductHunt/Reddit همین لینک را می‌خواهند.

## چک‌لیست پایان مرحلهٔ ۲
- [ ] مخزن public با README دوزبانه + پوستر
- [ ] About پر (توضیح + topics)
- [ ] Release v1.6.5 با zip آزمایشی و SHA-256
- [ ] هیچ فایل خزانه‌ای آپلود نشده (جدول بخش ۰ را دوباره چک کنید)
