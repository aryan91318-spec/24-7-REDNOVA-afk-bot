# REDNOVA AI Minecraft Bot

यह Mineflayer bot है। यह Minecraft Java server में login करके:
- पेड़ के logs collect कर सकता है (`!wood`)
- पास के ores mine/collect कर सकता है (`!mine`)
- खिलाड़ी के पास आ सकता है (`!come`)
- follow कर सकता है (`!follow`)
- coordinates पर जा सकता है (`!goto x y z`)
- stop/status/inventory commands चला सकता है
- auto-eat और disconnect होने पर reconnect कर सकता है

## जरूरी बात
40 घंटे की गारंटी bot code अकेले नहीं दे सकता। जिस फोन/PC/hosting पर Node.js process चलेगा, वह 40 घंटे online और server तक connected रहना चाहिए। यह server के AFK/kick नियमों को bypass नहीं करता।

## Setup
1. Node.js 18 या नया install करें।
2. इस folder में terminal खोलें।
3. `npm install` चलाएँ।
4. `.env.example` की copy बनाकर `.env` नाम दें।
5. `.env` में अपने server का host/port और bot username भरें।
6. `npm start` चलाएँ।

अगर server offline/cracked है तो `MC_AUTH=offline` रखें। Online-mode server में उस server की authentication requirements के अनुसार account/auth setup चाहिए।

## Commands
`!help`
`!come`
`!follow`
`!stop`
`!wood`
`!mine`
`!status`
`!inv`
`!goto 100 64 -20`

## Security
OWNER_NAME भरने पर chat commands सिर्फ उसी player से स्वीकार होंगे। इसे public server पर उपयोग करते समय whitelist/permissions लगाना बेहतर है।
