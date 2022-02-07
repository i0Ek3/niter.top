# Welcome to [i0Ek3's Galaxy](https://niter.top)


> I'm good! And you?

This is my personal website which I build and generate by Hugo to record my experiences and what I learned from Internet. Also have some posts just like tweet and the fun stuffs I collected from somewhere.




## Record

Some days ago, my blog on Netlify went offline cause of I changed it's name servers to the original one(Namesilo). So I decide to record what should I do after my blog offline. Here's thing:

First, I found some seemingly available solutions:

- buy a new domain(or register a free one on Freenom) to bind your VPS and restore my blog(finally, I used this one)
- deploy your site on your VPS instead of Netlify with rsync(use deploy script to deploy your website on your VPS)
- configure external DNS for Netlify, ref [here](https://docs.netlify.com/domains-https/custom-domains/configure-external-dns/)(add A record with IP 75.2.60.5, but nothing gonna happen)
- use Nginx to reverse proxy(I didn't have a try)
- find the other solution(like hyber name servers, it seems not work well)

Secondly, I just tried the third one and I got nothing. 

~~Today, I want to try to deploy my blog on my VPS and to look what happened. And now, you can visit my blog again~~. 

And I added some themes, you can visit [here](https://github.com/i0Ek3/niter.top/tree/master/themes) to see what kind themes is my type, I'll pick one of them as my default theme.

Enjoy!



## How To?

> This is another record to show how my website [https://niter.top](https://niter.top) online again.

- First, I register a new domain on Freenom(my lucky, only work in U.S. IP), and detach my original one(niter.top)
- Second, bind my VPS IP on new domain and released niter.top
- Third, clean all stuffs on my GitHub about Netlify and Netlify it's own
- Fourth, re-login Netlify and generate new team or use original one, authorized GitHub on Netlify, and follows steps to setting
- Next, adjust the structure of niter.top on GitHub and reuse netlify.toml, add gitflow
- Last, run command `hugo -D` to generate static website resource on public and git push all things on GitHub
- Here we are




## Deploy on VPS

> DO NOT RUN ./deploy DIRECTLY!

Before you deploy your website on your VPS, you need to change follows items in script deplpy to your own to make sure this script work well:

- HOST: like niter.top
- DIR: where you put the public/ on your VPS
- YOUR_PORT: like 22 or something else

After that, run command `hugo -D` and run script `./deploy` to deploy. 



## To-Do List

- [x] support https
- [x] support [picture upload](https://github.com/Molunerfinn/PicGo)
    - use picx: [https://github.com/XPoet/picx](https://github.com/XPoet/picx)
- [x] support comment system
- [ ] enable [cdn](https://www.jsdelivr.com/) speed up
- [ ] support traffic analysis
- [ ] support [i18n & l10n](https://www.bmpi.dev/dev/i18n-l10n/)



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


## Reference

- Check how to deploy your website on different stuffs: [https://gohugo.io/hosting-and-deployment/hugo-deploy/](https://gohugo.io/hosting-and-deployment/hugo-deploy/)
- Deploy website on your VPS(but this post have some issues, please kindly be informed): [https://www.enit.xyz/tech/deploy-hugo-on-vps/](https://www.enit.xyz/tech/deploy-hugo-on-vps/)



## Credit

You All Guys!
