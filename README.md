# 👋 Merhaba, ben Berat Taner | Embedded Firmware Developer  

Gerçek sahada kullanılan ürünler için firmware geliştiren bir gömülü yazılım geliştiricisiyim.  
Custom hardware platformlarında çalışan sensör tabanlı sistemler, haberleşme protokolleri ve gerçek zamanlı kontrol uygulamaları geliştiriyorum.  
Sistemlerin test, doğrulama ve performans süreçlerinde aktif rol alıyorum.  

---

# 🚀 Uzmanlık Alanları  

- Firmware Development (C / C++)  
- Gömülü Sistem Geliştirme  
- Sensör Entegrasyonu ve Kalibrasyonu  
- Haberleşme Protokolleri (UART, I2C, SPI, RS485, MQTT, WiFi)  
- Gerçek Zamanlı Kontrol Sistemleri  
- Local Web Arayüz Geliştirme  
- Sistem Test ve Doğrulama    
- Hata Loglama ve Veri Analizi  

---

# 📂 Gömülü Sistem Proje Alanları  

## 🎵 Etkileşimli Sistemler  

Gerçek zamanlı kullanıcı etkileşimi ve ses kontrol sistemleri  

- Darbuka Interactive System (Dubai Music Museum)
  
  MPU6050 ivmeölçer verisini gerçek zamanlı işleyerek FFT tabanlı frekans analizi ile LED ekolayzır ve darbe karakteristiği oluşturduk. Sistem ESP32 tabanlı özel PCB üzerinde düşük gecikmeli ve kararlı biçimde müze ortamında aktif olarak çalışmaktadır.
  
  Teknolojiler: ESP32-WROOM-32U, C/C++, FFT, Real-time Signal Processing, Custom PCB
- Çark Interactive System (Dubai Music Museum)
  
  10 sensör girişini MCP I/O expander üzerinden okuyarak çift diskli mekanizmanın kombinasyonlarını boolean sadeleştirme (Karnaugh) ile deterministik biçimde çözen kontrol algoritması geliştirdim. Seçilen kombinasyon UART üzerinden ses modülüne iletilerek SD tabanlı       dosya sisteminden oynatıldı. Sistem kararlı ve düşük gecikmeli çalışacak şekilde tasarlandı.

  Teknolojiler: ESP32-WROOM-32U, C/C++, MCP I/O Expander, UART, SD File System, Boolean Logic Optimization 
- Sound Effect System (Multi-country deployments)

  6 butonlu custom PCB üzerinden tema seçimi alındı ve RS485 ile 50–55m mesafedeki diğer karta gönderildi. DY-HV20T ses modülü UART üzerinden kontrol edildi, fade-out ve ses genliği bazlı LED senkronizasyonu sağlandı. Sistem sahada düşük gecikmeli, kararlı ve güvenli      çalışacak şekilde tasarlandı.

  Teknolojiler: Custom PCB, C/C++, RS485, UART, Audio Control, LED Synchronization  
- Animal Sound System

  Touch sensörlü çocuk figürleri ile etkileşim sağlanarak her dokunuşta ilgili hayvan sesi anında oynatıldı. Sistem custom PCB üzerinde low-latency ve güvenli şekilde çalışmaktadır.

  Teknolojiler: Custom PCB, C/C++, Touch Sensor, DY-HV20T, Audio Playback, Real-time Event Handling  
- Animal Jaw Movement Controller

  Animatronik ağız hareketlerini müzik ve ses efektleriyle senkronize ettim. Servo PWM kontrolü ve UART tabanlı ses tetikleme ile doğal ağız hareketleri üretildi.

  Teknolojiler: C/C++, Servo PWM Control, UART Audio Triggering, Timing Synchronization, Custom PCB  

---

## 🏭 Endüstriyel Kontrol Sistemleri  

Endüstriyel otomasyon ve kontrol uygulamaları  

- Traffic Lights Control System (Data logging & error tracking)
  
  32x32 SPI LED matrix üzerinde milisaniye hassasiyetli interrupt/task tabanlı ekran yenileme sağladım. Sensör verileriyle akış dinamik yönetildi, tüm veriler hem local web arayüzünden izlenip hem de EEPROM’da kaydedilerek kalıcı olarak saklandı. Parametreler hem manuel   hem local web arayüzünden ayarlanabilir.
  
  Teknolojiler: C/C++, SPI LED Matrix, Interrupt Architecture, EEPROM Persistence, Local Web Interface  
- Smart Scale System (Multi-node loadcell architecture)

  Loadcell verilerini kalibre edip lineerleştirdim. LED görselleştirme eşik bazlı, maksimum kilo ve minimum dara değerleri local web arayüzünden ayarlanabilir. ESP-NOW üzerinden iki cihaz arasında senkron veri aktarımı sağlandı.

  Teknolojiler: Loadcell, Calibration Algorithm, C/C++, ESP-NOW, Addressable LED, EEPROM, Local Web Interface  
- Smart Stadiometer (Ultrasonic measurement system)
  
  Ultrasonik sensör ile boy ölçümü yapıldı, adreslenebilir LED akışıyla aralık bazlı görselleştirme sunuldu. Ölçümler filtrelenerek hassas boy oranı elde edildi ve local web arayüzü üzerinden kalibrasyon ayarları yapılabildi.

  Teknolojiler: C/C++, Ultrasonic Sensor, Addressable LED, Filtering, Calibration, Local Web Interface  
