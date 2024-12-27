# Struct
Struct veri yapısı:
birden fazla değişkeni (farklı veri türlerinden bile olabilir) bir araya getirerek tek bir birim olarak gruplamak için kullanılan bir veri yapısıdır. Bu, genellikle bir nesne ya da varlık hakkında birden fazla özellik veya veri tutmak gerektiğinde kullanılır.

Özellikleri
* Bir struct, birden çok veri türünden değişkeni bir arada tutabilir.
* Bu değişkenlere "üye" (member) denir.
* Kullanıcı tanımlı bir veri türüdür.

Yapının Avantajları
* Modülerlik: İlgili verileri bir arada gruplar.
* Okunabilirlik: Kodun daha temiz ve anlamlı olmasını sağlar.
* Esneklik: Bir nesnenin birden çok özelliğini kolayca modelleyebilirsiniz.

Paylaştığım kodun tanımını yapacak olursam eğer şöyle söyleyebilirim;

5 farklı öğrencinin bilgilerini içeren string integer float veri tipindeki değişkenleri tutan bir struct yapımız var bu bilgileri tanımladığımız öğrenci nesneleriyle çağırarak değer atıyoruz , iki öğrenciyi pointer ile tanımladık pointer yapısı kullanma sebebimiz bu öğrencilerin bilgileri için önceden bellekte yer ayırıyoruz ve bu yerleri kullanıyoruz bunu da malloc(sizeof(bilgiler)) kullanarak yapıyoruz , ayrıca pointerin kullanımının bir diğer amacı verilerin tutulduğu yerin adresine sahip olması ve bu adreslere direkt erişebilme imkanı sağlaması. pointer olmayan değerleri atarken öğrenci.yas = x diye değer atarken pointer ile tanımlanan öğrencilerde atamayı ogrenci->yas=x şeklinde verebildik.
Öğrencilerin bilgilerini tanımladıktan sonra bunu ekrana yazdırıyoruz.

Bu örnekte malloc(sizeof()) yapısı kullanarak bellekte önceden yer ayırdık , struct veri yapısı ile farklı tipte değişkenleri tanımladık ve değer atadık , pointer ile bu değerlerin adreslerine de erişim sağlama imkanı elde ettik.
