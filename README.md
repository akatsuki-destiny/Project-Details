# Project-Details

## Konu: E-Ticaret Projesi 

- Bu proje için microservis yapısını kullanacaktır.
- Bütün endpointler Postman ve Swagger UI kullanılacaktır. 
- Proje arayüzü için React kullanılacaktır. 
- Proje arayüzü için Html5, Css3, Js, React, jQuery, Tailwind kullanabilirsiniz. 


## Proje Açıklaması 
- Mini Otomotiv Parça E-Ticaret Projesini mini bir E-Ticaret projesidir. Kullanıcıların ve adminin olduğun bir sistemdir. 
- Kullanıcıların sisteme giriş yapabilmesi, kayıt olması için ekranlar bulunmaktadır. 
- Ürünü satın alabilmek için üye olunması şarttır. 
- E-Ticaret projesinde ürün satın alınabilinir. 
- Alınan ürünler fake bir metotla ürün kargolama yapılacaktır. 
- Kullanıcı(User) daha önceden aldığı ürünleri listelemek 
- Kullanıcı(User) bilgileri isterse veri tabanında(Database) üzerinden saklanacaktır. 
- Ürünler alındıkça, veri tabanında ürün tablosunda ürün düsecektir. 
- Dil seçeni olacaktır. (Türkçe ve İngilizce) 
- Kullanıcı birden fazla hatalı girişlerde kilitlenmesi. 
- Admin olarak sisteme ürün ekleyebilecek

## Proje Tanımı 
- Mini Otomotiv Parça E-Ticaret Projesinde, kullanıcı(user) yönetici(admin) olmak üzere 2 tane rol bulunmaktadır. Bu roller arasında Çok tane (Admin) , Çok tane (User) olacak şekildedir. Rol management sistemindeki bu durum N-M (ManyToMany)seklinde yapılacaktır. 
- Kullanıcı(User) daha önceden sistemde kayıtlı degilse öncelikle sisteme kayıt olması (Register) gerekmektedir. 
- Kayıt olduktan sonra sisteme gelen mail adresinden onayladıktan sonra kullanıcı aktiflesecektir. 
- Kullanıcı(user) eticaret sisteminden istediği bir ürünü sepet(Basket) ekleyerek alabilecektir. 
- Ürün satın alındıktan sonra kullanıcının belirlediği email adresine ürünü satın alan kisiye mail gönderilecektir. 
- Anasayfada X üründen kaçtane olduğunu ekranda gösterilecektir. 
- Kullanıcı ürün satın alırken Fake olarak Kredi kartı bilgileri Veritabanında(Database) üzerinde kayıt olsun yada olmasın diye kullanıcıda bilgi verilsin. Eğer kullanıcı Bilgiler saklansın dediginde kullanıcı(User) ile Kredi kartı bilgileri olacak şekilde veri tabanında saklanacaktır. Kullanıcı(1) Kredi Kartı(N) olacak şekilde OneToMany olacak sekilde iliski olacaktır. 
• Kullanıcını istediginde Türkçe veya İngilizce (i18N) butonuna tıklayarak projeyi Türkçe veya İngilizce yapabilecektir. Bunun için Resource Bundle (ValidationMessages.properties ve ValidationMessages_tr.properties) olması gerekmektedir.


## Proje Özellikleri 
- Kullanıcının sisteme hatalı girişleri için veri tabanında Loglama yapılacaktır. 
- Sistemin derlenmesinden, sistemin kapanmasında kadar herşeyi tutulduğu project.log dosyasında kaydedilecektir. 
- Veri tabanında Create(Ekleme), Delete(Silme), Update(Güncelleme) işlemlerinde Transaction kullanılacaktır. 
- Kullanıcı isterse admine mail gönderebilecektir.
- Ana sayfada ürünü almak isteyen kullanıcı için üründe filtreleme yapılabilmesi gerekmektedir. 
- Projede eğer kullanıcı 5 kere sisteme girerken hatalı giriş yaparsa, kullanıcı kilitlenecektir ve bu kiliti ancak Admin kaldırabilecektir. 
- Projenin Dockerize yaparak çalıştırırsanız extra puan alacaksınız. Eğer dockerize yaparsanız bunun adımlarını README.md ```sh ``` arasında step step yazalım lütfen. 
- Yazdığınız projenizi Unit Testlerinide yaparsanız extra puan alacaksınız. 
- Yazdığınız projenizde resim eklemeyi ister database gömebilirsiniz isterseniz database sadece url olacak ve bir dizinde saklayabilirsiniz.  
- @Repository join işlemlerinde kendi @Query yazmalısınız.

## Kriterler
- OOP kurallarına göre yazmak önemlidir. ?
- Data Structure(Veri Yapıları) Collection uygulamak çok önemlidir.  
- Commitleri atarken, çalışmayan hiçbir kodu commitlemeyelim. 
- Frontend için kullanılacak teknolojiler (en popülerlerini kullanalım.), HTML5, CSS3, JavaScript, Jquery, Bootstrap, Tailwind , React, Responsive design (Media Query) bu teknoloji kullanabilirsiniz. 
- Projeyi oluştururken her bir sayfanın responsive design uygun olacak şekilde tasarlayalım. Mobil, Table, PC ve Büyük ekranlar olacak şekilde break pointler oluşturabilirsiniz. İster Media Query 
yazarsanız isterseniz CSS Frameworku olan (Bootstrap) veya Tail Wind kullanabilirsiniz. 
- Backend için kullanılacak teknolojiler. GOLANG. 
- POSTMAN kullanalım. Kullanılan verilerin POSTMAN Documenttide projenizde ayrı bir dosyada olsun. 
- API için Swagger Kütüphaneside olması gerekmektedir. 
- Database anasayfada listelemek için cache bellek yöntemini kullanabiliriz. 
- Git için README.md olması gerekmektedir. README.MD lisanı için ingilizce kullanalım. 
- SOLID prensibine göre yazılması gerekmektedir. 
- Design Pattern prensibine göre yazılması gerekmektedir. 
- Clean Code, Yazılım prensiblerine (YAGNI,KISS, Dummy) vs göre yazılması gerekmektedir. 
- Her bir class ilgili paket altında olması gerekiyor örneğin; business>dto>UserDto gibi. 
- Kullanıcı bilgilerinden Şifre(Bcrypted) olacak şekilde olması gerekmektedir. 
- Email benzersiz olmalı.
- (En popülerlerini kullanalım.) React için Componentler arasında props, context veya redux kullanabilirsiniz. 
- React için Kullanıcı bilgileri için context yazılacaktır. Bu componette kullanıcı bilgileri tutulacaktır. 
- Kullanıcı Login olduktan sonra React dependencies için; react-hot-toast kullanabilirsiniz.
- Kullanıcı sisteme giriş yaptığında Javascript için LocalStorage veya SessionStorage verileri saklayabilirsiniz. 
- React için package.json içinde Spring Boot için URL için proxy kullanalım.
