# Not Alma Uygulaması :  App Architecture (MVVM)

Bu proje, Android Architecture Components kullanılarak geliştirilmiş bir not alma uygulamasını içermektedir. Projenin geliştirme sürecini ve kullanılan teknolojileri aşağıda bulabilirsiniz.

## Geliştirme Süreci

Projenin ilk bölümünde, Andorid App Components (Room, ViewModel, LiveData ve LifeCycle) ne olduğunu, nasıl çalıştığını ve neden ihtiyaç duyulduğunu öğrendik. Activity ve Fragment , lifecycle, ViewModel ve LiveData'nın nasıl kullanılabileceğini keşfettik.

ViewModel'lar, UI ile ilgili verileri depolayıp yöneterek yapılandırma değişikliklerini sağlıklı bir şekilde atlatmamıza yardımcı oldu. LiveData ise gözlemlenebilir bir veri taşıyıcısı olarak, yaşam döngüsü farkındalığına sahip olarak UI denetleyicilerini doğru zamanlarda otomatik olarak güncellemeye başladı ve durdurdu.

Uygulamamızın arka tarafında "Room Persistence Library"ni kullandık. Bu kütüphane, SQLite'nin etrafında bir sargı görevi görerek ve Annotations'ları kullanarak tekrarlayan kodu azaltarak veritabanı işlemlerini kolaylaştırdı. Room'un sağladığı derleme zamanı doğrulaması sayesinde, SQL ifadeleri için yazım hatalarından kaynaklanan çalışma zamanı istisnalarını en aza indirebildik. Ayrıca, ViewModel ile veri modeli arasında soyutlama katmanı olarak çalışan bir "Repository" sınıfı ekledik.

Bu yapı ile, single responsibility ve separation of concerns prensiplerine dayanan bir "MVVM" (Model-Görünüm-ViewModel) mimarisi oluşturduk.

## Kullanılan Teknolojiler

Proje, Java programlama dilinde geliştirildi ve aşağıdaki teknoloji ve kütüphanelerini içeriyor:

- Android Architecture Components (Room, ViewModel, LiveData, Lifecycle)
- RecyclerView
- SQLite veritabanı

Kaynak : https://www.youtube.com/watch?v=ARpn-1FPNE4&list=PLrnPJCHvNZuDihTpkRs6SpZhqgBqPU118&index=2&ab_channel=CodinginFlow


https://github.com/kadersuutlu/Android-Architecture-Components/assets/80063396/8ca87f12-d510-4233-a8a1-4286d0e2b91f

