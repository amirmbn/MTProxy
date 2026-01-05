# MTProxy
MT-Proto proxy
<br><br>
<div align="right">
به‌روزرسانی سرور و نصب NodeJS، NPM، GIT و PM2 روی اوبونتو (**Ubuntu**) و دبیان (**Debian**)
</div>
<div align="left">
```
sudo apt-get update && sudo apt-get install -y nodejs npm git && sudo npm install -g pm2
```
<br>

Install NodeJS, NPM, GIT and PM2 on **CentsOS** & **RHEL**
```
sudo yum update && sudo yum install -y nodejs npm git && sudo npm install -g pm2
```
<br>

Clone repository on your server:
```
git clone https://github.com/amirmbn/MTProxy.git
```
<br>

Start the app in cluster mode using pm2:
```
pm2 start /root/MTProxy/mtproxy.js -i max
```
<br>

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
