# MTProxy
MT-Proto proxy<br><br>

Update Server and Install NodeJS, NPM, GIT and PM2 on Debian & Ubuntu
```
sudo apt-get update && sudo apt-get install -y nodejs npm git && sudo npm install -g pm2
```

Install NodeJS, NPM, GIT and PM2 on CentsOS & RHEL
```
sudo yum update && sudo yum install -y nodejs npm git && sudo npm install -g pm2
```

Clone repository on your server:
```
git clone https://github.com/amirmbn/MTProxy.git
```

Start the app in cluster mode using pm2:
```
pm2 start /root/MTProxy/mtproxy.js -i max
```
