# STM32 Potansiyometre ve OLED Ekran Uygulaması

Bu projede, STM32 Nucleo kartı kullanılarak potansiyometreden okunan analog değer, 0.96 inç OLED ekranda bar grafiği ve yüzde olarak gösterilmektedir. Proje yazılımı STM32CubeIDE ortamında C dili ile geliştirilmiştir.

## Kullanılan Malzemeler
* STM32 Nucleo-C031C6
* 0.96" I2C OLED Ekran 
* 10K Potansiyometre

## Pin Bağlantıları
* **OLED Ekran:** `PA9` (SCL) ve `PA10` (SDA)
* **Potansiyometre:** `PA0` (ADC1_IN0)

## Projenin Çalışma Mantığı
Sistemde, potansiyometreden elde edilen 0-4095 arasındaki 12-bit ADC (analog) değerleri okunur. Ardından bu değerler 0 ile 100 arasında bir yüzdeye matematiksel olarak oranlanır. Hesaplanan sonuç, I2C haberleşme protokolü kullanılarak OLED ekrana anlık olarak hem sayısal veri (yüzde) hem de dinamik bir bar grafiği şeklinde aktarılır.
