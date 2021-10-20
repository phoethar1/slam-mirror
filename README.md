#  slam-mirrorbot၏gitကို android phone သုံးပြီး herokuမှာ git push လုပ်နည်း


```
termux-setup-storage
```
```
pkg update
```
```
pkg upgrade 
```
```
pkg install git
```
```
git config --global user.email "မိမိgmailထည့်@example.com"
```
```
git config --global user.name " Name ထည့်"
```
```
pkg install nodejs-lts
```
```
npm install -g heroku
```
```
npm install -g http-server
```
```
mkdir /sdcard/MyTermux/ -p
```
```
cd /sdcard/MyTermux
```
```
git clone https://github.com/phoethar1/slam-mirror
```
```
cd slam-mirror
```
```
heroku login
```
[`Enter ပြန်​ခေါက် Browser ​ပေါ်​ရောက်သွာမယ်`](#)

```
heroku create appname
```
```
heroku stack:set container
```
```
git add *
```
```
git commit -m "slam-mirror"
```
```
git push heroku main
```









