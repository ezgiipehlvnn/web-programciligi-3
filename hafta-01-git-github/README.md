# 1. Hafta: Git ve GitHub
## Araştırma
1. Git Nedir?
Git, Linus Torvalds tarafından 2005 yılında geliştirilmiş, açık kaynaklı ve dağıtık bir versiyon kontrol sistemidir (Distributed Version Control System). Temel amacı, bir yazılım projesinin kaynak kodlarındaki değişiklikleri zaman içinde takip etmek, geçmiş sürümleri saklamak ve birden fazla geliştiricinin aynı proje üzerinde çakışma yaşamadan çalışmasını sağlamaktır. "Dağıtık" olması, projede çalışan her geliştiricinin bilgisayarında deponun tam bir geçmişiyle (yedekli olarak) bulunması anlamına gelir.
2. GitHub Nedir?
GitHub, Git tabanlı projelerin uzak sunucularda depolanmasını, paylaşılmasını ve ortaklaşa geliştirilmesini sağlayan bulut tabanlı bir platformdur (şu anda Microsoft bünyesindedir). Kod barındırmanın yanı sıra hata takibi (issue tracking), proje yönetimi araçları, kod İncelemeleri (code review) ve GitHub Actions gibi otomatikleştirilmiş CI/CD süreçleri sunar.
3. Git ile GitHub Arasındaki Fark Nedir?
Git, bilgisayarınızda yerel olarak çalışan, dosyalarınızdaki değişiklikleri izleyen bir yazılım/araçtır. İnternet bağlantısı olmadan da çalışabilir.

GitHub, Git ile yönettiğiniz projeleri internet üzerinde saklayabildiğiniz, başkalarıyla paylaşabildiğiniz ve ekip çalışması yaptığınız bir web platformudur.

Repository (Repo - Depo): Projenizin tüm dosyalarını, klasörlerini ve bu dosyalara ait geçmiş değişiklik geçmişini (commit geçmişini) barındıran çalışma alanıdır. Yerel (local) veya uzak (remote) olabilir.

Commit: Projenizde yaptığınız değişikliklerin (eklenen, silinen veya düzenlenen kodların) kaleme alındığı, Git geçmişine kaydedilmiş anlık bir fotoğrafıdır. Her commit'in kendine ait benzersiz bir kimliği (hash) ve açıklama mesajı bulunur.

Branch (Dal): Ana projeyi (genellikle main veya master) bozmadan yeni bir özellik geliştirmek veya hata düzeltmek için açılan bağımsız çalışma kollarından biridir.

Merge (Birleştirme): Farklı bir branch üzerinde yapılan çalışmaları (örneğin yeni bir özelliği) ana branch ile birleştirme işlemidir.

Clone (Klonlama): Uzak bir sunucudaki (örneğin GitHub'daki) bir projeyi, tüm geçmişi ve dosyalarıyla birlikte kendi bilgisayarınıza kopyalama işlemidir.

Pull (Çekme): Uzak depodaki (GitHub) güncel kodları ve değişiklikleri, yerel bilgisayarınızdaki projenize aktarıp senkronize etme işlemidir.

Push (Gönderme): Yerel bilgisayarınızda yaptığınız ve commit'lediğiniz değişiklikleri uzak depoya (GitHub'a) yükleme işlemidir.

.gitignore Dosyasının Amacı: Git tarafından takip edilmemesi, versiyon geçmişine eklenmemesi gereken geçici dosyaların (şifre dosyaları, derlenmiş çıktı dosyaları, işletim sistemi önbellekleri vb.) listelendiği özel bir yapılandırma dosyasıdır.

## sektör araştırması
1-)
Proje Adı: Dil Analizi ile Alzheimer Risk Tespiti (Bilişsel Dil Analizi Uygulaması)

GitHub Adresi:https://github.com/noktavirgul/Dil-analizi-ile-alzheimer-risk-tespiti

Kullanılan Programlama Dili: Python (%1) ve Jupyter Notebook(%99)

Kullanılan Framework / Kütüphaneler requirements.txt içinde
streamlit==1.28.0
plotly==5.15.0
transformers==4.33.0
torch==2.0.1
accelerate==0.21.0
pandas==2.0.3
numpy==1.24.3
scikit-learn==1.3.0

 Projenin Amacı: Doğal Dil İşleme (NLP) ve makine öğrenmesi modelleri kullanarak kullanıcıdan alınan metinler üzerinde bilişsel dil analizi yapmak; Alzheimer gibi bilişsel bozuklukların erken belirtileri olabilecek dilsel sapmaları (kelime tekrarı sıklığı, zamir analizleri, anlam belirsizliği vb.) tespit ederek bir ön risk değerlendirmesi sunmaktır.

 Yaklaşık Commit Sayısı: 24 commit

 Contributor (Katkı Veren) Sayısı: 2 geliştirici 

 Klasör Yapısı:	
veri seti csv

LICENSE

README.md

alzheimer_zamir_bert.ipynb

anlam_belirsizligi.ipynb

arayuz.py

atom.logo.jpeg

