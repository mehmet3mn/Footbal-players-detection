# ⚽ YOLOv8 ile Futbol Maçı Analizi: Oyuncu, Hakem ve Top Tespiti

Bu proje, **YOLOv8** (You Only Look Once) nesne algılama modelini kullanarak futbol maçlarındaki oyuncuları, hakemleri, kalecileri ve futbol topunu tespit etmek ve takip etmek amacıyla geliştirilmiştir. Model, **Google Colab (T4 GPU)** üzerinde eğitilmiş ve video üzerinde test edilmiştir.

---

## 🚀 Proje Özellikleri

*   **Nesne Algılama (Object Detection):** Sahadaki her bir aktörü (Oyuncu, Hakem, Kaleci) ve topu anlık olarak tespit eder.
*   **Nesne Takibi (Object Tracking):** `ByteTrack` algoritması entegrasyonu sayesinde oyunculara benzersiz ID'ler atayarak hareketlerini video boyunca takip eder.
*   **Google Colab Entegrasyonu:** Eğitim ve çıkarım (inference) süreçleri tamamen bulut üzerinde, GPU hızlandırıcı kullanılarak yapılmıştır.

---

## 📊 Veri Seti (Dataset)

Projede, **Roboflow** üzerinde bulunan "football-players-detection" veri seti kullanılmıştır.
*   **Toplam Görsel Sayısı:** 372 Görsel (Tren: 298, Validasyon: 49, Test: 25)
*   **Sınıflar (Classes):**
    1.  `player` (Oyuncu)
    2.  `referee` (Hakem)
    3.  `goalkeeper` (Kaleci)
    4.  `ball` (Top)

---

## 🛠️ Kurulum ve Gereksinimler

Projeyi yerel bilgisayarınızda veya Google Colab'de çalıştırmak için aşağıdaki kütüphanelerin kurulması gerekir:

```bash
pip install ultralytics roboflow opencv-python


<img width="781" height="436" alt="Ekran görüntüsü 2026-07-16 154820" src="https://github.com/user-attachments/assets/b5e69cd0-48ac-4b5e-8a56-3df82b3ce3b9" />
<img width="775" height="434" alt="Ekran görüntüsü 2026-07-16 155200" src="https://github.com/user-attachments/assets/55b73baa-88c5-45d5-94d6-91f3f91ff608" />
