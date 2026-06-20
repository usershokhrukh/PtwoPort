# 🚀 PtwoPort — Visual Mock API Generator

**PtwoPort** — dasturchilar uchun backend kodini qoʻlda yozmasdan, vizual tarzda **Mock API** endpointlarini chizish imkonini beruvchi SaaS platformadir. Barcha ma'lumotlar foydalanuvchining shaxsiy kompyuteridagi `db.json` fayliga real vaqtda yozib boriladi!

---

## 🎨 1. Arxitektura (2-Part Architecture)

Brauzer sandbox cheklovlari tufayli lokal fayllarga to'g'ridan-to'g'ri yoza olmaydi. Shu sababli tizim ikki qismdan iborat:
1. **Brauzer UI (SaaS):** Faqat dizayn va visual boshqaruv oynasi.
2. **Lokal CLI Agent (`npx ptwoport`):** Kompyuterda `4000-port`da Mock API serverni ko'taradi va `db.json` faylini boshqaradi. UI bilan **WebSocket (WS)** orqali bog'lanadi.

---

## 🛡️ 2. Xavfsizlik va Maxfiylik

* **100% Maxfiylik:** Ma'lumotlaringiz hech qanday bulutli (Cloud) serverga chiqmaydi, hammasi o'zingizning kompyuterizda (`localhost`) qoladi.
* **Zero Installation:** Kompyuterga og'ir dasturlar o'rnatish shart emas, yadro fonda `npx` orqali vaqtincha ishga tushadi.

---

## 🚀 3. Tezkor Ishga Tushirish

1. **Yadroni yoqing:** Loyiha papkangizda terminalni ochib, buyruqni bering:
   ```bash
   npx ptwoport