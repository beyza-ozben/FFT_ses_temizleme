# FFT_ses_temizleme
BİL314-Sinyaller ve Sistemler Dersi/Final Projesi (Fourier Dönüşümü)

"Gürültü Giderme ve Ses Temizleme Sistemi" isimli dönem sonu projesi için isterler şu şekildedir:

1. Ses Kayıtlarının Alınması
2. Gürültü Analizi ve Ayrıştırma
3. Gürültü Giderme ve Ses Temizleme
4. Gerçek Zamanlı Uygulama
5. Raporlama ve Teslim

Proje kapsamında gerekli dökümantasyon hazırlanmış olup bu depoda uygulama aşaması açıklanmıştır. Ses kayıtları kişiye ve projeye özeldir, bu depoya kayıtlar eklenmemiştir. Senaryo (script) adım adım incelenmeli ve mevcut kayıt için gerekli yerler düzenlenmelidir. _SNR değerinin kontrolünü yapınız._ 
*Soundfile kütüphanesi ile entegre çalışmak için ses kayıtları ".WAV" uzantılı olmalıdır!*

# Birinci Adım: Çalışma Ortamının Hazırlanması
```
  $ conda create --name sinyal python=3.10 -y
  $ conda activate sinyal
  $ pip install librosa numpy matplotlib scipy soundfile pyaudio (librosa==0.9.2 numpy==1.23.5 matplotlib==3.7.2 scipy==1.10.1 soundfile==0.13.1 pyaudio==0.2.14)
  $ conda install -c conda-forge libstdcxx-ng
```

Zaman geçtikçe kütüphanelere güncellemeler gelmektedir, bu sebepten kütüphane uyumsuzluklarıyla alakalı hata alınabilir, kontrol edilmesi gerekmektedir.

# İkinci Adım: Senaryonun Koşulması

```
  $ python sesanalizi.py
  $ python sestemizleme.py
  $ python gercekzaman.py
```
Eldeki ses kayıtlarına göre düzenlenen senaryo için tek yapılacak olan bunların sırayla koşulmasıdır. (Sadece ses temizleme isteniyorsa "sestemizleme.py" senaryosunun koşulması yeterlidir.) 
