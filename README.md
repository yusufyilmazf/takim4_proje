# Fabrika Parça Üretim Takibi


Fabrikamızda hammadde stokları takip edilerek mobilya üretimi yapılacaktır.Fabrikamızda üretebileceğimiz mobilya türleri en az 6 adet olacak şekilde önceden tanımlanacaktır. Fabrikamızda mobilya üretimi için en az 3 adet hammadde kullanılacaktır. Fabrika kapasitemize göre personel çalıştırılacak ve personellere dayalı olarak saatlik üretimler yapılacaktır.Hammadde stoklarımız saatlik olarak takip edilecek ( bu sistem için 1 sn) gerektiğinde hammadde tedariği yapılacaktır ve gün sonunda günlük olarak üretilen mobilyaların miktarları kullanıcıya raporlanacaktır. 

## Yapılacaklar

- Var sayılan olarak en az 6 adet Mobilya sisteme yazılım aşamasında tanımlanacak
- Yazılım başladığında kullanıcıya her mobilyanın tüm özellikleri tek tek rapor edilecek
- Kullanıcı isterse konsoldan (ftm.Scan...) gireceği komutlarla çalışma anında default mobilyaların bilgilerini düzenleyebilecektir.
- Kullanıcı isterse konsoldan kendi fabrikasının boyutlarını tanımlayabilecektir.
- Kullanıcı başlat komutu verdiğinde fabrikada üretim işlemleri yapılacak ve saatlik (her saat sistem için 1 saniye olabilir) üretimlere göre stok takibi yapılıp gerektiğinde tedarik sürecine gidilecektir ve sonuçları adım adım ekranda yazılacaktır.
- Günlük olarak 24 saate bir ( 24 sn) toplam üretilen edilen mobilyaların miktarları kullanıcıya iletilecektir.

## Çalışma Prensibi

- Fabrikada günlük olarak Random siparişler alınacak. Alınan siparişin tahmini bitişi hesap edilecek. Bir sonraki sipariş bitişten sonra alınacak.
- Stoklar sürekli takip edilerek siparişler üretilelcek burada iş gücüne göre üretim yapılacak.
- Günlük üretim raporları ve sipariş durumları kullanıcıya rapor edilecek


## Notlar

- Mobilya tanımlamalarında Struct kullanılacak.
- Mobilyaların özellerikleri tanımlanırken "methotlar" kullanılacak (foknsiyonlar değil).
- Mobilyalar in-memory map olarak hafızada tutlacak ( map kullanılacak ).
- Log akışları sırasında time.Sleep ile log akışı yavaşlatılırsa daha gerçekci olacaktır.
- Yazılım ilk başladığında nasıl çalıştığını kullanıcın neler yapabileceğini anlatan bir çıktıyı ekranda göstermelidir.
