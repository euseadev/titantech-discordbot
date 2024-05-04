# Titantech Minecraft Discord Botu

## Komutlar
- `/ban`: Üye yasaklamaya yarar. (Cooldown: 30 saniye)
- `/kick`: Üyeyi sunucudan atmaya yarar. (Cooldown: 25 saniye)
- `/mute`: Üyeyi susturmaya yarar. (Cooldown: 15 saniye)
- `/sil`: Belirtilen miktarda mesaj silmeye yarar. (Cooldown: 5 saniye)
- `/reset-api-configuration`: API ayarlarını sıfırlar ve yerine yeni ayarları ekler. (Cooldown: 120 saniye)
- `/ticketmesaj`: Destek talebi oluşturma metnini gönderir. (Cooldown: 5 saniye)
- `/vipbilgi`: Seçilen vip üyeliğinin bilgilerini gönderir.

## Komutlar Hakkında Bilgilendirme
### /ban 
- Komut Çalıştırıldığında Gönderilen Mesaj
  
  ![ban](https://cdn.discordapp.com/attachments/1131692946916392962/1236060057377046588/ban.png?ex=6636a222&is=663550a2&hm=c35d9c52930e8a8b4a91e18899344a9101fcf54b77a71c28b7ca83060a6f6e35&)
- Komut Çalıştırıldığında Log Kanalına Gönderilen Mesaj
  ![banlog](https://cdn.discordapp.com/attachments/1131692946916392962/1236060057150427237/banlog.png?ex=6636a222&is=663550a2&hm=27eba017d50484262a084e8fd219c86abd946a478f4a4838da440cd614423d3d&)

### /kick
- Komut Çalıştırıldığında Gönderilen Mesaj
 
  ![kick](https://cdn.discordapp.com/attachments/1131692946916392962/1236061491392811048/image.png?ex=6636a378&is=663551f8&hm=87d44e272fcca30b2ccf79c7b6915ae065a3e99bd15c130d8c9dc1ae9981c984&)
- Komut Çalıştırıldığında Log Kanalına Gönderilen Mesaj
  
  ![kicklog](https://cdn.discordapp.com/attachments/1131692946916392962/1236061522057367633/image.png?ex=6636a37f&is=663551ff&hm=1c567168f5036a8da355d37f0dc1c18c3960e4a04584f804d153e2b5a3b6304d&)

### /mute 
- Komut Kullanımı:

  ![mute](https://cdn.discordapp.com/attachments/1131692946916392962/1236061941185908746/image.png?ex=6636a3e3&is=66355263&hm=ba99fc585eb2890469c7eba1d9aa9e5329eb356daa2a93ab55b27bc277f2e546&)
- Komut Başarıyla Çalıştırıldığında Gönderilen Mesaj
  
  ![mutemessage](https://media.discordapp.net/attachments/1131692946916392962/1236062304219697303/image.png?ex=6636a43a&is=663552ba&hm=7664d8c63a0cbdbcc7d233b52272b4bba272a1213ff8267f22adc5a45e6e0b0a&=&format=webp&quality=lossless)
- Log Kanalına Gönderilen Mesaj
  
  ![mutelog](https://cdn.discordapp.com/attachments/1131692946916392962/1236062304609505481/image.png?ex=6636a43a&is=663552ba&hm=34eb4bc38c6147075d12e95a16a44a11ef33c6585fec8e35d22589819a7ba22a&)
- Ceza Kaldırma
  
  ![unmute](https://cdn.discordapp.com/attachments/1131692946916392962/1236062627441021048/image.png?ex=6636a487&is=66355307&hm=0a84ec2389add97f08123e078d9d29e925e3d8cf7c502b264e44be3207399b78&)

### /sil
- Komut Başarıyla Çalıştırıldığında Gönderilen Mesaj
  
  ![sil](https://cdn.discordapp.com/attachments/1131692946916392962/1236062902268723261/image.png?ex=6636a4c8&is=66355348&hm=4f59d0dae0443b36e50acf8a4431637a37a2f0fc165a51e430285992d9b2f313&)
### /reset-api-configuration
- Komut Aydınlatma Metni:
  Bu pakette yarı otomatik sunucu durum sistemi bulunmaktadır. Diğer Discord botlarındaki gibi hazır API kullanarak sunucu durumunu almak yerine kendisi bir API oluşturarak, sunucu ile bot arasında bağlantı kurmayı sağlar. Örneğin, sunucunuzun bakımda olduğunu hayal edelim. Sunucu bakımda olduğunda diğer API'lerde (örneğin, api.mcsrvstat.us gibi) sunucunuz aktif görünecektir ve bu yüzden sunucunuz bakımda olsa bile, sunucu durum odasında sunucunuzun bakımda olduğu görünmeyecektir. İşte bu sorunu önlemek için böyle bir API sistemi hazırladık. API sistemini şu şekilde kullanabilirsiniz:
  
- Sunucuyu aktif olarak göstermek için: `http://vdsip:apiport/api/v1/serverstatus?status=aktif&auth=api-authorization-key` 
- Sunucuyu bakımda olarak göstermek için: `http://vdsip:apiport/api/v1/serverstatus?status=bakımda&auth=api-authorization-key`

- Komut Başarıyla Çalıştırıldığında Gönderilen Mesaj:
  [Mesaj Buraya Gelecek]
- Sunucu Durumu API Aracılığıyla Değiştirildiği Zaman Gönderilen Loglar
  - Yetkisiz Erişim (Yanlış Şifre):

    ![unauthorized](https://cdn.discordapp.com/attachments/1131692946916392962/1236065811165216858/image.png?ex=6636a77e&is=663555fe&hm=d6fd3472adcffcb0d220d13d52dd35b397ff72d1b7161a35acfba2268cc31927&)
  - Geçersiz İstek (Status Kısmı Aktif ya da Bakımda Değilse)

    ![invalidrequest](https://cdn.discordapp.com/attachments/1131692946916392962/1236067649574928504/image.png?ex=6636a934&is=663557b4&hm=b99842e1fa416e4a7b2b7b87ae06a67acf7e3f04c9c4d39082fb3b6930231916&)
  - Her Şey Sorunsuzsa
    ![success](https://cdn.discordapp.com/attachments/1131692946916392962/1236068045668225124/image.png?ex=6636a993&is=66355813&hm=1cb99c36370e72dba2f2837453c0ddaf7d43ba52c022fb7e0480ff1120afb3e0&)
    ![success2](https://cdn.discordapp.com/attachments/1131692946916392962/1236068153008591019/image.png?ex=6636a9ac&is=6635582c&hm=8f9c2af27c322d4e22730b22d6ec192d6ecd9ee996781c3c1708f38868807d53&)

### /ticketmesaj
- Komut Başarıyla Çalıştırıldığında Gönderilen Mesaj

  ![ticketmessage](https://cdn.discordapp.com/attachments/1131692946916392962/1236069029953671198/image.png?ex=6636aa7d&is=663558fd&hm=dbbc4e5c4b7524bcf6fe2f68f9cd616b3daeec4ac725fbe08e3f09052fc730b6&)

### /vipbilgi
- Komut İlk Çalıştırıldığında Gelen Mesaj
  
  ![vipinfo1](https://cdn.discordapp.com/attachments/1131692946916392962/1236086308686921768/image.png?ex=6636ba95&is=66356915&hm=9ff3565b543e5225f3036d0691c17d9f3cab8d49cdd3cc3ef139808cf0d93959&)
- Bir Butona Tıklayınca
  
  ![vipinfo2](https://cdn.discordapp.com/attachments/1131692946916392962/1236086164159725631/image.png?ex=6636ba72&is=663568f2&hm=878cc4309067c479eafa3ee78150f60fde66d30fad7e74b7caa8c7da875d6f03&)

## 

# Fiyatlandırma

- Botun Satış Fiyatı: 400 ₺
- Editleme Hizmeti: 400 ₺
- 7/24 Sınırsız Destek: 250 ₺

Satın Alım: [discord.gg/titantech](https://discord.gg/titantech)
