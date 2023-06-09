(EN)
ERASMUS DATABASE DESIGN

In the first stage of the project, a database was designed to store the data of students who applied for Erasmus. At the beginning of the design the data that should be stored were analyzed. Then, entities and attributes were determined and tables were created by applying normalization steps.

In the project, it was requested that all information of the student be accessed using the account id. For this reason, the 'Account' table is associated with other tables. 'AccountID' in the 'Account' table is added to all tables and marked as foreign key in these tables except the table containing the document types.

According to the design,

One application can be made by one account and one account can make one application. A one-to-one relationship has been established between the application and the account.

One account can be created by one student and one student can create one account. A one-to-one relationship has been established between the student and the account.

One education status can belong to one account, and one account can have many education statuses. A one-to-many relationship has been established between education and accounting. The purpose of storing other educational information is that the education life of the student will be important in the process of determining the students who will participate in Erasmus and this information will be needed in the selection process.

One contact information can belong to one account, and one account can have many contact information. A one-to-many relationship has been established between communication and account.

One account can have one disability status and one disability status belongs to one student. A one-to-one relationship has been established between the disability status and the account.

One account can upload many documents and one document can be uploaded by one student. A one-to-many relationship has been established between the document and the student.

One document has one type and there can be many documents belonging to one type. A one-to-many relationship has been established between the document and the  type of document.


(TR)
ERASMUS DATABASE TASARIMI 

Projenin ilk aşamasında erasmus başvurusunda bulunan öğrencilerin verilerini depolamak amacıyla bir veri tabanı tasarlanmıştır.Tasarımın başlangıcında depolanması gereken veriler analiz edilmiştir. Ardından varlıklar ve özellikler belirlenmiş ve normalizayon adımları uygulanarak tablolar oluşturulmuştur. 

Projede, hesap id kullanılarak öğrencinin tüm bilgilerine erişilebilmesi talep edilmiştir. Bu sebeple 'Account' tablosu diğer tablolarla ilişkilendirilmiştir. 'Account' tablosundaki 'AccountID', döküman tiplerini içeren tablo dışındaki tüm tablolara eklenmiş ve bu tablolarda foreign key olarak işaretlenmiştir. 

Yapılan tasarıma göre,

Bir başvuru bir hesap tarafından yapılabilir ve bir hesap bir başvuru yapabilir. Başvuru ve hesap arasında bire bir ilişki kurulmuştur. 

Bir hesap bir öğrenci tarafından oluşturulabilir ve bir öğrenci bir hesap oluşturabilir. Öğrenci ve hesap arasında bire bir ilişki kurulmuştur

Bir eğitim durumu bir hesaba ait olabilir ve bir hesabın birçok eğitim durumu olabilir. Eğitim ve hesap arasında bire çok ilişki kurulmuştur. Bir hesabın diğer eğitim bilgilerini depolamaktaki amaç erasmusa katılacak öğrencilerin belirlenmesi sürecinde öğrencinin eğitim hayatının önem arz edecek olması ve seçim sürecinde bu bilgilere ihtiyaç duyulacak olmasıdır.

Bir iletişim bilgisi bir hesaba ait olabilir ve bir hesabın birçok iletişim bilgisi olabilir. İletişim ve hesap arasında bire çok ilişki kurulmuştur.

Bir hesabın bir engel durumu olabilir ve bir engel durumu bir öğrenciye aittir.Engel durumu ve hesap arasında bire bir ilişki kurulmuştur. 

Bir hesap birçok döküman yükleyebilir ve bir döküman bir öğrenci tarafından yüklenebilir. Döküman ve öğrenci arasında bire çok ilişki kurulmuştur.

Bir dökümanın bir tipi vardır ve bir tip dökümana ait birçok belge bulunabilir. Döküman ve döküman tipi arasında bire çok ilişki kurulmuştur.
