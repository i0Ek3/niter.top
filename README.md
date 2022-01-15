# Welcome to [i0Ek3's Galaxy](https://niter.top)


## Record

My blog(niter.top) was down today, cause of I changed my domain's name servers to the original one, which offered by Namesilo. So I decide to record what should I do after this:

- Open [https://app.netlify.com](https://app.netlify.com) and login with your account
- Find `Domain management` item, and you will see `Check DNS configuration`. In this item, you need set the name servers offered by Netlify instead of your domain provider it's own. But if you want to use domain for Netlify and VPS at same time, you need find a way to fix it. So I thought some methods to solve this problem:
    - buy a new domain(or register a free one) to bind your VPS, restore the original one
    - [WIP] deploy your site on your VPS instead of Netlify
    - configure external DNS for Netlify, ref [here](https://docs.netlify.com/domains-https/custom-domains/configure-external-dns/)(add A record with IP 75.2.60.5)
    - use Nginx to reverse proxy
    - find the other solution(like hyber name servers, it seems not work well)

I just tried the third one and I got nothing, maybe I need some time to study how to made that work first, and then try the other methods.


## To-Do List

- [x] support https
- [x] support [picture upload](https://github.com/Molunerfinn/PicGo)
    - use picx: [https://github.com/XPoet/picx](https://github.com/XPoet/picx)
- [ ] support comment system
- [ ] support traffic analysis
- [ ] support [i18n & l10n](https://www.bmpi.dev/dev/i18n-l10n/)
- [ ] enable [cdn](https://www.jsdelivr.com/) speed up



## Something About Blog Tags And Categories

There are three categories and several tags in every category, just like:

- 个人见闻（PK: Personal Knowledge）
    - 情感（Emotion）
    - 经历分享（Sharing）
    - etc.
- 玩物丧志（BG: Be a Geek）
    - 刷机（Play）
    - 开箱（Unpack）
    - etc.
- 学习笔记（LN: Learning Note）
    - 源码阅读（Source Code Reading）
    - 想法（Ideas）
    - etc.


## Credit

You All Guys!
