<div align="center">
    <img src="https://files.catbox.moe/4dt7iv.jpg" width="100%" style="margin-left: auto;margin-right: auto;display: block;">
</div>

<h1 align="center">Elaina Base - WhatsApp Bot</h1>
<h3 align="center">Clean & Simple WhatsApp Bot for Termux</h3>

<p align="center">
<a href="https://github.com/naim-SC/elaina-base">
<img title="Author" src="https://img.shields.io/badge/AUTHOR-Nimzz-green?style=for-the-badge&logo=Github">
</a>
<img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white">
<img src="https://img.shields.io/badge/Baileys-25D366?style=for-the-badge&logo=whatsapp&logoColor=white">
<img src="https://img.shields.io/badge/Termux-000000?style=for-the-badge&logo=android&logoColor=white">
</p>

<div align="center">
    <a href="https://github.com/naim-SC">
        <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&duration=4000&color=FF6B8B&center=true&vCenter=true&width=600&lines=Hello,+I+am+Nimzz;Welcome+to+Elaina+Base+🤖" alt="Typing SVG" />
    </a>
</div>

<div align="center">
  <img src="https://count.getloli.com/@naim-SC?name=elaina-base&theme=booru&padding=7&offset=0&align=center&scale=2&pixelated=1&darkmode=0" align="center">
</div>

📢 Connect With Me

<p align="center">
  <a href="https://whatsapp.com/channel/0029VbAwI4cJ3jv4IuzKob04"><img src="https://img.shields.io/badge/Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"></a>
  <a href="https://wa.me/6282364532184"><img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"></a>
  <a href="https://t.me/pantatbegetar"><img src="https://img.shields.io/badge/Telegram-0088cc?style=for-the-badge&logo=telegram&logoColor=white"></a>
  <a href="https://github.com/naim-SC"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"></a>
</p>

✨ Features

· ✅ Termux Compatible - Works perfectly on Android Termux
· ✅ Clean Codebase - No bloat, easy to modify
· ✅ Dual Connection Mode - QR Code & Pairing Code support
· ✅ Sticker Creator - Image/Video to WebP with EXIF
· ✅ Multi Database - JSON & MongoDB support
· ✅ Owner System - Easy owner management
· ✅ Premium Features - User premium management
· ✅ Anti-Delete - Detect deleted messages
· ✅ Auto Backup - Backup script feature
· 🎯 NEW: Case Management - Add/del case via command
· 🎮 NEW: Fun Commands - Games & entertainment
· 🔧 NEW: Tools Utility - Converter & calculators
· 💫 Enhanced Menu - Better UI & organization

🚀 Installation

For Termux User

```bash
# Update package manager
pkg update && pkg upgrade -y

# Install dependencies
pkg install nodejs git ffmpeg -y

# Clone repository
git clone https://github.com/naim-SC/elaina-base.git
cd elaina-base

# Install npm packages
npm install --legacy-peer-deps

# Configure bot
nano settings.js

# Run bot
npm start
```

For Ubuntu/SSH User

```bash
apt update && apt upgrade -y
apt install nodejs git ffmpeg -y
git clone https://github.com/naim-SC/elaina-base.git
cd elaina-base
npm install --legacy-peer-deps
npm start
```

⚙️ Configuration

Edit settings.js file:

```javascript
global.owner = ["6282364532184"]          // Your WhatsApp number
global.namaOwner = "Nimzz"                // Your name
global.namaBot = "Elaina"                 // Bot name
global.pairing_code = false               // false = QR Code, true = Pairing Code
global.pairingKode = 'ELAINA67'           // Your pairing code
global.linkSaluran = "https://whatsapp.com/channel/0029VbAwI4cJ3jv4IuzKob04" // Channel link
```

📁 Project Structure

```
elaina-base/
├── index.js          # Main bot file
├── settings.js       # Configuration
├── case.js          # Command handler (MAIN FILE)
├── lib/             # Core libraries
│   ├── message.js   # Message processing
│   ├── myfunction.js # Utilities
│   ├── exif.js      # Sticker creator
│   ├── converter.js # Media converter
│   └── database.js  # Database handler
├── data/            # Database files
│   ├── owner.json   # Owner list
│   ├── premium.json # Premium users
│   └── settings.json # Bot settings
├── package.json     # Dependencies
├── tmp/            # Temporary files
└── README.md        # Documentation
```

🛠️ Available Commands

📋 Main Commands

```
.menu          - Show main menu
.ping          - Check bot status
.status        - Bot status info
.help          - Quick help
.time          - Current time
.date          - Today's date
```

🎮 Fun & Games (NEW)

```
.fun-menu      - Show fun games menu
.quote         - Inspirational quotes
.motivasi      - Motivation words
.fakta         - Random facts
.tebak         - Guessing game
.jawab         - Answer guessing game
.truth         - Truth questions
.dare          - Dare challenges
.bijak         - Wise words
.jodoh <nama1> & <nama2> - Match prediction
.siapaaku      - Guess character game
.apakah        - Random questions
.rate <something> - Rate something
.kapankah      - Time prediction
.bucin         - Love quotes
.gombal        - Sweet talks
.dice          - Roll dice
.coin          - Flip coin
.8ball <question> - Magic 8-ball
.choose <option1> | <option2> - Choose random
.random <min> <max> - Random number
```

🔧 Tools & Utility (NEW)

