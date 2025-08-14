# AFFiNE Self-Host Template

Bu şablon, [AFFiNE](https://affine.pro)’i tek tıkla **Railway.app** üzerinde dağıtmak için tasarlanmıştır. Kalıcı olmasa da, test ve kişisel kullanım için idealdir.

## 🚀 Tek Tıkla Deploy

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/deploy/hC8QHa?referralCode=R1DuZA)

> ⚠️ Not: Railway ücretsiz planında veri kalıcılığı sınırlıdır. Üretim (production) kullanımı için harici PostgreSQL önerilir.

---

## 🛠️ Yapılandırma

Deploy sonrası, aşağıdaki ortam değişkenlerini Railway "Variables" sekmesinden düzenleyebilirsin:

| Değişken | Açıklama | Varsayılan |
|--------|--------|----------|
| `POSTGRES_PASSWORD` | PostgreSQL şifresi | Otomatik üretilir |
| `NODE_ENV` | Ortam tipi | `production` |
| `AFFINE_PUB_WORKER_COUNT` | Yayın işçi sayısı | `1` |

---

## 🌐 Erişim

Deploy bittikten sonra, Railway otomatik bir URL atar (örneğin `https://sizin-affine.up.railway.app`). Tarayıcıdan açarak AFFiNE’e erişin.

---

## 🔄 Güncelleme

Yeni bir AFFiNE versiyonu çıkmışsa:
1. Railway'de projeyi durdur.
2. `Image` sekmesine git → `toeverything/affine-pro:latest` imajını yeniden çek.
3. Yeniden başlat.

---

## 💡 İpucu: Kalıcı Veri İçin

Eğer verilerin kalıcı olsun istiyorsan:
- Harici bir PostgreSQL (örneğin [Neon.tech](https://neon.tech)) kullan.
- `DATABASE_URL`’i buna göre değiştir.

---

## 📂 Kaynak

Resmi dökümantasyon: [https://docs.affine.pro](https://docs.affine.pro)
