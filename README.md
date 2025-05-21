Bu proje İnönü Üniversitesi Bilgisayar mühendisliği öğrencileri ile Tıp Fakültesi öğrencilerini, doktorları buluşturmayı temel edinen bir projedir. Proje esasında öğrencilerin yapay zeka entegreli çözümsel modüllerinin sisteme belirli testlere tabii kalarak yüklemesi ve doktorların ve tıp öğrencilerin bu modülleri kullanarak daha kolay bir çalışma ortamına sahip olmalarını hedeflemektedir.

Kullanılan Teknolojiler
Python
Django
Bootstrap
Html - css - JavaScript
PostgreSQL
Celery
RabbitMQ
IIS
Tanıtım
Kategorize edilmiş bir ana sayfa ile kullanıcı kullanmak istediği modüle rahatlıkla ulaşabilmektedir. image

Sisteme giriş yapan öğrencilerin modüllerini görebileceği, düzenleyebileceği, silebileceği bir projelerim sayfası. image

Öğrencilerin ekleyecekleri modüllerin problemsiz çalışması için önceden test ettirilmesini sağlayan bir code test sayfası. Bu sayfaya öğrenciler kodlarını ve yapay zekalarını yüklüyorlar ve eğer problemsiz bir şekilde çalışıyor ise modülleri sisteme yükleniyor aksi halde terminalden düzenlemeleri gerekiyor. image

Öğrenciler eğer iki kişilik bir ekip halince çalışacaklar ise projeye iki kişinin de düzenleyebilmesi için bir ekip oluşturmaları geerekmektedir bunun için de ekip oluşturma sayfası bulunmaktadır. image

Ana sayfadan çalıştırılmak istenen modül seçildikten sonra eğer 3 boyutlu bir çıktı vericekse ona uygun eğer iki boyutlu bir çıktı vericekse ona uygun dosya yüklenir ve işlem sırasına girer burda işlem sırasını celery ile sağladık. image

Gönderilen işlemin başarılı, başarısız ya da daha işlemde olduğunu gösteren bir sonuç sayfamız vardır bu sayfa kullanıcı id sine özeldir ve bir kullanıcının yaptığı işlem sadece onda gözükür bunun yanında herkses açık da işlem yapılabilir. image

-Çıkan sonuç 2 farklı şekilde gösterilmektedir ilk gönderilen ham görüntü ve teşhis edilen sonuç. Bunların yanında eğer kullanıcı görsel üzerinde bir işaretleme yapmışsa bu bir json ile aktarılmakta ardından görsele çizilmektedir eğer istersek bunu sayfa üzerinden açıp kapatabiliriz. image image

Genel işlemlerin kontrolü, sisteme kayıt olacak öğrencilerin ayarlanması, projelerin kontrolü, derslerin seçilmesi ve değiştirilmesi, kategorilerin eklenmesi silinmesi ya da sıralanması gibi işlemler için bir admin paneli bulunmakta işlemlerin kısayla özetlemek gerekirse.
Öğrenci Listeleme: Sisteme kaydolacak öğrencilerin listesi bir excel tablosu ile yüklenir ve bu öğrenciler aldıkları derse göre kategori edilir ve sadece bu dersler için modül yükleyebilirler ya da sadece modül çalıştırabilirler. Aynı zamanda sonradan öğrenci ekleme ve silme işlemleri yapılabilmektedir
Projeler: Projelerin listelenebileceğii düzenlenebileceği, silinebileceği bir sayfadır aynı zamanda aktif-pasif yapılabilmektedir pasif durumda bulunan bir modül ana sayfada gözükmemektedir.
Ders işlmeleri: Dersleri ekleme, silme, düzenleme işlemlerinin yapıldığı sayfadır.
Kategori işlemleri: Modül kategorilerinin eklenme, silme, değiştirme işlemlerinin yapıldığı sayfadır aynı zamanda sıralarının da ayarlandığı bir kategori sayfasıdır. image
Genel
Proje aktif şekilde kullanılmaktadır ve uzun yıllar kullanılmaya devam edecektir. Dönemsel projelerin yapılması ve yönetilmesi açısından kolaylıklar sağlamaktadır. 3 ay gibi bir süreçte yapılan bu proje aynı zamanda benim bitirme projemdir. Kullanıcı deneyimlerine göre geliştirme yaptığım bu süreçte tamamen kullanıcı kolaylığına odaklandım ve buna göre eklemeler çıkarmalar yaptım, özelleştirmeleri tamamen kullanıcının rahat edebileceği şekilde yaptım.