```
.tools-menu    - Show tools menu
.calc <expression> - Calculator
.base64 <encode/decode> <text> - Base64 converter
.binary <encode/decode> <text> - Binary converter
.hex <encode/decode> <text> - Hex converter
.style <text>  - Text styling
.fontlist      - Font list
.flip <text>   - Flip text
.qrcode <text> - Create QR code
.stickerinfo   - Sticker information
.getexif       - Media info
.say <text>    - Repeat text
.echo <text>   - Echo text
```

👑 Owner Commands

```
.owner-menu    - Show owner menu
.addowner <number> - Add new owner
.delowner <number> - Remove owner
.addprem <number> <days> - Add premium user
.delprem <number> - Remove premium user
.listprem      - List premium users
.backup        - Backup bot script
.self          - Set self mode
.public        - Set public mode
.addcase <name> - Add new case
.addcaser <name> - Add case with reply code (NEW)
.delcase <name> - Delete case
.getcase <name> - View case code
```

⚡ Advanced Features

```
.x <code>      - Execute code (owner only)
.xx <async code> - Execute async code (owner only)
$ <command>    - Execute shell command (owner only)
```

🎯 Key Improvements (Modifikasi)

1. Enhanced Case Management

```javascript
.addcaser testcase
// Reply dengan kode yang ingin ditambahkan
// Example reply: m.reply("Hello World!");
```

2. Fun Factory System

· 100+ quotes, facts, and games
· No API required
· Local data storage
· Interactive games

3. Utility Tools

· Base64/Binary/Hex converters
· Text styling options
· Calculator with safety checks
· QR code generator

4. Better Menu System

· Organized command categories
· Clear descriptions
· External ad reply integration
· Better user experience

5. Improved Error Handling

· Consistent error messages
· Safety checks for eval/exec
· Graceful degradation

📸 Preview Commands

<div align="center">
  <table>
    <tr>
      <td><strong>Menu System</strong></td>
      <td><strong>Fun Games</strong></td>
      <td><strong>Tools</strong></td>
    </tr>
    <tr>
      <td>
        <img src="https://img.shields.io/badge/Main_Menu-7289DA?style=flat-square&logo=whatsapp&logoColor=white">
      </td>
      <td>
        <img src="https://img.shields.io/badge/Fun_Games-FF6B8B?style=flat-square&logo=gamepad&logoColor=white">
      </td>
      <td>
        <img src="https://img.shields.io/badge/Tools-25D366?style=flat-square&logo=tools&logoColor=white">
      </td>
    </tr>
    <tr>
      <td><code>.menu</code></td>
      <td><code>.tebak</code></td>
      <td><code>.calc 10+5*2</code></td>
    </tr>
    <tr>
      <td><code>.owner-menu</code></td>
      <td><code>.jodoh Budi & Ani</code></td>
      <td><code>.base64 encode Hello</code></td>
    </tr>
    <tr>
      <td><code>.fun-menu</code></td>
      <td><code>.quote</code></td>
      <td><code>.qrcode https://...</code></td>
    </tr>
  </table>
</div>

🐛 Troubleshooting

Common Issues & Solutions

```bash
# Error: Cannot find module
rm -rf node_modules package-lock.json
npm install --legacy-peer-deps

# Error: Permission denied
chmod 755 *.js
npm install --no-bin-links

# Error: FFmpeg not found
pkg install ffmpeg -y

# Bot not connecting
rm -rf session
node index.js

# JSZip not found (for backup)
npm install jszip --legacy-peer-deps
```

Quick Fix Script

```bash
#!/bin/bash
# Save as fix.sh and run: bash fix.sh

echo "🔧 Fixing common issues..."
rm -rf node_modules package-lock.json
npm cache clean --force
npm install --legacy-peer-deps --no-bin-links
echo "✅ Done! Try: npm start"
```

📊 GitHub Stats

<p align="center">
  <a href="https://github.com/naim-SC">
    <img src="https://github-readme-stats.vercel.app/api?username=naim-SC&show_icons=true&theme=chartreuse-dark&hide_border=true">
  </a>
  <a href="https://github.com/naim-SC">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=naim-SC&theme=chartreuse-dark&hide_border=true">
  </a>
</p>

<p align="center">
  <a href="https://github.com/naim-SC">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=naim-SC&theme=chartreuse-dark&layout=compact&hide_border=true">
  </a>
</p>

🤝 Contributing

1. Fork the Project
2. Create your Feature Branch (git checkout -b feature/AmazingFeature)
3. Commit your Changes (git commit -m 'Add some AmazingFeature')
4. Push to the Branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

Note: This is a modified version based on the original Elaina Base. Please give credit to the original author while modifying.

⭐ Support

Jika project ini membantu Anda, jangan lupa kasih ⭐ ya!
Saran saya pake panel aja ya 🗿

---

<div align="center">
  <p>Made with ❤️ by <a href="https://github.com/naim-SC">Nimzz</a></p>
  <p><strong>⚠️ Note:</strong> Ini adalah base hasil modifikasi dengan penambahan fitur-fitur baru dan perbaikan struktur kode.</p>
  <p>© 2026 - Elaina Base | WhatsApp Bot (Modified Version)</p>
  <p>🚀 <strong>Modifikasi Features:</strong> Case Management, Fun Games, Tools Utility, Enhanced Menus</p>
</div>
