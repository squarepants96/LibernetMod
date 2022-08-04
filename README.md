# Info
- Hanya mengedit ulang auto reconnect yang sudah ada [di sini!](https://github.com//zzzt27/liberfix/)
- Libernet harus libernet ori/fresh installer bisa klik [di sini!](https://github.com/lutfailham96/libernet)

## Cara Instal
- Stop libernet kalau masih running
- Siapin kuota reguler
#
 Copas ke terminal
- Pertama
```sh
rm /root/libernet/bin/auto_recon.sh
rm /root/libernet/bin/service.sh
rm /root/libernet/system/config.json
wget -O "/root/libernet/bin/auto_recon.sh" --no-check-certificate https://raw.githubusercontent.com/squarepants96/LibernetMod/main/root/libernet/bin/auto_recon.sh && chmod +x /root/libernet/bin/auto_recon.sh
wget -O "/root/libernet/bin/service.sh" --no-check-certificate https://raw.githubusercontent.com/squarepants96/LibernetMod/main/root/libernet/bin/service.sh && chmod +x /root/libernet/bin/service.sh
wget -O "/root/libernet/system/config.json" --no-check-certificate https://raw.githubusercontent.com/squarepants96/LibernetMod/main/root/libernet/system/config.json && chmod +x /root/libernet/system/config.json

```
- Kedua
```sh
rm /www/libernet/api.php
rm /www/libernet/index.php
rm /www/libernet/js/index.js
wget -O "/www/libernet/api.php" --no-check-certificate https://raw.githubusercontent.com/squarepants96/LibernetMod/main/www/libernet/api.php && chmod +x /www/libernet/api.php
wget -O "/www/libernet/js/index.js" --no-check-certificate https://raw.githubusercontent.com/squarepants96/LibernetMod/main/www/libernet/js/index.js && chmod +x /www/libernet/js/index.js
wget -O "/www/libernet/index.php" --no-check-certificate https://raw.githubusercontent.com/squarepants96/LibernetMod/main/www/libernet/index.php && chmod +x /www/libernet/index.php

```

- Clear cache browser untuk menghindari error
- Save ulang config (SSH-WS-CDN, dkk)

#
Biar libernetnya gk berat karena kebanyakan log, copas ini ke schedule task (hapus log setiap 3 jam)
```sh
0 */3 * * * rm /root/libernet/log/service.log && touch /root/libernet/log/service.log
```
#