baglac_hatalari.ipynb

baglac_hatasi.ipynb

cumle_uzunlugu_model.ipynb

kelime_tekrar_sikligi

kurabiye.hirsizi.jpeg

modal_egitim.ipynb

multimodal.ipynb

requirements.txt

sozcuk_seciminde_tutarsizlik.ipynb

zamir_analysis_3.py

README Yapısı:

Proje başlığı ve genel tanıtım (özet açıklama)

Özellikler (Çok modüllü analiz, risk seviyeleri, görsel destekli soru setleri)

Sistem gereksinimleri ve Python sürüm uyumluluğu

Adım adım kurulum ve çalıştırma rehberi (git clone, venv oluşturma, pip install komutları)

Uygulamanın nasıl ayağa kaldırılacağı (streamlit run arayuz.py)

2-)
Proje Adı: KACHOW - Kamu Sektörü İçin Çoklu Yapay Zeka Ajanı Karar Destek Platformu

GitHub Adresi:https://github.com/chyp3r/KACHOW-Teknofest-2026.git

Kullanılan Programlama Dili: Python, TypeScript

Kullanılan Framework ve Teknolojiler:

Backend: FastAPI, Pydantic, SQLAlchemy, LangGraph / LangChain, Ollama / Evren API

Frontend: React 18, TypeScript, Vite, TanStack Query

Veritabanı & Arama: PostgreSQL (pgvector, Row-Level Security), Qdrant (Hibrit Arama), Redis

Projenin Amacı: Kamu kurumlarındaki karmaşık resmi evrak süreçlerini yapay zekâ desteğiyle otomatik olarak analiz etmek, ilgili mevzuatı bulmak, yanıt taslağı oluşturmak, kaynak doğrulaması yapmak ve doğru kurumsal birime yönlendirmek

Yaklaşık Commit Sayısı: ~815 commit

Contributor (Katkı Veren) Sayısı: Ekip tabanlı geliştirilen kapsamlı bir TEKNOFEST yarışma projesi.

README Yapısı:

Proje rozetleri (Backend tests, Coverage, Lisans)

KACHOW'un tanımı ve mimari şemaları (Mermaid akış diyagramları)

Demo videoları ve arayüz ekran görüntüleri galerisi

Temel yetenekler (Evrak analizi, mevzuat arama, taslak üretimi, insan onayı)

Sistem mimarisi ve teknoloji yığını tabloları

Hızlı başlangıç, Docker / Kubernetes kurulum rehberi ve ortam değişkeni açıklamaları

3-)
Proje Adı: KAIZEN Teknofest 2026 Dil Ajanları Video Analiz ve Karar Sistemi

GitHub Adresi:https://github.com/TulinBabalikKopmaz/KAIZEN_Teknofest26_DilAjanlar-_VideoAnalizKararSistemi.git

Kullanılan Programlama Dili: Python,css,HTML

Kullanılan Framework / Altyapı: Doğal Dil İşleme (NLP), video işleme ve yapay zekâ ajan tabanlı karar destek bileşenleri.

Projenin Amacı: TEKNOFEST 2026 yarışma senaryolarına uygun olarak, video verilerini ve doğal dil girdilerini işleyip analiz eden, bu veriler doğrultusunda akıllı karar mekanizmaları ve raporlar üreten entegre bir yapay zekâ sistemi geliştirmektir.

Yaklaşık Commit Sayısı:46

Contributor (Katkı Veren) Sayısı: Proje sahibi (Tülin Babalık Kopmaz) ve ilgili geliştirici ekibi.

README Yapısı:

Projenin adı ve TEKNOFEST 2026 bağlamını belirten genel tanıtım

Sistemin çalışma mantığı ve bileşenleri hakkında açıklamalar

Kurulum, bağımlılıklar ve çalıştırma adımları
## Uygulama ödevi 


## öğrendiklerim  
klasörün gite nasıl bağlandğını ve git terimlerini öğrendim commit yapma sırasın da oluşabilicek sorunları gördüm ayrıca açık kaynakların nasıl inceleneceğini ve readme tanımını ve anlamını öğrendim. git up da yüklü olan projelerin nasıl inceleneceğini öğrendim .

## kaynaklar 
https://github.com/TulinBabalikKopmaz/KAIZEN_Teknofest26_DilAjanlar-_VideoAnalizKararSistemi
https://github.com/chyp3r/KACHOW-Teknofest-2026.git
https://github.com/noktavirgul/Dil-analizi-ile-alzheimer-risk-tespiti
http://git-scm.com/book/tr/v2/Ba%C5%9Flang%C4%B1%C3%A7-Git-Nedir%3F
https://docs-github-com.translate.goog/en/get-started/start-your-journey/what-is-github?_x_tr_sl=en&_x_tr_tl=tr&_x_tr_hl=tr&_x_tr_pto=tc&_x_tr_hist=true
https://docs-github-com.translate.goog/en/get-started/start-your-journey/what-is-github?_x_tr_sl=en&_x_tr_tl=tr&_x_tr_hl=tr&_x_tr_pto=tc&_x_tr_hist=true