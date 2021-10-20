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

`BOT_TOKEN ​နေရာမှာ [BotFather](@BotFather)က​နေ ယူပြီးဖြည့်`

`GDRIVE_FOLDER_ID ​နေရာမှာ မိမိ upload လုပ်မယ့် folder id ဖြည့်`

OWNER_ID ​နေရာမှာ [MissRose_bot](https://t.me/MissRose_bot)မှာ/idလို့ ပို့လိုက် idကျလာရင် idကို copy လုပ်ပီးဖြည့်လိုက်

`IS_TEAM_DRIVE ​နေရာမှာ "True"`

`TELEGRAM_API ​နေရာမှာ my.telegram.orgမှာ loginဝင်ပြီးAPI developments tools ထဲက App api_id ကိုcopy လုပ်ပြီးဖြည့်ပါ ပြီးရင်App api_hashကို copyလုပ်ပြီး TELEGRAM_HASH ​နေရာမှာဖြည့်လိုက်ပါ`

`USE_SERVICE_ACCOUNTS ​နေရာမှာ "True"`

`BASE_URL_OF_BOT ​နေရာမှာ https://မိမိherokuappname.herokuapp.com လို့ဖြည့်(appname က unique ဖြစ်နိုင်တာကိုထည့်ပါ)`

ပြီးရင်

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
`(config.envမှာဖြည့်ထားတဲheroku app name)`
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









