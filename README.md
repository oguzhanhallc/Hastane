# Hastane

Proje Dokümantasyonu – Proje 2: Hastane Randevu Sistemi

1. Temel Tanım
Bu proje, hastaların uygun doktorlardan randevu almasını ve bu randevuları yönetmesini sağlayan bir sistemdir. Python programlama dili ve tkinter arayüz kütüphanesi kullanılarak geliştirilecektir.
2. Temel Sınıfların Tanımlanması
Hasta Sınıfı: Hasta bilgilerini ve geçmiş randevularını tutar.
- Özellikler: isim (str), tc (str), randevu_gecmisi (list)
Doktor Sınıfı: Doktor bilgilerini ve uygunluk durumunu saklar.

![Ekran görüntüsü 2025-05-19 204037](https://github.com/user-attachments/assets/acc07ae7-ba2a-449a-8d2e-116b347b1f41)

Randevu Sınıfı: Bir hasta ile doktor arasında oluşturulan randevuyu temsil eder.
- Özellikler: tarih (str), doktor (Doktor), hasta (Hasta)
3. Randevu Sistemi Fonksiyonları
randevu_al(hasta, doktor, tarih): Hasta için doktorun uygunluk durumuna göre randevu oluşturur.
randevu_iptal(hasta, randevu): Mevcut bir randevuyu iptal eder ve doktorun müsaitlik listesini günceller.

 ![Ekran görüntüsü 2025-05-19 204113](https://github.com/user-attachments/assets/75d3e7e4-0ea6-47cc-9dc7-385866faf9fa)

- Liste (list): Hasta ve doktor nesnelerini saklamak için.
4. Veri Yapıları
  
- Sözlük (dict): TC ile hasta erişimi sağlamak için.
- JSON: Verilerin dosyada kalıcı olarak saklanması.
- datetime/str: Tarih ve saat bilgileri için.

![Ekran görüntüsü 2025-05-19 204127](https://github.com/user-attachments/assets/0156b611-3a5d-40e8-ac7a-553f0934a036)

![Ekran görüntüsü 2025-05-19 204206](https://github.com/user-attachments/assets/ca8614cc-a59a-40b7-a242-35ab3dd28443)


5. Kullanıcı Arayüzü (GUI)
Araçlar: tkinter, customtkinter
Tema: Mavi tonlar, tıbbi ikonlar (steteskop, iğne)
Ekranlar: Giriş, doktor seçimi, randevu takvimi, randevu iptali
6. Kodlama Aşamaları
1. Sınıfların tanımlanması
2. Fonksiyonların yazılması
3. JSON veri kaydetme/yükleme
4. GUI oluşturulması
5. Kullanıcı girdisi ve işlem mantığı
6. Ana döngünün yönetimi
7. Test Etme
- TC ile hasta girişi
- Aynı saate iki randevu alınamaması
- Randevu alındıktan sonra doktorun uygunluk güncellemesi
- Randevu iptali sonrası zaman diliminin serbest kalması
- JSON veri kaydının test edilmesi
8. Kullanım Kılavuzu
1. Programı başlatın: python main.py
2. TC ile giriş yapın: Yeni hasta otomatik eklenir.
3. Doktor ve tarih seçin, Randevu Al butonuna basın.
4. Randevu geçmişi üzerinden iptal işlemi yapılabilir.


