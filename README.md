ℹ️ Hakkında
=========================
Steam Oyun Saati Artırıcı, 2FA desteğine sahip "kişisel bilgisayarınızda" veya "sunucuda" çalıştırabileceğiniz basit ve güvenli bir Steam saat artırma botu'dur.

⬇️ NodeJS'yi yükleyin
=========================
İlk olarak [**NodeJS**](https://nodejs.org/tr/download/)'nin son sürümünü resmi web sitesinden indirin ve bilgisayarınıza kurun. 

🕸️ NodeJS bağlılıklarını yükleyin
=========================
- NodeJS bağlılıklarını yüklemek için sadece `npm install` yeterlidir. Ancak bazı durumlarda yetkilendirme ve imza izinleri eksik olabilir.
- Bu yüzden böyle bir hata ile karşılaşırsanız önce `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser` komutunu çalıştırın. Ardından `npm install` komutunu çalıştırarak sorunsuz ilerleyebilirsiniz.

🎮 Popüler oyun kimlikleri
=========================
Arc Raiders: `1808500`

Counter-Strike: `10`

Half-Life: `70`

Counter-Strike Zero: `80`

Half-Life 2: `220`

Counter-Strike: Source: `240`

Team Fortress 2: `440`

Dota 2: `570`

Counter-Strike 2: `730`

PlanetSide 2: `218230`

Rust: `252490`

PUBG: `578080`

Destiny 2: `1085660`

Apex Legend: `1172470`

Battlefield™ 2042: `1517290`

Battlefield™ 6: `2807960`

C.O.D Warzone: `1962663`

The Finals: `2073850`

🆔 Oyun kimliğini nasıl öğrenebilirim?
=========================
- Steam mağaza sayfasını açın.
- Arama kutusuna Rust yazın ve oyun sayfasını açın.
- Açılan sayfada adres çubuğundaki URL şu şekilde olmalıdır: https://store.steampowered.com/app/252490/Rust/
- URL içindeki bu "252490" numaralar oyunun benzersiz steam kimliğidir.


▶️ Örnek config/accounts.js yapılandırması
=========================
```javascript
// Bu kodları değiştirmeyin veya silmeyin!
var configsArray = []; 
var config;

// Steam Hesabı 1
config = {};
// Steam hesap adı
config.username = 'Hesap_Adınız';
// Steam hesap parolası
config.password = 'Hesap_Parolanız';
// Steam Guard kodu kullanacaksanız burayı boş bırakın.
config.sharedSecret = '';
// Çevrimiçi durumunuzu görünmez kılmak için bu değeri "false" olarak değiştirin.
config.enableStatus = true;
// Steam profilinizde görünmesini istediğiniz özel mesaj ve oyunların Steam mağazası kimlikleri.
config.gamesAndStatus = ['Half-Life 3', 10, 70, 240, 440, 570, 730, 218230, 252490, 578080, 1085660, 1172470, 1962663, 552990,];
// Arkadaş listenizden birisi size mesaj gönderdiğinde otomatik yanıtlayın.
config.replyMessage = 'Steam oyun saatlerimi arttırmak için boşta bekliyorum.';
// Komut terminali mesajlarını bir dosyaya kaydetmek istiyorsanız bu değeri "true" olarak değiştirin.
config.receiveMessages = false;
// Sohbet mesajlarını bir dosyaya kaydetmek istiyorsanız bu değeri "true" olarak değiştirin.
config.saveMessages = false;
// Bu kodu değiştirmeyin veya silmeyin!
configsArray.push(config);

// Bu kodu değiştirmeyin veya silmeyin!
module.exports = configsArray;
```

🫳 Botu elle çalıştırın
=========================
```bash
npm run start
```

⌨️ Botu komut dosyası ile çalıştırın
=========================
Bot ana dizinde Başlat.cmd adında bir dosya oluşturun.
Daha sonra aşağıdaki kod satırını içine yapıştırın ve kaydedin.

```bash
@echo off
npm run start
```

Bu komut dosyası ile kod girmeden botu başlatabilirsiniz.

❤️ Botu otomatik olarak başlat
=========================
Bilgisayar açıldığında botun otomatik olarak başlamasını istiyorsanız aşağıdaki adımları sırasıyla uygulayın.

- İlk olarak, botun kurulu olduğu dizindeki `Başlat.bat` dosyasına `SHIFT` tuşuna basılı tutarak sağ tıklayın ve `Kısayol oluştur` seçeneğine tıklayın.
- Oluşturulan kısayolun adı varsayılan olarak `Başlat.bat - Kısayol` olacaktır.
- Bu dosyaya tekrar sağ tıklayın ve Yeniden adlandır seçeneğini kullanarak adını `Başlat.bat` olarak değiştirin. Sonundaki `- Kısayol` ifadesi tamamen kaldırılmalıdır.
- Dosya Gezgini’ni açın ve adres çubuğuna şu yolu yapıştırıp `ENTER` tuşuna basın:
`C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup`
- Oluşturmuş olduğunuz kısayol dosyasını `CTRL + X` ile kesin ve ardından yukarıdaki `Startup` klasörünün içinde `CTRL + V` tuşlarına basarak yapıştırın.





