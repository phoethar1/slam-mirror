#  slam-mirrorbot၏ gitကို androidဖုန််းသုံးပြီးgit push heroku လုပ်နည်း


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
[`မိမိဖုန်းfile manager ထဲက MyTermuxဆိုတဲ့ folder ထဲဝင် service-accountsဆိုတဲ့ folderထဲက accounts folderရယ် token.pickle file ကို slam-mirrorဆိုတဲ့ folderထဲမှာ copy လုပ်ပြီးထည့် 
ပြီးရင် slam-mirror folderထဲက config.envကို ဖွင့်ပြီး မိမိ account နဲ သက်ဆိုင်တဲ့ တန်ဖိုးကို ပြင်ဆင်သတ်မှတ်ပါ`](#)












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









