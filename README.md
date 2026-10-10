#STM32 Potansiyometre ve OLED Ekran Uygulaması

Bu projede STM32 Nucleo kartı kullanarak potansiyometreden okuduğum değeri 0.96 inç OLED ekranda bar grafiği ve yüzde olarak gösterdim. Kodları STM32CubeIDE üzerinden C diliyle yazdım.

# Kullandığım Malzemeler
* STM32 Nucleo-C031C6
* 0.96" I2C OLED Ekran 
* 10K Potansiyometre

#Pin Bağlantılarım
* **OLED Ekran:** `PA9` (SCL) ve `PA10` (SDA)
* **Potansiyometre:** `PA0` (ADC1_IN0)

## Projenin Çalışma Mantığı
Potansiyometreyi çevirdikçe oluşan 0-4095 arasındaki ADC (analog) değerlerini okuyorum. Sonra bu değeri 0 ile 100 arası bir yüzdeye oranlıyorum. Çıkan sonucu da I2C haberleşmesiyle OLED ekranda hem sayı olarak hem de dolup boşalan bir bar grafiği olarak anlık yazdırıyorum.