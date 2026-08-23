# Content Ingestion — Sprint 0



## Amaç

Bu branch, resmî SPL çalışma notlarının kaynağını, sürümünü ve müfredat bağlantısını kaybetmeden sisteme alınması için veri sözleşmesini kurar. Öğrenci yüzünde yalnızca doğrulanmış kaynaklarla bağlı içerik görünecektir.



## Kaynak kaydı

Her belge kaydı aşağıdaki alanları taşımalıdır:



- `sourceId`: benzersiz kayıt kimliği
- 
- `title`: resmî belge adı
- 
- `licenseCode`: ilgili lisans
- 
- `moduleId`: hedef modül
- 
- `versionDate`: belge sürüm veya yayın tarihi
- 
- `pageStart` / `pageEnd`: kaynak sayfa aralığı
- 
- `verificationStatus`: `draft`, `verified`, `archived`
- 
- `reviewedBy` ve `reviewedAt`: kontrol kaydı
- 


## Durum geçişi

`draft → verified → archived`



`draft` kaynaklar yönetim ekranında görülebilir ancak ders, soru veya deneme içeriğine dönüşmez. `verified` durumundaki kayıtlar müfredat konusuna bağlanabilir. `archived` kayıtlar yeni içerik üretiminde kullanılmaz fakat geçmiş referanslar korunur.



## İlk teslim

1. Kaynak kayıt türleri ve doğrulama kuralları oluşturulacak.
2. 
2. Modül-konu-kaynak eşlemesi eklenecek.
3. 
3. Kaynak kaydı olmadan öğrenci içeriği açılmayacak.
4. 
4. Kaynak değişikliğinde işlem geçmişi tutulacak.
5. 


## Kabul kriteri

Bir ders veya soru, en az bir `verified` kaynak kaydı ve sayfa aralığı olmadan öğrenci yüzünde yayınlanamaz.











