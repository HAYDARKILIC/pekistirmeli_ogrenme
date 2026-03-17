# Pekiştirmeli Öğrenme

** Haydar Kılıç, Yapay Zeka Mühendisliği** 
---

## 📖 Kaynak Kitap

Bu repodaki Jupyter notebook'lar Pekiştirmeli Öğrenme dersinin teorik içeriğin Python uygulamasını içermektedir.

---

## 📂 İçerik

| Notebook | Konu | Algoritmalar |
|----------|------|--------------|
| [`PO_Ders1_MDP.ipynb`](PO_Ders1_MDP.ipynb) | Markov Karar Süreçleri | Değer İterasyonu, Politika İterasyonu |
| [`PO_Ders2_ValuePrediction.ipynb`](PO_Ders2_ValuePrediction.ipynb) | Değer Tahmin Problemleri | TD(0), Monte Carlo, TD(λ), LSTD |
| [`PO_Ders3_Control.ipynb`](PO_Ders3_Control.ipynb) | Kontrol Algoritmaları | Q-Öğrenme, SARSA, Actor-Critic, REINFORCE, UCB |

---

## 🗂 Notebook Detayları

### 📓 Bölüm 1 — Markov Karar Süreçleri (MDP)
`PO_Ders1_MDP.ipynb`

- MDP tanımı: durum uzayı, eylem uzayı, geçiş çekirdeği, ödül fonksiyonu
- Değer fonksiyonları ve Bellman denklemleri
- **Değer İterasyonu** — Bellman optimallik operatörü T\* ile geometrik yakınsama
- **Politika İterasyonu** — değerlendirme + iyileştirme döngüsü
- 📦 Uygulama 1: GridWorld (4×4 ızgara dünyası)
- 📦 Uygulama 2: Envanter Kontrolü (Örnek 1.1 — Poisson talep modeli, (s,S) politikası)
- 📦 Uygulama 3: Kumar Problemi (Örnek 1.2 — farklı kazanma olasılıkları)

### 📓 Bölüm 2 — Değer Tahmin Problemleri
`PO_Ders2_ValuePrediction.ipynb`

- **Tabular TD(0)** (Algoritma 1) — bootstrapping, farklı α değerleriyle yakınsama analizi
- **Every-Visit Monte Carlo** (Algoritma 2) — geriye doğru getiri hesabı, TD(0) ile karşılaştırma
- **TD(λ)** — uygunluk izleri (eligibility traces), λ ∈ [0,1] taraması
- **Doğrusal Fonksiyon Yaklaşımı** — büyük durum uzaylarında TD(0)
- **LSTD(0)** (Algoritma 7) — least-squares çözümü, tek geçişte yakınsama
- Tüm yöntemlerin RMSE bazlı kapsamlı karşılaştırması

### 📓 Bölüm 3 — Kontrol Algoritmaları
`PO_Ders3_Control.ipynb`

- **Çok Kollu Bandit & UCB1** (Algoritma 5) — keşif-sömürü ikilemi, Thompson Sampling karşılaştırması
- **Q-Öğrenme** (Algoritma 12) — off-policy TD kontrolü, Watkins (1989)
- **SARSA** — on-policy TD kontrolü, Q-öğrenme ile karşılaştırma
- **Actor-Critic**  — softmax politika + TD critic, eligibility trace
- **REINFORCE** — politika gradyanı (Williams 1992), baseline ile/olmadan
- Tüm kontrol algoritmalarının çok-çalışma (multi-run) karşılaştırması

---

## 🚀 Kurulum ve Çalıştırma

### 1. Gereksinimler

```bash
pip install -r requirements.txt
```

### 2. Notebook'ları Başlat

```bash
jupyter notebook
```

Ardından tarayıcıda ilgili `.ipynb` dosyasını açın.

### 3. Önerilen Çalışma Sırası

```
PO_Ders1_MDP.ipynb  →  PO_Ders2_ValuePrediction.ipynb  →  PO_Ders3_Control.ipynb
```

Her notebook bağımsız çalışır; önceki notebook'a bağımlılık yoktur.

---

## ⚙️ Gereksinimler

```
numpy >= 1.24
matplotlib >= 3.7
scipy >= 1.10
jupyter >= 1.0
notebook >= 7.0
```

Python 3.9+ önerilir.

---