- Wireless Sensor Network (KOSGEB Project)

  ESP-NOW tabanlı iki kartlı kablosuz ağda, sensör enerjisi veri alışverişine bağlı sırayla aktive edildi. Dinamik MAC eşleşme ve EEPROM kalıcılığı ile güç kesintisine dayanıklı yapı kuruldu.

  Teknolojiler: C/C++, ESP-NOW, Dynamic MAC Pairing, Energy-efficient Sensor Control, EEPROM  

---

## 🔥 Simülasyon Sistemleri  

Gerçek dünya senaryolarını simüle eden sistemler  

- Fire Simulation System (Interactive fire suppression scenario)
  
  Linux tabanlı sistemden 64x32 LED panellere yüksek hızlı veri aktarımı sağladım. Görsel ve işitsel efektler ESP32 ile senkronize edildi. Yangın şiddeti local web arayüzünden ayarlanabilir ve sistem lokalden başlatılıp durdurulabilir.

  Teknolojiler: Linux Embedded, ESP32, Serial Communication, LED Matrix Control, Audio Integration, Local Web Interface  
- Kitchen Fire Simulation (Multi-device synchronized system)
  
  6 node’lu dağıtık sistemde ESP-NOW ile senaryo tabanlı state machine mimarisi geliştirdim. Smoke cihazı ready sinyali gelmeden sistem başlatılamaz ve her node local web arayüzünden izlenebilir.

  Teknolojiler: C/C++, ESP-NOW, Distributed State Machine, UART, Local Web Interface  
- Smart Smoke Generator (PID controlled industrial device)

  PID kontrollü sıcaklık cihazı entegrasyonu ile smoke sistemi çalıştırıldı. Sıcaklık alt/üst eşik değerlerinde başlatma devre dışı kalıyor ve sistem ready sinyali gelmeden localden başlatılamıyor. Donanımsal termik sigorta ile güvenli, fail-safe tasarım sağlandı.

  Teknolojiler: C/C++, Custom PCB, PID Control, Safety Interlocks, Local Start Control  

---

## 🎮 Etkileşimli Uygulamalar  

Kullanıcı etkileşimli deneyim projeleri  

- Slime Automation Project

  Tek fazlı asenkron motor ile dolum ve döküm süreci kontrol edildi. Sensör ve LED entegrasyonu ile işlem durumu gösterildi; local web arayüzü üzerinden başlat/durdur işlemi yapılabilir ve emergency stop ile sistem güvenli şekilde durdurulabilir.

  Teknolojiler: C/C++, Custom PCB, Motor Control, Sensor Integration, LED Feedback, Local & Manual Control  
- Seconds Reaction Game

  Tek butonlu tepki oyunu 64x32 LED panel ile milisaniye doğruluğunda sayaç ve alan bazlı ekran güncelleme. Kalıcı hafıza ile veri kaybı önlendi.

  Teknolojiler: C/C++, Custom PCB, LED Matrix, Button Control, Persistent Memory, Real-time Counter  

---

## 🖥️ İzleme ve IoT Sistemleri  

Uzaktan izleme ve veri toplama sistemleri  

- ThingsBoard IoT Monitoring (MQTT based telemetry system)

  85+ cihaz için MQTT tabanlı uzaktan izleme ve parametre yönetim altyapısı geliştirdim. WiFi yoksa AP moduna geçiş, veri buffer’lama ve bağlantı sonrası otomatik veri senkronizasyonu sağlandı. Token bazlı dashboard kontrolü ile merkezi yönetim sağlandı.

  Teknolojiler: C/C++, WiFi, MQTT, EEPROM Buffering, Remote Parameter Management, Dashboard Integration  

---

## 📊 Yardımcı Sistemler  

Günlük kullanım amaçlı yardımcı sistemler  

- Time & Temperature Display (RTC + Temperature sensor system)

  64x32 LED panel üzerinden saat ve sıcaklık bilgisi gösterildi. NTP ve RTC tabanlı hibrit zaman senkronizasyonu ile online/offline modlar desteklendi. Local arayüz üzerinden manuel ayar yapılabilir.

  Teknolojiler: C/C++, Custom PCB, LED Matrix, RTC, EEPROM, NTP Sync, Local Interface  

---

# 🧠 Teknik Yetkinlikler  

- Bare-metal firmware geliştirme  
- Gerçek zamanlı gömülü sistem mimarisi  
- Sensör veri işleme ve filtreleme  
- Haberleşme protokol entegrasyonu  
- Sistem performans optimizasyonu  
- Hata yönetimi ve loglama  
- Endüstriyel kontrol algoritmaları  
- Signal processing tabanlı efekt sistemleri  
- PID kontrol uygulamaları  

---

# 🛠️ Kullandığım Teknolojiler  

C • C++ • PlatformIO • MQTT  
Custom Hardware Platforms • Sensor Systems  
Embedded Communication Protocols  
Local Web Interface Development  

---

# 🌍 Projelerin Kullanıldığı Ülkeler  

Geliştirilmesine katkı sağladığım sistemler aşağıdaki ülkelerde aktif olarak kullanılmaktadır:

Türkiye, Yunanistan, Romanya, Portekiz, Rusya, Ukrayna, Fransa, Hollanda, Birleşik Arap Emirlikleri (Dubai), Mısır ve Amerika Birleşik Devletleri.                

---

# 📫 İletişim  

📧 Mail: berat.taner.indere@gmail.com  
💼 LinkedIn: https://www.linkedin.com/in/berat-taner/  

---

⭐ Bu profil gerçek saha deneyimine dayalı gömülü sistem projelerini içermektedir.
Geliştirilen sistemler gerçek donanım üzerinde test edilmiş ve sahada aktif olarak çalışmaktadır.  
