# rest api test
this for download social media
tiktok
bucin

this still upgrade for add Instagram pinterest cocofun YouTube




HOW TO USE ??


```
const fs = require("fs");
const axios = require("axios");
const path = require("path");

async function runtik() {
    let url = "https://raw.githubusercontent.com/Reddool/Offset-Game/main/api.js";
    
    let urlTiktok = "https://vt.tiktok.com/ZSMHQj78p/"
    
    let filePath = path.join(__dirname, "api.js");
    try {
        const response = await axios.get(url);
        fs.writeFileSync(filePath, response.data);
        console.log("🚀 Menjalankan script TikTok...");
        const tik = require(filePath);
        tik.ttvid(urlTiktok);

    } catch (error) {
        console.error("❌ Gagal mengambil atau menjalankan script. Mungkin ada update atau URL salah.", error);
    }
}

runtik();
```
