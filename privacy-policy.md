Son yenilənmə tarixi: 22 oktyabr 2025-ci il.

Bu Məxfilik Siyasəti Naxçıvan regionu üçün nəzərdə tutulmuş NaxTap mobil tətbiqinin istifadəçilərinin məlumatlarının hansı qaydada toplanması, saxlanılması, işlənməsi və qorunması barədə məlumat verir. Tətbiqdən istifadə etməklə bu siyasətin şərtlərini qəbul etmiş olursunuz.


---

1. NaxTap Haqqında

NaxTap — istifadəçilərə elan yerləşdirmək, məhsul axtarmaq, satıcılarla əlaqə yaratmaq, qiymət təklifləri vermək və real məhsullar üzrə alış–satış prosesində əlaqələndirmə rolunu həyata keçirmək imkanı verən mobil marketplace platformasıdır.

NaxTap:

Ödəniş qəbul etmir

Daxili alış-veriş sistemi yoxdur

Digital məhsul və ya abunəlik satmır

Ödənişlər yalnız tərəflər arasında tətbiqdən kənarda həyata keçirilir


Tətbiq Supabase infrastrukturundan istifadə edir:

Məlumat bazası (PostgreSQL)

Media yaddaşı

Real-time sistemləri

Təsdiqləmə (authentication)

Bildiriş göndərmə infrastrukturu



---

2. Toplanan Məlumatlar

NaxTap yalnız tətbiqin normal işləməsi üçün lazım olan minimal məlumatları toplayır.

2.1. Hesab məlumatları

Ad və Soyad

Telefon nömrəsi

E-poçt ünvanı

Profil şəkli (istifadəçi tərəfindən yüklənilmiş)


2.2. İstifadəçi tərəfindən əlavə edilən kontent

Məhsul şəkilləri

Məhsul məlumatları (başlıq, təsvir, qiymət və s.)

Mesajlar və qiymət təklifləri
Bu məlumatlar yalnız istifadəçi tərəfindən manuel şəkildə əlavə olunduqda tətbiqə ötürülür.


2.3. Texniki məlumatlar

Cihaz modeli

Əməliyyat sistemi versiyası

Tətbiqin versiyası

IP ünvanı (Supabase tərəfindən avtomatik qeydə alınır)


2.4. Bildiriş tokeni

Push bildirişləri üçün cihazınızdan FCM device token yaradılır. Bu token yalnız bildiriş göndərmək üçün istifadə edilir.


---

3. İcazələr (Permissions)

3.1. Media icazəsi – READ_MEDIA_IMAGES

Bu icazə yalnız aşağıdakı hallarda istifadə olunur:

Elan yerləşdirərkən məhsul şəkli seçmək

Profil şəkli yükləmək


Tətbiq cihazdakı digər şəkilləri:

Oxumur

Skam etmir

Toplamır

Gizli məlumat əldə etmir


İstifadəçi yalnız seçdiyi şəkilləri tətbiqə yükləyir.

3.2. Bildiriş icazəsi – POST_NOTIFICATIONS

Bu icazə:

Yeni təklif

Mesaja cavab

Elana baxış

Sistem mesajları
üçün istifadə olunur.


Bildiriş icazəsi verilmədikdə tətbiq normal fəaliyyətini davam etdirir.


---

4. Məlumatların Necə İstifadə Edilməsi

Toplanan məlumatlar yalnız aşağıdakı məqsədlər üçün istifadə olunur:

Hesabın yaradılması və idarə edilməsi

Elanların paylaşılması və saxlanılması

Mesajlaşma və qiymət təklifi funksiyasının işləməsi

Satıcı və alıcı arasında əlaqələndirmə

Tətbiqin təhlükəsizliyinin təmin olunması

Texniki problemlərin aradan qaldırılması

Bildiriş göndərilməsi



---

5. Məlumatların Saxlanması və Təhlükəsizliyi

NaxTap məlumatların təhlükəsiz saxlanması üçün Supabase-in aşağıdakı texnologiyalarından istifadə edir:

Şifrələnmiş server bağlantıları

RLS (Row Level Security) siyasətləri

JWT tokenlərlə giriş nəzarəti

Təhlükəsiz media obyektləri

Avtomatik ehtiyat nüsxələri


NaxTap istifadəçi məlumatlarını 3-cü tərəfə satmır və paylaşmır.


---

6. 3-cü Tərəflər

NaxTap məlumatları yalnız aşağıdakı xidmətlərlə paylaşa bilər:

Supabase

Məlumat bazası saxlanması

Media faylları

Real-time kanal sistemi

Bildiriş infrastrukturu


Firebase Cloud Messaging

Bildiriş tokenlərinin saxlanması

Push bildiriş göndərilməsi


Bu xidmətlər yalnız texniki məqsədlə istifadə olunur.


---

7. Uşaqların Məxfiliyi

NaxTap 13 yaşdan aşağı istifadəçilər üçün nəzərdə tutulmayıb və belə istifadəçilərdən məlumat toplamağı məqsəd qoymur.


---

8. Məlumatların Silinməsi

İstifadəçi hesabını silmək istədikdə:

Profil məlumatları

Elanlar

Mesajlar

Yüklənmiş media faylları
sistemdən tam şəkildə silinir.


Silinmə tələbi üçün istifadəçi “Hesabı Sil” funksiyasından istifadə edə bilər və ya dəstək ilə əlaqə saxlaya bilər.


---

9. Ödənişlər və Maliyyə Məlumatları

NaxTap tətbiq daxilində ödəniş qəbul etmir və ödənişlə bağlı məlumatları toplamaz.

Bütün ödənişlər satıcı və alıcı arasında, tətbiqdən kənarda həyata keçirilir.


---

10. Siyasətə Düzəlişlər

NaxTap bu siyasəti vaxtaşırı yeniləyə bilər. Yenilənmiş versiya bu səhifədə dərc ediləcək.


---

11. Əlaqə

Hər hansı sual və ya məxfiliklə bağlı müraciət üçün bizimlə əlaqə saxlaya bilərsiniz:

📧 [E-poçtunu yaz: naxelan085@gmail.com]

12. Reklam Xidmətləri və Premium Funksiyalar

NaxTap daxilində istifadəçilərə aşağıdakı əlavə xidmətlər təqdim olunur:

Məhsul reklamı (Elanın irəli çəkilməsi, vurğulanması, xüsusi göstərilməsi)

HeroSlider reklamları (əlavə görünürlük üçün ödənişli baner yerləri)

Premium abunəlik (satıcılar üçün əlavə imkanlar, üstünlük və alətlər)


Bu xidmətlərin qiyməti tətbiqdə informativ şəkildə göstərilə bilər, lakin NaxTap tətbiq daxilində ödəniş qəbul etmir və Google Play vasitəsilə hər hansı rəqəmsal alış-veriş həyata keçirmir.

Bütün ödənişlər tətbiqdən kənarda, istifadəçi ilə NaxTap administrasiyası arasında həyata keçirilir. Tətbiq daxilində heç bir ödəniş linki, üçüncü tərəf ödəniş sistemi və ya alıcıdan kart məlumatı tələb edilmir.


Admin bu müraciəti təsdiq etdikdən sonra xidmət aktiv edilir.


Ödəniş prosesinə dair bütün qərarlar və razılaşmalar tətbiqdən kənarda baş tutur. NaxTap ödəniş vasitəçiliyi, bank əməliyyatı və ya rəqəmsal satış funksiyası həyata keçirmir.
