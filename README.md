 Kursumuz Mikroservis mimarisinde tamamen Api Backendi ile tek Solutionda her sınıf kütüphanesi de bir katman kabul edilirse 24 katmanın (Web UI, Class Library, Api) ayağa kaldırılmasıyla çalışıyor.
Projemizde MSSQL, MongoDB, PostgreSQL, Redis, SQLLite gibi birbirinden farklı 5 veri tabanı var. (Azure Db de eklenecek)
Projemizin Backend kısmı tamamen Api ile yazıldı.
Her bir mikroserviste farklı bir yaklaşımı ele almaya çalıştık. Bir mikroserviste Dapper kullanırken bir diğerinde CQRS Design Pattern'e yer verdik.
Mediator, Unit of Work gibi tasarım desenlerini de uygulamalı olarak kullandık.
Sepet işlemleri için Redis'i, apilerimizi test etmek için Swagger ve Postman'i, bütün veri tabanlarını tek noktadan yönetmek için DBeaver'ı kullandık.
Her şey localimizde kalmasın dedik Docker kullanıp arayüz olarak da Portainer'den yönetim sağladık.
Api dağıtımlarında uzun uzun konfigürasyonlar yapmak zorlaşacak, apileri bizim yerimize başka biri dağıtsın dedik Ocelot kullandık.
Aynı sayfada birden fazla mikroservisi çalıştırdığımız durumlarda farklı dblerden veriler gelmeli dedik, sidebardaki kategorileri MongoDb'den, sağ üstteki sepette yer alan veri sayısını Redis'ten, kullanıcı bilgilerini Identity üzerindeki Docker'dan ayağa kaldırdığımız MSSQL'den, yorumları ise localdeki MSSQL'den çektik.
Admin tarafında mesajlar ve bildirimler anlık görülsün dedik ve SignalR'a yer verdik.
Güvenlik işlemleri için bolca token doğrulaması kullandık.
MultiShop Asp.Net Core MultiShop Mikroservis E-Ticaret Projesi Redis, Docker, MongoDb, PostgreSQL, Onion Arch, CQRS, Ocelot, Postman, Identity Server ve Daha Fazlası Bu Projede!
Projemizde gerçek bir senaryo üzerinde her bir başlığı ayrı bir mikro serviste tutulduğu dolu dolu bir içerikle sizleri bekliyor.
Giriş yapan kullanıcılar için ayrı, misafir kullanıcılar için ayrı, admin için ayrı bir yetkilendirme senaryosuna sahip projemizde tam bir e-ticaret senaryosu uygulandı.
Sıfırdan boş bir Solution altında MultiShop isminde dolu dolu bir proje hazırladık. Bu projede neler yok ki;

Redis

Dapper

Docker

MongoDB

PostgreSQL

MSSQL

SQLLite

RabbitMQ

Caching

Logging

Google Drive Entegreli Fotoğraf Yükleme

Identity Server

Api Gateway

Ocelot Gateway

Postman

Swagger

Onion Architecture

CQRS Design Pattern

Mediator Design Pattern

Repository Design Pattern

AspNet Core Api

Api Consume

Rapid Api

Authentication

Authorization

Json Web Token

JWT Bearer

SignalR

Ajax
