#  slam-mirrorbot၏ gitကို androidဖုန််းသုံးပြီးgit push heroku လုပ်နည်း
## Guide:
-  YouTube Guide:[Tutorial video](https://youtu.be/vCj3_kufRCc)
-----

-  အရင်ဆုံး Termux ကို မိမိဖုန်းထဲ install လုပ်ပါ။Termux ကို ​အောက်ကပုံ နိပ်ပြီး downloadလုပ်ပါ
[![](1.png)version 0.117](https://drive.google.com/uc?export=download&id=19VycS90NijIR1u_KYTumRJDu4c2xKK7P)
--------
-  Service Accounts မလုပ်တက်ရင် ​အောက်ကနည်းအတိုင်းပြုလုပ်ပါ

          ⬇️⬇️

   [Create Service Accounts](https://github.com/phoethar1/service-accounts)
---------
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

--------
-  confing.env ဖွင့်မရရင် ​[ဒီLINK က app](https://www.google.com/url?sa=t&source=web&rct=j&url=https://play.google.com/store/apps/details%3Fid%3Dcom.rhmsoft.edit%26hl%3Dmy%26gl%3DUS%26referrer%3Dutm_source%253Dgoogle%2526utm_medium%253Dorganic%2526utm_term%253Dquickedit%26pcampaignid%3DAPPU_1_ovhvYZL5C4e6qtsP5cWDsA4&ved=2ahUKEwiS0uPc7NjzAhUHnWoFHeXiAOYQ5YQBegQIBhAC&sqi=2&usg=AOvVaw1CNFUinhUrTrs3FLQFv64Q)ကိုdownloadလုပ် ပြီးရင်confing.env.txt​ ခန name changeလိုက် ဖြည့်စရာဖြည့်ပြီးရင် နဂို name (config.env )rename ပြန်လုပ်
--------
-  BOT_TOKEN ​နေရာမှာ [BotFather](https://t.me/BotFather)က​နေToken ယူပြီးဖြည့်

-  GDRIVE_FOLDER_ID ​နေရာမှာ မိမိ upload လုပ်မယ့် folder id ဖြည့်

-  OWNER_ID ​နေရာမှာ [MissRose_bot](https://t.me/MissRose_bot)မှာ/idလို့ ပို့လိုက် idကျလာရင် idကို copy လုပ်ပီးဖြည့်လိုက်

-  IS_TEAM_DRIVE ​နေရာမှာ "True"

-  TELEGRAM_API ​နေရာမှာ my.telegram.orgမှာ loginဝင်ပြီးAPI developments tools ထဲက App api_id ကိုcopy လုပ်ပြီးဖြည့်ပါ ပြီးရင်App api_hashကို copyလုပ်ပြီး TELEGRAM_HASH ​နေရာမှာဖြည့်လိုက်ပါ

-  USE_SERVICE_ACCOUNTS ​နေရာမှာ "True"

-  BASE_URL_OF_BOT ​နေရာမှာ https://မိမိherokuappname.herokuapp.com လို့ဖြည့်(appname က unique ဖြစ်နိုင်တာကိုထည့်ပါ)

-  account folderနဲ့ token.pickle file ကို slam-mirror folderထဲ copyကူးလာထည့်
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









