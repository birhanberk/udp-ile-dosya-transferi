## Hakkında

* FTP protokolünü UDP üzerinden gerçekleştiren sunucu servisi ve istemcisidir.
* Sunucu 42. portu dinlemektedir.

## Kullanım

1. Sunucu `sunucu.py` ile çalıştırılır.
1. İstemci `istemci.py sunucu_ip_adresi` ile çalıştırılır.

* Sunucudan dosya almak için `get dosya_adi.uzanti` komutu kullanılır.

    Ornek kullanım -> get Manowar-Call_to_Arms_lyrics.txt

* Sunucuya dosya göndermek için `put dosya_adi.uzanti` komutu kullanılır.

    Ornek -> put Judas_Priest-Hell_Patrol.mp3

* Sunucu üzerindenki dosyaları listelemek için `listele` komutu kullanılır.

    Ornek -> listele

## Yapı

* Sunucu çalıştırıldığında kendi dizininde bulunan dosyaları listeler ve verilen portu dinler.
* İstemci çalıştırıldığında sunucu üzerindeki ve istemcinin dizininde olan dosyaları listeler.
* İstemci bu süreçten sonra verdiği komutlara göre transfer işlemlerini gerçekleştirebilir.
* Transfer sırasında bağlantı kopması durumunda paketlerin karşıya ulaşıp ulaşmadığı kontrol edilmektedir. Paketlerin karşı tarafa ulaşmadığı durumda uyarı verilir.
