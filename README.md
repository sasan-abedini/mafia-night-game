# mafia-night-game

ربات تلگرامی حرفه ای شب های مافیا با پنجاه نقش

پیش نیازا : 
داکر 
 داکر کامپوز  
هر نسخه از سرور ویندوز که داکر روش نصب بشه (  Virtulazation ) روی بایوس فعال  شده باشه
هر ورژن از لینوکس 
Ubuntu 20.04, 22.04 :
sudo apt update;sudo apt upgrade
sudo apt install docker.io
sudo systemctl status docker ( چک کنید سرویس داکر فعال شده باشه )
sudo mkdir -p ~/.docker/cli-plugins/
curl -SL https://github.com/docker/compose/releases/download/v2.25.0/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
sudo chmod +x ~/.docker/cli-plugins/docker-compose
docker compose version ( بعد اینکه مطمئن شدین داکر کامپوز هم نصب شده )

از طریق winscp یا ابزار اف تی پی سورس رو روی سرور اپلود کنید توی دایرکتوری html ( فولدر html)
بررسی کنید یه فایل باید با پسوند yml و دیگری dockfile باید وجود داشته باشه
وارد دایرکتوری بات بشین ، فایل config.php رو ادیت کنید چیزایی که لازمه رو ادیت کنید 
توکن بات : @BotFather
اگر بلد نیستین در کل چطور بات ساخته میشه خیلی سادست توی مقالات ما (توسعه مجازی نیل) اموزش هست. دامین نیازی نداره ولی در صورت ضرورت میتونید تهیه کنید
فقط کافیه  IPv4 رو با اسم ساب ثبت کنید وارد فایل کانفیگ کنید .
ایدی عددی ادمین بات رو هم از userchatinfo تلگرام سرچ کنید میاره بازم اگر هر کجا رو بلد نبودین میتونید از گوگل سرچ کنید .

بعد ادیت به دایرکتوری html مجدد برگردین دستور پایینو وارد کنید :
docker compose up -d —build
و تمام موفق باشین




Professional Mafia Nights Telegram Bot with Fifty Roles

**Prerequisites:**
- Docker
- Docker Compose
- Any version of Windows Server that supports Docker (Virtualization enabled in BIOS)
- Any version of Linux

**For Ubuntu 20.04, 22.04:**
```sh
sudo apt update; sudo apt upgrade
sudo apt install docker.io
sudo systemctl status docker  # Ensure Docker service is active
sudo mkdir -p ~/.docker/cli-plugins/
curl -SL https://github.com/docker/compose/releases/download/v2.25.0/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
sudo chmod +x ~/.docker/cli-plugins/docker-compose
docker compose version  # Verify Docker Compose is installed
```

Upload the source to the server in the html directory using WinSCP or any FTP tool (html folder). Ensure there is a file with the .yml extension and another file named Dockerfile.

Enter the bot directory and edit the config.php file to modify the necessary settings:
- Bot Token: @BotFather
- If you are not familiar with how to create a bot, it's very simple. You can find tutorials on this in our articles (Nile Virtual Development). A domain is not required, but you can obtain one if necessary. Simply register the IPv4 as a subdomain and enter it into the config file.
- Find the bot admin's numeric ID using Telegram's userchatinfo. If you are unsure about anything, you can always search Google for assistance.

After editing, return to the html directory and enter the following command:
```sh
docker compose up -d —build
```
And that's it. Good luck!






