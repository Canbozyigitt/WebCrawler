Sporcu Beslenmesi Üzerine Otomatik Web Tabanlı Veri Toplama ve İçerik Analizi

## Proje Açıklaması

Bu proje, sporcu beslenmesi ile ilgili web tabanlı veri toplama ve bu verilerin otomatik olarak işlenmesini amaçlamaktadır. Selenium ve BeautifulSoup gibi kütüphaneler kullanılarak, Google arama sonuçlarından veri çekilmekte ve bu veriler analiz edilerek veritabanına kaydedilmektedir.

## İçindekiler

- [Kurulum](#kurulum)
- [Kullanım](#kullanım)
- [Dosya Açıklamaları](#dosya-açıklamaları)
- [Katkıda Bulunanlar](#katkıda-bulunanlar)

## Kurulum

1. *Gereksinimler:*

   - Python 3.x
   - Selenium
   - BeautifulSoup4
   - Google Chrome ve ChromeDriver

2. *Gerekli Kütüphanelerin Yüklenmesi:*

   bash
   pip install -r requirements.txt
   

3. *ChromeDriver Kurulumu:*

   - ChromeDriver'ı [buradan](https://chromedriver.chromium.org/downloads) indirip, chromedriver dosyası proje dizinine yerleştirilmiştir.

     

## Kullanım

1. *Kodun Çalıştırılması:*

   Projeyi çalıştırmak için terminalde aşağıdaki komut kullanılmıştır:

   bash
   python crawler.py
   


2. *Veri İşleme ve Kaydetme:*

   - Web sayfasından alınan içerik, tarama.py ve tok.py dosyalarındaki fonksiyonlar ile işlenir.
   - İşlenen veriler, kelime.py ve database.py dosyaları yardımıyla CSV dosyasına ve veritabanına kaydedilir.

## Dosya Açıklamaları

- *crawler.py:* Web tarayıcıyı kontrol eder ve arama sonuçlarından veri çeker.
- *database.py:* İşlenen kelimeleri veritabanına ekler.
- *kelime.py:* İşlenen verileri CSV dosyasına kaydeder.
- *kelimeler.csv:* İşlenen ve kaydedilen verilerin saklandığı CSV dosyası.
- *requirements.txt:* Proje için gerekli Python kütüphanelerini listeler.
- *stopwords.json:* Metin işleme sırasında kullanılmayan kelimelerin listesi.
- *tarama.py:* Web sayfasından alınan HTML içeriğini temizler ve işler.
- *tok.py:* Temizlenen metni kelime köklerine ayırır.

## Katkıda Bulunanlar

- [Ahmet Faruk Çatlar](mailto:ahmetfaruk411@gmail.com)
- [Umutcan Bozyiğit](mailto:umutcanbozyigit34012@gmail.com)
