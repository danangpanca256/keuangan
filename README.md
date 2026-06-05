<p align="center">
  <img height="300" height="auto" src="https://github.com/sipalingnode/sipalingnode/blob/main/logo.png">
</p>

<h2 align="center"><b>Follow Community Team</b></h2>
<p align="center">
  <a href="https://www.airdropasc.com" target="_blank"><img src="https://github.com/sipalingnode/sipalingnode/blob/main/logo.png" width="50"/></a>&nbsp;&nbsp;&nbsp;
  <a href="https://t.me/airdropasc" target="_blank"><img src="https://github.com/user-attachments/assets/56e7f6ee-18b7-4b36-becc-ec6e4de7bff9" width="50"/></a>&nbsp;&nbsp;&nbsp;
  <a href="https://x.com/Autosultan_team" target="_blank"><img src="https://github.com/user-attachments/assets/fbb43aa4-9652-4a49-b984-5cf032b6b1ac" width="50"/></a>&nbsp;&nbsp;&nbsp;
  <a href="https://www.youtube.com/@ZamzaSalim" target="_blank"><img src="https://github.com/user-attachments/assets/c15509f9-acb7-49ce-989a-5bac62e7e549" width="50"/></a>
</p>

---
# Manage Your Money
---
## Create Spreasheet Drive
* Open [GoogleDrive](https://drive.google.com/drive/u/0/home)
* Click Baru/New
* Google Spreadsheet
* Contoh URL spreadsheet: https://docs.google.com/spreadsheets/d/1AbCdEfGhIjKlMnOpQrStUvWxYz/edit
* Copy bagian: 1AbCdEfGhIjKlMnOpQrStUvWxYz
* Itu adalah: spreadsheetId
---
## Install Nodejs
```
curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash -
sudo apt install nodejs -y
```
---
## Clone Repository
```
git clone https://github.com/sipalingnode/keuangan.git
cd keuangan
```
---
## Activate Api & Create Apikey Spreadsheet
* Open [GoogleConsole](https://console.cloud.google.com/)
* Klik menu (pojok kiri)
* api&services > library
* pilih google sheet > enable api
* Klik menu (pojok kiri)
* IAM&Admin > service accounts
* create service accounts
* Open service accounts
* Pilih keys > add keys
* Create New Key > pilih json
* Download file json
* Rename json to rekap-credentials.json
* Upload file rekap-credentials.json to folder keuangan
---
## Add Access to Spreadsheet
* Open file rekap-credentials.json
* Cari: "client_email": "rekap-bot@xxxxx.iam.gserviceaccount.com"
* Copy email
* Open Spreadsheet
* Klik share/bagikan
* Add email to editor
---
## Create Telegram Bot
* Open [BotFather](https://t.me/BotFather)
* Send: `/newbot`
* Enter bot name & username
* Copy the BOT TOKEN
## Get Telegram Chat ID
* Open [GetID](https://t.me/userinfobot)
* Send: /start
* Copy your Chat ID
---
## Edit file rekap.json
```
nano rekap.json
```
**Simpan gunakan `CTRL+X+Y` lalu `ENTER`**
---
## Install Modul
```
npm init -y
npm install telegraf googleapis
```
---
## Running
```
node rekap.js
```
---
## Available Commands

| Command                | Description                                   |
|------------------------|-----------------------------------------------|
| `/start`               | Mulai bot dan tampilkan contoh                |
| `/help`                | Tampilkan format transaksi                    |
| `/bulan`               | Rekap bulanan bulan ini                       |
| `/bulan MM YYYY`       | Rekap bulanan untuk bulan tertentu            |
| `/last`                | Lihat transaksi hari ini/terakhir              |
| `/edit` | Edit transaksi   |
| `/hapus`         | Hapus transaksi             |

## Transaction Examples

* masuk airdrop 1.5 jt
* masuk 20 usdt airdrop
* masuk $10 freelance
* keluar wifi 250k
* keluar rokok 30k
* keluar bensin 50rb
---
