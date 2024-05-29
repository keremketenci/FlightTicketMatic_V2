# FlightTicketMatic_V2

# Uçuş Biletmatik Uygulaması_V2

Bu, C# ve Visual Studio kullanılarak geliştirilmiş bir windows form uygulamasıdır. Bu uygulama, kullanıcının bir uçuş için bilet satın almasını sağlar.

## Kullanım

Uygulamayı çalıştırmak için aşağıdaki adımları takip edin:

1. Projeyi Visual Studio'da açın.
2. Program.cs dosyasını bulun ve çalıştırın.

Uygulama başladığında, aşağıdaki adımları takip ederek bilet satın alabilirsiniz:

## Kullanıcı Paneli
1. İlk olarak, kullanıcı olarak kayıt olun veya giriş yapın.
2. Başarılı bir şekilde giriş yaptıktan sonra bilet almak istediğiniz lokasyonları seçiniz.
3. Lokasyonlar Seçildikten sonra seçilen lokasyonlara ait uçuşlar listelenecektir, bir uçuş seçin.
4. Uçuş seçildikten sonra seçilen uçuşa ait uçağın koltukları listelenecektir, satın almak istediğiniz koltuk(ları) seçiniz.
5. Koltuk(lar) seçildikten sonra rezervasyon ekranında seçtiğiniz uçuşa ait bilgiler ve toplam bilet tutarınız listelenecektir, onayla tuşuna basıp bilet alma işlemini gerçekleştirebilirsiniz.

## Admin Paneli
1. İlk olarak, admin olarak giriş yapın.
2. Başarılı bir şekilde giriş yaptıktan sonra Uçak ekleme veya uçuş ekleme paneline girin.
3. Karşınıza çıkacak formda gerekli bilgileri doldurun.
4. Onayla tuşuna basarak data ekleme işlemini gerçekleştirin.

## Sınıflar

Bu proje aşağıdaki sınıflardan oluşmaktadır:

- Program.cs: Ana uygulama dosyasıdır ve kullanıcıyla etkileşim sağlar.
- User.cs: Kullanıcıları temsil eden sınıfı içerir.
- Admin.cs: Yöneticileri temsil eden sınıfı içerir.
- Flight.cs: Uçuşları temsil eden sınıfı içerir.
- Plane.cs: Uçakları temsil eden sınıfı içerir.
- Reservation.cs: Bilet rezervasyonlarını temsil eden sınıfı içerir.

## Önemli Notlar

- Bu uygulama sadece temsili bir amaç taşımaktadır ve gerçek bir bilet rezervasyon sistemi olarak kullanılamaz.
- Uygulama SQLite veritabanını kullanarak rezervasyonları "Data" klasörünün içindeki "FlightTicketMaticDb.db" dosyasına kaydeder.
- Kredi kartı giriş ekranı tamamen göstermeliktir girdiğiniz veriler hiçbir şekilde işlenmez veya kaydedilmez, herhangi bir kart bilgisi girmedende işleminize devam edebilirsiniz.
- Hatalı girişlerde uygulama çökmez, bunun yerine hata mesajı gösterir ve kullanıcıyı tekrar giriş yapmaya yönlendirir.
- Kullanıcı istediği zaman geri dönüp farklı bir seçim yapabilir ve bilet işlemlerini yeniden başlatabilir.
- Bu değişiklikler, kullanıcı deneyimini iyileştirmek ve hata yönetimini güçlendirmek için yapılmıştır.

## Uygulama içi ekran görüntüleri

### Giriş Paneli: 
![Login](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/69208746-4983-419e-808b-b415c2b8d663)

### KayıtOl Paneli: 
![Register](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/9a55848f-deee-4947-9d95-0746b70220ff)

### KullanıcıAnaEkran Paneli: 
![UserHome](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/fb96f86e-5209-4714-85dc-aa74b5563479)

### Lokasyon Paneli: 
![Location](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/c6ed6a07-db69-4501-aff3-bc69c57a4b19)

### Koltuk Paneli: 
![Seat](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/4ec71564-8220-45fe-99a8-7b6291d2111c)

### Reservasyon Paneli: 
![Reservation](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/3fd45fa7-e2b0-45d2-96b4-f51c5807fefd)

### AdminGiriş Paneli: 
![AdminLogin](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/865a1321-37b8-4665-a10e-99dc2c97d3eb)

### AdminAnaEkran Paneli: 
![AdminHome](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/466edd16-be17-4c25-8043-97ba7abc3f17)

### AdminUçak Paneli: 
![AdminPlane](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/ccef1bb2-d14e-40d4-830d-ac943d69154b)

### AdminUçuş Paneli: 
![AdminFlight](https://github.com/keremketenci0/FlightTicketMatic_V2/assets/128905838/c4b0cabf-3c04-411e-abce-080fecfff100)

## Not: Dosyalardaki engel hatası

Bu projeyi indirdikten sonra, eğer böyle bir hata alıyorsanız 

"Severity	Code	Description	Project	File	Line	Suppression State
Error		Couldn't process file FlightTicketMatic.resx due to its being in the Internet or Restricted zone or having the mark of the web on the file. Remove the mark of the web if you want to process these files.	FlightTicketMatic_V2"

Dosya gezgini üzerinden ilgili dosyanın üzerine sağ tıklayıp özellikler seçeneğinden "unblock" seçeneğini aktif edip "tamam"a basıp kaydedin.

### Yardımcı olabilecek kaynaklar
https://stackoverflow.com/questions/51348919/couldnt-process-file-resx-due-to-its-being-in-the-internet-or-restricted-zone-o

![image](https://github.com/keremketenci0/TicketMatic_V2/assets/128905838/705fd411-41e5-415f-8639-50a628a0a643)
