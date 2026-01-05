# MTProxy
MT-Proto proxy
<br><br>
<div align="right">

این پروژه امکان راه‌اندازی دو نوع پروکسی تلگرام را فراهم می‌کند؛ نسخه ساده بدون تبلیغات و نسخه همراه با تبلیغات.<br><br><br>
به‌روزرسانی سرور و نصب NodeJS، NPM، GIT و PM2 روی اوبونتو (**Ubuntu**) و دبیان (**Debian**)
</div>
<div align="left">

```
sudo apt-get update && sudo apt-get install -y nodejs npm git && sudo npm install -g pm2
```
</div><br>
<div align="right">

نصب NodeJS، NPM، GIT و PM2 روی سنت‌اواس (**CentsOS**) و رد هت اینترپرایز لینوکس (**RHEL**)
</div>
<div align="left">

```
sudo yum update && sudo yum install -y nodejs npm git && sudo npm install -g pm2
```
</div><br>
<div align="right">

کلون کردن مخزن (**Repository**) روی سرور شما:
</div>
<div align="left">

```
git clone https://github.com/amirmbn/MTProxy.git
```
</div><br>
<div align="right">

اجرای برنامه در حالت کلاستر (**Cluster**) با استفاده از PM2:
</div>
<div align="left">

```
pm2 start /root/MTProxy/mtproxy.js -i max
```
</div><br>

<div align="right">

### نسخه همراه با تبلیغات
</div><br>
<div align="right">

سرور اوبونتو را آپدیت کنید
</div>
<div align="left">

```
apt-get update
```
</div><br>
<div align="right">

نصب Docker روی اوبونتو / دبیان
</div>
<div align="left">

```
apt-get install docker.io
```
</div><br>
<div align="right">

پروکسی را برای دریافت تگ (TAG) از بات @MTProxybot اجرا کنید
</div>
<div align="left">

```
docker run -d -p6900:443 --name=mtproto-proxy --restart=always -v proxy-config:/data -e SECRET=fe7034e21304d30a82f634358a5ab18f telegrammessenger/proxy:latest
```
</div><br>
<div align="right">

قبل از اجرا کد زیر به بات @MTProxybot در تلگرام مراجعه کنید و یک پروکسی جدید بسازید و آی پی سرور و پورت 6900 اگر تغییر ندادید و سکرت کد fe7034e21304d30a82f634358a5ab18f را به ربات بدهید و در نهایت تگی که بات به شما میدهد را ذخیره کنید تا در ادامه نیاز میشود<br>
و در ادامه پروکسی را انتخاب و Edit promotion را بزنید و آیدی کانال تلگرامی که میخواهید تبلیغ کنید را وارد کنید<br>
کد زیر برای متوقف کردن کانتینر mtproto-proxy است
</div>
<div align="left">

```
docker container stop mtproto-proxy
```
</div><br>
<div align="right">

پاک کردن کانتینر mtproto-proxy
</div>
<div align="left">

```
docker container rm mtproto-proxy
```
</div><br>
<div align="right">

در کد زیر تگی که بات @MTProxybot به شما داد رو جایگزین 40e3b3c69143e023f9800261257b7760 کنید
</div>
<div align="left">

```
docker run -d -p6900:443 --name=mtproto-proxy --restart=always -v proxy-config:/data -e WORKERS=0 -e SECRET=fe7034e21304d30a82f634358a5ab18f -e TAG=40e3b3c69143e023f9800261257b7760 telegrammessenger/proxy:latest
```
</div><br>

## 💰 Support This Project with Crypto
[![Donate BTC](https://img.shields.io/badge/Donate-BTC-orange)](https://www.blockchain.com/btc/address/bc1qul4v4rudyl7lacekfp8yda5sc5575mh2tzv9au)
[![Donate ETH](https://img.shields.io/badge/Donate-ETH-purple)](https://etherscan.io/address/0x79Bb867649277272C65ae047083A36ea91DFeE5B)
[![Donate TRX](https://img.shields.io/badge/Donate-TRX-red)](https://tronscan.org/#/address/TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6)
[![Donate USDT](https://img.shields.io/badge/Donate-USDT-green)](https://tronscan.org/#/address/TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6)

<br>

Bitcoin `bc1qul4v4rudyl7lacekfp8yda5sc5575mh2tzv9au`

Ethereum `0x79Bb867649277272C65ae047083A36ea91DFeE5B`

Tron `TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6`

Tether (TRC20) `TVdJjbJLMdSLzEZEsWuCutjo5RimaiATd6`
