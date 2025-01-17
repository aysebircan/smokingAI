#projenin adı:
smokingAI

#proje hakkında:
Bu proje sigarayı bıraktırmaya yardım amaçlı tasarlanmıştır. Kullanıcıların sigara içen ve içmeyen kişiler arasındaki farkı görerek neden sigarayı bırakmaları gerektiğini görebilirler.

#özellikler:
- Uyku seviyeleri, kalp atış hızı ve solunum hızı verilerini birleştirme ve zaman bazlı analiz.
- Sigara içenler ve içmeyenler için sağlık metriklerinin ortalamalarını hesaplama.
- Uyku seviyelerinin, kalp atış hızının ve solunum hızının zamana göre değişimini görselleştirme.

#gereksinimler:
Bu projeyi çalıştırmak için aşağıdaki Python kütüphaneleri gereklidir:
- `matplotlib`
- `pandas`

Kurulum için aşağıdaki komutu kullanabilirsiniz:
```bash
pip install matplotlib pandas
```

#kullanım:
1. Kod dosyasını bir Python ortamında çalıştırın.
2. Analiz sonuçları konsola yazdırılacaktır.
3. Uyku seviyeleri, kalp atış hızı ve solunum hızına dair grafikler görüntülenecektir.

#kod açıklamaları:
#verilerin hazırlanması:
- **`sleep_data`**, **`heart_rate_data`** ve **`breathing_rate_data`**: Uyku, kalp atış hızı ve solunum verilerini içeren veri setleri.
- **`create_dataframe` fonksiyonu**: Verileri Pandas DataFrame formatına dönüştürür.
- **`pd.merge_asof`**: Farklı veri kaynaklarını zaman etiketlerine göre birleştirir.

#analiz:
**`analyze_smoking_impact` fonksiyonu:**
- Sigara içenler ve içmeyenler için:
  - Ortalama kalp atış hızını hesaplar.
  - Ortalama solunum hızını hesaplar.
  - Toplam uyku süresini hesaplar.
- Sonuçları konsola yazdırır.

#görselleştirme:
**`plot_sleep_heart_rate_breathing` fonksiyonu:**
- Üç farklı grafikte:
  1. Uyku seviyelerinin zamanla dağılımı.
  2. Kalp atış hızının zamanla değişimi.
  3. Solunum hızının zamanla değişimi.
- Görselleri matplotlib ile oluşturur.

#örnek çıktılar:
#konsol çıktısı:
- Sigara içenler ve içmeyenler için ortalama sağlık metrikleri ve toplam uyku süresi.

#grafikler:
1. Uyku seviyelerinin süreleri.
2. Kalp atış hızının zamana göre değişimi.
3. Solunum hızının zamana göre değişimi.

#lisans:
Bu proje açık kaynaklıdır. İstediğiniz gibi kullanabilir, geliştirebilir ve paylaşabilirsiniz.

#not:
Kodu Google colab üzerinden yazdım. Chatgpt,kütüphaneler,yazılım bilgisi olan arkadaşlarımdan ve colab in yapay zekasından yardım aldım.Kodda kullandığım sağlık verilerini de dev.fitbit.com adresinden belirli bir tarih arasıyla olanlardan aldım.Kodu kopyalayıp google colabden yazdırır iseniz hata vermeden rahatlıkla projeme ulaşabilirsiniz.
