# FFT_ses_temizleme
BİL314-Sinyaller ve Sistemler Dersi/Final Projesi (Fourier Dönüşümü)

"Gürültü Giderme ve Ses Temizleme Sistemi" isimli dönem sonu projesi için isterler şu şekildedir:

1. Ses Kayıtlarının Alınması
2. Gürültü Analizi ve Ayrıştırma
3. Gürültü Giderme ve Ses Temizleme
4. Gerçek Zamanlı Uygulama
5. Raporlama ve Teslim

Proje kapsamında gerekli dökümantasyon hazırlanmış olup bu depoda uygulama aşaması açıklanmıştır. Ses kayıtları kişiye ve projeye özeldir, bu depoya kayıtlar eklenmemiştir. Senaryo (script) adım adım incelenmeli ve mevcut kayıt için gerekli yerler düzenlenmelidir. _SNR değerinin kontrolünü yapınız._ \\
*Soundfile kütüphanesi ile entegre çalışmak için ses kayıtları ".WAV" uzantılı olmalıdır!*\\

# Birinci Adım: Çalışma Ortamının Hazırlanması
```
  $ conda create --name sinyal python=3.10 -y
  $ conda activate sinyal
  $ pip install librosa numpy matplotlib scipy soundfile (librosa==0.9.2 numpy==1.23.5 matplotlib==3.7.2 scipy==1.10.1 soundfile==0.13.1)
```

Zaman geçtikçe kütüphanelere güncellemeler gelmektedir, bu sebepten kütüphane uyumsuzluklarıyla alakalı hata alınabilir, kontrol edilmesi gerekmektedir.\\

# İkinci Adım: Senaryonun Koşulması

```
  $ python sinyal.py
```
Eldeki ses kayıtlarına göre düzenlenen senaryo için tek yapılacak olan bunun koşulmasıdır. Ardından sırayla iki pencere açılacaktır. Birinci pencerede orijinal sinyalin ve gürültüsü giderilmiş sinyalin zaman alanındaki (time-domain) grafikleri mevcuttur, pencere kapatılınca proje koşulmaya devam eder. İkinci pencerede orijinal sinyal spektrogramı ve gürültü giderilmiş sinyal spektrogramının grafikleri mevcuttur, pencere kapatılınca proje koşulması tamamlanır ve terminal sonlanır. Açılan pencereleri kaydetmeyi unutmayın!

