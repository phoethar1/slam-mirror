# Slam Mirror bot (https://github.com/SlamDevs/slam-mirrorbot) ကို deployment အတွက် modified လုပ်ထားတဲ့ version ဖြစ်ပါတယ်

## General Usage 
/mirror [anylink including facebook video links]

/watch [youtubelink]

use /help for more

# Deployment ဘယ်လိုလုပ်မလဲ

## Step 1
၁. https://git-scm.com/downloads မှာ git ကို install ပါ 

၂. https://devcenter.heroku.com/articles/heroku-cli မှာ windows 64bit အတွက် heroku cli install ပါ

## Step 2

https://github.com/kzinthant-kas/slammirrorbot-cli.git
ဒီ repo ကို git clone ပါ

အဲ folder ထဲကိုသွားပါ ပြီးရင် token.pickle ကို အဲ folder ထဲထည့်ပါ


## Optional Step (token.pickle)

### token.pickle မရှိရင်ဘယ်လိုယူရလဲ
Service accounts လုပ်ဖူးတဲ့ သူ က service accounts လုပ်ဖူးတဲ့ folder ထဲမှာ ရှိပါမယ် 

မရှိရင် 

၁. google oauth client ကို console.cloud.google.com မှာ publish လုပ်ပါ

၂. client id create ပါ။ json ကို down ပြီး credentials.json လို့ rename ပါ။ အဲ json ကို ခုနက down ထားတဲ့ folder ထဲထည့်ပါ 

၃. ပြီးရင် အဲ folder ထဲမှာ cmd နဲ့ pip3 install -r requirements-cli.txt လုပ်ပါ။ ပြီးရင် py generate_drive_token.py သို့ python3 generate_drive_token.py ဆိုပြီးလုပ်သွားရင် token.pickle ရောက်လာပါမယ်

## Optional Step (service accounts)
တစ်နေ့ကို 750GB ထပ်ပို upload မယ်ထင်ရင် (တကယ်တော့ upload မလုပ်ဖြစ်ကြပါ) service accounts folder ကို repo folder ထဲထည့်ပါ။ foler name က accounts ဖြစ်ရမယ်

ပြီးရင် config.env မှာ USE_SERVICE_ACCOUNTS = "True" လုပ်ပေးရပါမယ်


## Step 3 

config.env ကိုဖွင့်ပါ တန်ဖိုးတွေဖြည့်ပါ။ 

BOT_TOKEN ကို bot father က ယူပြီးဖြည့်ပါ

GDRIVE_FOLDER_ID က upload ရဲ့ folder id ပါ

OWNER_ID ကို https://t.me/MissRose_bot က /id နဲ့ ကြည့်ပြီးထည့်ပါ

IS_TEAM_DRIVE = "True"

TELEGRAM_API = my.telegram.org မှာ login ၀င်ပြီး API developments tools ထဲက App api_id ကိုယူပါ (App မရှိရင် create ပါ)

TELEGRAM_HASH = အပေါ်ကအတိုင်း App api_hash ကိုယူပါ 

mega pro သုံးရင် mega ထည့်ပါ ရိုးရိုးဆိုမလိုပါ

BASE_URL_OF_BOT = "https://appname.herokuapp.com" လို့ဖြည့်ပါ , appname က unique ဖြစ်ရပါမယ် unique ဖြစ်နိုင်တာကိုထည့်ပါ

ကျန်တဲ့ config တွေအသေးစိတ်သိချင်ရင် မူရင် repo https://github.com/SlamDevs/slam-mirrorbot မှာ သွားဖတ်ပါ

## Step 4 

repo folder ထဲမှာ right click -> git bash here လုပ်ပါ

heroku login လုပ်ပြီး heroku ကို authenticate လုပ်ပါ။ ပြီးလို့ရပ်နေရင် ပိတ်ပြီး git bash here ပြန်လုပ်ပါ

အောက် က command လေးတွေကို အစဥ်လိုက်ရိုက်သွားပါ

**Notice: အောက်က appname က config မှာ ပေးခဲ့ တဲ့ unique appname နဲ့တူရမယ်**

> heroku create appname 

> heroku stack:set container

> git add .

> git commit -m "mycommit"

> git push heroku main

ပြီးရင် စောင့်ပါ , heroku မှာ log သွားကြည့်လို့လည်းရတယ်

if there is any question, ask at t.me/drivetalk
