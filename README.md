STM32 Gömülü Sistem Çalışmaları Arşivi 🚀

Bu depo, STM32 mikrodenetleyicileri ve STM32 HAL kütüphanesi kullanarak geliştirdiğim temel ve orta seviye gömülü sistem uygulamalarını içermektedir. 

Projeler, STM32CubeIDE ortamında C dili ile yazılmış olup temel çevre birimi kullanımlarını anlamak ve donanım kontrolü pratiği yapmak amacıyla numaralandırılmış bir arşiv şeklinde düzenlenmiştir.

 📂 Çalışma Konuları
Bu arşivde yer alan klasörler aşağıdaki temel gömülü sistem konularını kapsar:
* **GPIO (Genel Amaçlı Giriş/Çıkış):** LED sürme, buton okuma, yazılımsal debounce ve zaman gecikmeli algoritmalar (Trafik lambası, karaşimşek vb.).
* **EXTI (Harici Kesmeler):** Donanımsal kesmeler kullanılarak ana döngüden (while) bağımsız, hızlı tepki veren buton ve sensör okumaları.
* **ADC (Analog-Dijital Çevirici):** Sensörlerden ve potansiyometrelerden gelen analog verilerin 12-bit dijital verilere dönüştürülmesi.
* **I2C Haberleşmesi:** Sensör verilerinin OLED ekran gibi modüllerde anlık ve grafiksel (bar grafiği vb.) olarak gösterilmesi.

 🛠️ Kullanılan Araçlar
* **Geliştirme Kartı: STM32 Nucleo seriş (C031C6)
* **Geliştirme Ortamı: STM32CubeIDE 