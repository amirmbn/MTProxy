# MTProxy
MT-Proto proxy

Install NodeJS, NPM and GIT on Debian & Ubuntu
```
apt-get install nodejs npm git
```

Install NodeJS, NPM and GIT on CentsOS & RHEL
```
yum install nodejs npm git
```

Install PM2 
```
npm install pm2 -g
```

Clone repository on your server:
```
git clone https://github.com/amirmbn/MTProxy.git
```

Start the app in cluster mode using pm2:
```
pm2 start mtproxy.js -i max
```
