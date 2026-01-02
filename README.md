# 📊 Model Evaluation Report | Model Değerlendirme Raporu

---

## 🇹🇷 Türkçe

### 🔍 Model Değerlendirme Sonuçları

| Metrik | Değer |
|------|------|
| Test Örnek Sayısı | 30 |
| Doğru Tahmin | 21 |
| Accuracy | 0.7000 |
| Precision | 0.7458 |
| Recall | 0.7000 |
| F1-Score | 0.6583 |

---

## 🔢 Token Kullanımı ve Sorgular

### 🟢 SORGU 1-1: Basit Alan Tespiti
- **Input Token:** 174  
- **Output Token:** 173  
- **Toplam Token:** 347  

**Soru:**  
Bu hukuki karar hangi alana girer?

**Karar Metni (Özet):**  
4. Ceza Dairesi 2021/5312 E., 2023/1 K. – Tehdit, hakaret, kasten yaralama, görevi yaptırmamak için direnme vb. suçlar.

---

### 🟢 SORGU 1-2: Detaylı Analiz
- **Input Token:** 304  
- **Output Token:** 503  
- **Toplam Token:** 807  

**İstenen Başlıklar:**
1. Dava Türü  
2. Ana Konu  
3. Karar Sonucu  
4. İlgili Kanun Maddeleri  
5. Hukuk Dairesi  
6. Dava Dosya No  
7. Mahkemesi  
8. Karar Tarihi  
9. Sanık Sayısı  
10. Sanık Adı Soyadı  
11. Katılan Sayısı  
12. Katılan Adı Soyadı  
13. Temyiz Yoluna Başvuranlar  
14. Temyiz Sebepleri  
15. HAGB Karar Tarihi  

---

### 🟢 SORGU 1-3: Özet Çıkarma
- **Input Token:** 214  
- **Output Token:** 213  
- **Toplam Token:** 427  

**İstek:**  
Kararı maksimum **3 cümle** ile özetleyiniz.

---

### 🟢 SORGU 2-1: Basit Alan Tespiti
- **Input Token:** 169  
- **Output Token:** 268  
- **Toplam Token:** 437  

**Karar Bilgileri:**
- **Daire:** 7. Hukuk Dairesi  
- **Esas No:** 2022/1960  
- **Karar No:** 2023/2  
- **Mahkeme:** Asliye Hukuk Mahkemesi  
- **Dava Türü:** Mülkiyet (%72 Güvenilirlik)

---

### 🟢 SORGU 2-2: Detaylı Analiz
- **Input Token:** 310  
- **Output Token:** 509  
- **Toplam Token:** 819  

**İstenen Başlıklar:**
1. Dava Türü  
2. Ana Konu  
3. Karar Sonucu  
4. İlgili Kanun Maddeleri  
5. Değerlendirme  

---

### 🟢 SORGU 2-3: Özet Çıkarma
- **Input Token:** 217  
- **Output Token:** 366  
- **Toplam Token:** 583  

**Hukuki Dayanak:**
- 5271 sayılı Kanun m.36  
- 6100 sayılı HMK m.369  

---

### 🟢 SORGU 3-1: Basit Alan Tespiti
- **Input Token:** 173  
- **Output Token:** 272  
- **Toplam Token:** 445  

**Konu:**  
Harici satış sözleşmesine dayalı tapu iptali ve tescil.

---

### 🟢 SORGU 3-2: Detaylı Analiz
- **Input Token:** 316  
- **Output Token:** 515  
- **Toplam Token:** 831  

**Ek Başlıklar:**
- İlgili Yargıtay Kararları  
- Analiz (Güvenilirlik %)  
- Özet (Güvenilirlik %)  

---

### 🟢 SORGU 3-3: Özet Çıkarma
- **Input Token:** 212  
- **Output Token:** 361  
- **Toplam Token:** 573  

---

## 📚 Eğitim Token Hesaplaması

| Parametre | Değer |
|---------|------|
| Dataset Kayıt Sayısı | 100 |
| Toplam Karakter | 353,736 |
| Token / Karakter Oranı | 0.25 |
| Epoch Başına Token | 88,434 |
| Epoch Sayısı | 3 |
| Toplam Eğitim Token | 265,302 (~0.27M) |

---

## ✅ Analiz Durumu
**ANALİZ TAMAMLANDI**

---

## 🇬🇧 English

### 🔍 Model Evaluation Results

| Metric | Value |
|------|------|
| Test Samples | 30 |
| Correct Predictions | 21 |
| Accuracy | 0.7000 |
| Precision | 0.7458 |
| Recall | 0.7000 |
| F1-Score | 0.6583 |

---

### 🔢 Token Usage Summary

- **Average Token / Character Ratio:** 0.25  
- **Total Training Tokens:** ~0.27M  
- **Training Method:** LoRA fine-tuning on LLaMA-based model  
- **Domain:** Turkish Legal Decisions (Criminal & Civil Law)

---

### 📌 Conclusion

- Token statistics are **consistent with LLaMA tokenization**
- Performance is **reasonable given dataset size**
- Prompt structure contributes significantly to token usage
- Suitable for **PoC / research-level domain adaptation**

---

