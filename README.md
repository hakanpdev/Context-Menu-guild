
# Context Menu Guild
Discord botlarda “Context Menu” (sağ tık menüsü) komutları kolayca oluşturmanı sağlayan bir tool





## 🚀 Özellikler / Features
Message Type context menü komutları

User Type context menü komutları

Discord resmi dokümanlarına uygun, kolay uygulanabilir kullanım

GPL‑3.0 lisansıyla açık kaynaklı ve özgür
##  ⚙️ Kullanım / Usage
Message ya da User tipinde komutlar oluşturun.

Discord API dökümantasyonundaki “Context Menus” kısmına bakarak mantığı anlayın.

Komutları bot’unuza kaydetmeyi unutmayın.

Örneğin:

```javascript
// Hypothetical örnek (Node.js + discord.js v14+)
// Message context menu
const { ContextMenuCommandBuilder } = require('discord.js');

const myMessageMenu = new ContextMenuCommandBuilder()
  .setName('Some message action')
  .setType(3); // 3 = mesaj

// User context menu
const myUserMenu = new ContextMenuCommandBuilder()
  .setName('Some user action')
  .setType(2); // 2 = kullanıcı

// Bunları botunuzun register işlemlerine ekleyin:
client.application.commands.set([
  myMessageMenu.toJSON(),
  myUserMenu.toJSON()
]);
```




## 🤝 Katkı / Contributing
Fork yap

Farklı branşta geliştirme yap

Pull request aç

Her türlü katkı değerlidir. Ufak düzenlemelerden yeni özelliklere kadar herşeyi bekleriz 😊


## 📄 Lisans / License
Bu proje GPL‑3.0 lisansı ile korunmaktadır.


## 📂 Dosya Yapısı / File Structure

```
Context-Menu-guild/
├── .gitignore
├── LICENSE (GPL‑3.0)
├── README.md
├── src/
│   ├── index.js  ← Örnek implementasyon olabilir
│   └── commands/ ← Context Menü komutları için klasör
└── examples/ ← (Varsa) örnek kullanımlar
```
## 👨‍💻 Geliştirici / Developer

@hakanpdev
