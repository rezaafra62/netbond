# NetBond 1.6.5 — hardware-locked perpetual licences

**Asset to attach to this release:** `netbond-1.6.5-trial48.zip`
(full-featured 48-hour trial; the commercial full edition is sold separately)

SHA-256: `daaa73c9d246cfa368658c873e84d70f8e274dde8e355a761ba8905b5e77d919`

## Highlights

- **Per-machine perpetual licences, fully offline.** A key is an Ed25519
  signature over the machine's hardware marks (firmware UUID, CPU id,
  system-disk serial, MAC, MachineGuid, hostname). A key leaked in public
  still will not run on another machine; replacing ONE part (e.g. the NIC)
  does not orphan a paying customer.
- **Revocation list:** a key found leaking can be killed in the next release;
  even stored activations are re-checked at startup.
- **The purchase path never closes:** an expired trial still allows
  `fingerprint` and `activate`, and the expiry dialog offers
  "I have a key — activate now".
- **Friendly everywhere:** busy port, missing key file, missing crypto
  package — every case speaks in plain words instead of a traceback.
- **In-app manuals** in Persian, English, Spanish and Arabic (GUI + CLI).
- **Per-app routing:** tick adapters in the Links table, route the aggregate
  into chosen programs; download splitting across links; fail-open policy.
- 1091 automated tests green.

## Upgrade notes

- Trial users: activate your purchased key from the Licence button — no
  reinstall needed; the countdown disappears.
- Sellers: nothing customer-facing changed in the kit workflow.

---

# NetBond 1.6.5 — لایسنس دائمی قفل‌شده به سخت‌افزار

**فایل ضمیمهٔ همین ریلیز:** `netbond-1.6.5-trial48.zip`
(نسخهٔ آزمایشی ۴۸ ساعته با همهٔ قابلیت‌ها؛ نسخهٔ کامل جداگانه فروخته می‌شود)

- کلید دائمی هر ماشین = امضای Ed25519 روی نشان‌های سخت‌افزاری همان ماشین؛
  کلید لو رفته روی ماشین دیگر اجرا نمی‌شود؛ تعویض یک قطعه لایسنس را نمی‌سوزاند.
- فهرست ابطال: کلید لو رفته در انتشار بعد می‌میرد، حتی فعال‌سازی ذخیره‌شده.
- مسیر خرید هرگز بسته نمی‌شود: trial منقضی هم fingerprint و activate را باز
  می‌گذارد و پنجرهٔ انقضا دکمهٔ «کلید دارم» دارد.
- همهٔ خطاها با زبان آدمیزاد: پورت اشغال، فایل کلید نیافتە، پکیج نبود.
- راهنمای داخل برنامه: فارسی، انگلیسی، اسپانیایی، عربی.
- ۱۰۹۱ آزمون سبز.
