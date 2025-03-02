
1. Geleneksel dosyalama sistemlerinin çalışma şeklini açıklayarak bildiğiniz bir programlama dili yardımıyla txt dosyadan veri okumak ve veri yazmak için bir uygulama geliştiriniz.
Geleneksel dosyalama sistemleri, verileri düz metin dosyalarında veya belirli formatlardaki (CSV, XML vb.) dosyalarda saklayan sistemlerdir. Bu sistemlerde, veriler genellikle manuel olarak düzenlenir ve erişim dosya okuma/yazma işlemleriyle yapılır.

Python Örneği:

# Dosyaya veri yazma
with open("veri.txt", "w") as dosya:
    dosya.write("Ad: Ali, Soyad: Kaya, Yaş: 25\n")
    dosya.write("Ad: Ayşe, Soyad: Yılmaz, Yaş: 22\n")

# Dosyadan veri okuma
with open("veri.txt", "r") as dosya:
    icerik = dosya.read()
    print(icerik)

2. Geleneksel dosyalama sistemleri ile veritabanı yönetim sistemlerinin benzerlik ve farklılıklarını açıklayınız.
Benzerlikler:

İkisi de veri saklamak için kullanılır.
Verilere erişim belirli kurallar çerçevesinde yapılır.
Farklılıklar:

Özellik	Geleneksel Dosyalama	Veritabanı Yönetim Sistemi (VTYS)
Veri Yapısı	Dosya tabanlı, düz metin veya belirli formatlar	Tablo, ilişkisel model
Hız	Büyük veri setlerinde yavaş	Optimize edilmiş, hızlı erişim
Veri Bütünlüğü	Manuel kontrol gerekir	Otomatik bütünlük sağlama
Güvenlik	Dosya bazlı yetkilendirme	Kullanıcı ve roller bazlı erişim
Veri Tekrarı	Aynı verinin farklı dosyalarda tekrar etme ihtimali yüksek	Normalizasyon ile tekrar azaltılır
3. VTYS’nin geleneksel sisteme göre üstün özelliklerini açıklayınız.
Veri bütünlüğü ve tutarlılığı sağlar.
Hızlı veri erişimi sunar.
Yetkilendirme ve güvenlik özellikleri içerir.
İlişkisel veri modelini destekler.
Veri yedekleme ve kurtarma mekanizmaları vardır.

4. Veritabanının görevini açıklayarak kullanıldığı alanlara örnekler veriniz.

Veritabanları, büyük miktarda veriyi organize bir şekilde saklama, yönetme ve erişim sağlama amacıyla kullanılır.

Kullanım Alanları:

E-Ticaret: Ürün ve müşteri bilgileri saklanır.
Bankacılık: Hesap ve işlem kayıtları yönetilir.
Sağlık Sektörü: Hasta kayıtları ve tıbbi bilgiler tutulur.
Okul Yönetim Sistemleri: Öğrenci ve öğretmen bilgileri depolanır.
5. Tablo, satır ve sütun kavramlarını açıklayınız.
Tablo (Table): Verilerin saklandığı, satır ve sütunlardan oluşan yapı.
Satır (Row - Kayıt): Bir tablodaki her bir veri girişidir.
Sütun (Column - Alan): Tablo içinde belirli bir veri türünü saklayan alanlar.
Örnek Tablo:

ID	Ad	Soyad	Yaş
1	Ali	Kaya	25
2	Ayşe	Yılmaz	22
6. Birincil anahtar ve yabancı anahtar kavramlarını ve farklılıklarını açıklayınız.
Birincil Anahtar (Primary Key): Bir tabloda her satırı benzersiz olarak tanımlayan sütundur.
Yabancı Anahtar (Foreign Key): Bir tablodaki sütunun başka bir tablodaki birincil anahtara referans vermesidir.
Farklar:

Birincil anahtar tektir, yabancı anahtar birden fazla olabilir.
Birincil anahtar boş olamaz, yabancı anahtar boş olabilir.

7. Veritabanı kullanıcı türleri nelerdir?
Veritabanı Yöneticisi (DBA - Database Administrator): Veritabanının güvenliğini ve yönetimini sağlar.
Uygulama Geliştiricisi: Veritabanı ile çalışan uygulamaları geliştirir.
Son Kullanıcılar: Veriyi görüntüleyen ve kullanan kişiler.

8. Örnek bir veritabanı için kullanıcıları belirleyerek yetkilendirmelerini şematik olarak gösteriniz.
Örnek Yetkilendirme:

Kullanıcı Türü	Yetkiler
DBA	Tüm yetkilere sahip
Geliştirici	Veri ekleyebilir ve güncelleyebilir
Son Kullanıcı	Sadece veri okuyabilir

9. Veritabanı ile VTYS’nin farkını açıklayınız.

Özellik	Veritabanı	VTYS
Tanım	Verilerin saklandığı yer	Veritabanlarını yönetmek için kullanılan sistem
İşlev	Veri depolama	Veri yönetimi ve erişimi sağlar
Kullanıcılar	Yazılım sistemleri ve insanlar	DBA, geliştiriciler ve kullanıcılar

10. İlişkisel veri modelini açıklayınız.

İlişkisel veri modeli, verileri tablo (relation) yapısında organize eden ve tablolar arasında ilişkiler kuran bir modeldir.

Örnek:

Öğrenciler Tablosu: Öğrenci ID, Ad, Soyad
Dersler Tablosu: Ders ID, Ders Adı
Kayıtlar Tablosu: Öğrenci ID (FK), Ders ID (FK)
Bu yapı sayesinde öğrenci ve ders bilgileri birbirine bağlanır.

11. Bir öğrenci bilgi sistemi için kullanılacak veritabanı, tablolar ve tablolar arasındaki ilişkileri belirleyiniz.
Bir öğrenci bilgi sisteminde şu tablolar olabilir:

Öğrenciler Tablosu

Öğrenci ID (PK)
Ad
Soyad
Doğum Tarihi
Dersler Tablosu

Ders ID (PK)
Ders Adı
Kredisi
Öğrenci-Ders Kayıtları Tablosu

Öğrenci ID (FK) → Öğrenciler Tablosu
Ders ID (FK) → Dersler Tablosu














Ara

Akıl Yürüt

ChatGPT hata yapabilir. Önemli bilgileri kontrol edin.
?
