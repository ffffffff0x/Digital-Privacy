<p align="center">
    <img src="./assets/img/logo.png">
</p>

---

# Manual

> 世界上有两种密码:一种是防止你的小妹妹偷看你的文件;另一种是防止当局阅读你的文件.

- Bruce Schneier《应用密码学》

<p align="center">
    <a href="https://en.wikipedia.org/wiki/Wojciech_Kossak"><img src=".//assets/img/readme.jpg"></a>
</p>

**项目起因 :** 为了保护自己的隐私,慢慢的开始学习与收集各种手段方法、网站、工具,我把这种行为称作数字洁癖.这些手段方法藏着掖着也不能当传家宝,那干脆就分享出来造福大众.

**涉及内容 :** 个人的隐私保护、查询手段,开源信息收集(OSINT)对抗等

**更新时间 :** 不定期

**事件集合 :** 还不清楚严重性？进来了解近年来的数据泄露、供应链污染事件:[Dork-Admin](https://github.com/No-Github/Dork-Admin)

**项目地址 :** https://github.com/No-Github/Digital-Privacy

---

## 免责声明

1. `本项目所有内容,仅供学习和研究使用,请勿使用项目的技术手段用于非法用途,任何人造成的任何负面影响,与本人无关.`

2. `本文档所有内容、新闻皆不代表本人态度、立场,如果有建议或方案,欢迎提交 issues`

3. `未收及不会收取任何广告费用,推荐的所有工具链接与本人无任何利害关系`

**tips**

1. 对于各类平台尽量使用不同昵称、头像.
2. 多平台不要使用统一、相似的密码,请建立一套自己的密码管理方式,推荐使用密码管理器.对于密码管理器本身的安全性,可以参考这个报告 https://www.securityevaluators.com/casestudies/password-manager-hacking/
3. 管住自己的炫耀欲.
4. 不要相信哪个公司不作恶、重视隐私.(感觉和2有冲突啊 XD)
5. 尽量少用部分浏览器"记住密码"的功能,chrome 是明文保存,而 firefox,可以参考该新闻 https://www.bleepingcomputer.com/news/security/mozilla-firefox-bug-let-third-parties-access-saved-passwords/
6. 不要以为开虚拟机、挂 vpn 就很安全,webRTC 泄露 IP,浏览器指纹,通过 DNS 判断(参考网飞),系统时间,浏览器 0day,等等等等.
7. 所以不要干坏事、不要干坏事、不要干坏事

---

## 大纲
* [隐秘性查询](#隐秘性查询)
    * [隐私查询](#隐私查询)
    * [浏览器指纹](#浏览器指纹)
    * [密码查询](#密码查询)
    * [DNS信息](#DNS信息)
    * [定位](#定位)
* [保护手段](#保护手段)
    * [操作系统](#操作系统)
    * [软件-脚本](#软件-脚本)
    * [浏览器扩展](#浏览器扩展)
    * [安全删除](#安全删除)
    * [加密](#加密)
    * [flash](#flash)
    * [輸入法](#輸入法)
    * [搜索引擎](#搜索引擎)
    * [身份生成](#身份生成)
    * [邮箱-信息](#邮箱-信息)
        * [查邮箱存活](#查邮箱存活)
        * [短信接码](#短信接码)
        * [临时邮箱](#临时邮箱)
        * [匿名邮箱](#匿名邮箱)
    * [平台管控设置](#平台管控设置)
* [OSINT](#OSINT)
    * [设备-语音助手](#设备-语音助手)
    * [平台-软件](#平台-软件)
    * [敏感信息](#敏感信息)
        * [EXIF信息](#EXIF信息)
    * [各类搜索](#各类搜索)
        * [航班](#航班)
        * [船舶](#船舶)
        * [可信度](#可信度)
        * [搜图](#搜图)
            * [acg](#acg)
        * [hack](#hack)
            * [wooyun](#wooyun)
        * [学术](#学术)
        * [物流](#物流)
        * [专利-商标](#专利-商标)
        * [报刊](#报刊)
        * [图表](#图表)
        * [数据](#数据)
        * [BGP](#BGP)
        * [电子硬件相关](#电子硬件相关)
        * [快照](#快照)
        * [社交-人际关系](#社交-人际关系)
    * [天气-环境](#天气-环境)
    * [地图](#地图)
        * [网络攻击地图](#网络攻击地图)

---

# 隐秘性查询
## 隐私查询
- [查你这个IP下载过哪些磁力链接🔗 太缺德了😂 Torrent downloads and distributions for IP](http://iknowwhatyoudownload.com/)
- [你注册过哪些网站？一搜便知](https://reg007.com/)
- [Instant Username Search](https://instantusername.com/#/)
- [n0tr00t/Sreg](https://github.com/n0tr00t/Sreg) - Sreg 可对使用者通过输入 email、phone、username 的返回用户注册的所有互联网护照信息.
- [seadog007/breach.tw](https://github.com/seadog007/breach.tw) - 一种可以跟踪数据违规行为的服务,例如"Have I Been Pwned",但这是针对台湾的.
- [decoxviii/userrecon-py](https://github.com/decoxviii/userrecon-py) - 一个查询数百个网站用户的脚本工具

---

## 浏览器指纹
- [Am I unique?](https://amiunique.org/fp)
- [Unique Machine](http://uniquemachine.org/)
- [Panopticlick](https://panopticlick.eff.org/)
- [Detect Canvas Fingerprint :: WebBrowserTools](https://webbrowsertools.com/canvas-fingerprint/)
- [What is my User Agent :: WebBrowserTools](https://webbrowsertools.com/useragent/)
- **相关文章**
    - [浏览器指纹](https://wzyboy.im/post/1130.html)
    - [2.5代指纹追踪技术—跨浏览器指纹识别](https://www.freebuf.com/articles/web/139984.html)
    - [浏览器指纹真的有效吗？](http://www.arkteam.net/?p=4147)
    - [浏览器的隐身模式有多隐身？](https://www.solidot.org/story?sid=61446)
    - [Cookieless cookies](http://lucb1e.com/rp/cookielesscookies/)
- **webRTC**
    - [ 你的VPN泄漏IP了吗:仍有20%的VPN服务商未解决WebRTC漏洞问题 ](https://www.freebuf.com/articles/web/166754.html)
- **leak HTTP**
    - [cure53/HTTPLeaks](https://github.com/cure53/HTTPLeaks) - 对于网页泄漏 HTTP 请求的方法总结

---

## 密码查询
- [DeHashed](https://dehashed.com/)
- [Have I Been Pwned: Check if your email has been compromised in a data breach](https://haveibeenpwned.com/)
- [pwd query](https://pwdquery.xyz/)
- [Firefox Monitor](https://monitor.firefox.com/)
- [Vigilante.pw ‐ The Breached Database Directory](https://vigilante.pw/)
- **泄露密码库**
    - https://cloud.mail.ru/public/2eHX/38Ek7Lmfx?tdsourcetag=s_pctim_aiomsg
    - https://downloads.skullsecurity.org/passwords/

---

## DNS信息
- [DNS leak test](https://dnsleaktest.com/)
- [What's My DNS Server?](http://www.whatsmydnsserver.com/)

---

## 定位
**案例**
- [看我如何通过邮箱获取IP定位](http://www.freebuf.com/articles/database/185954.html)
- [社工之经度纬度定位-50米以内](https://bbs.ichunqiu.com/thread-23489-1-26.html)
- [利用Wireshark任意获取QQ好友IP实施精准定位](http://www.freebuf.com/articles/web/137952.html)
- [跨国定位手机の奥义](https://mp.weixin.qq.com/s/K-zFVBaSw6yThuoLdUTjdg)
- [For sale: Systems that can secretly track where cellphone users go around the globe - The Washington Post](https://www.washingtonpost.com/business/technology/for-sale-systems-that-can-secretly-track-where-cellphone-users-go-around-the-globe/2014/08/24/f0700e8a-f003-11e3-bf76-447a5df6411f_story.html)

**GPS 定位**
- [MyGeoPosition.com – 免费地理编译,地理译码 / 地理元数据标记 (Geo-Metatag) / 地理标记(Geotag) / KML 文件!](http://mygeoposition.com/)
- [RTBAsia ODX - Open Data Exchange](https://ip.rtbasia.com/)
- [拾取坐标系统](http://api.map.baidu.com/lbsapi/getpoint/index.html)
- [在线地图经度纬度查询 — 经纬度查询地名|地名查询经纬度 —GPSspg](http://www.gpsspg.com/maps.htm)
- [openGPS.cn](https://www.opengps.cn/)
- [经纬度查询坐标|经纬度在线查询|经纬度查询工具|经纬度位置查询|谷歌地图经纬度查询](http://www.gzhatu.com/jingweidu.html)
- [经纬度定位|经纬度定位软件|经纬度定位工具|全球卫星定位地图](http://www.gzhatu.com/dingwei.html)
- [经纬度格式转换工具软件|经纬度转换成为度分秒公式|GIS经纬度批量换算度分秒单位|经纬度转化成度](http://www.gzhatu.com/du2dfm.html)
- [经纬度在线查询,地名(批量)查询经纬度,经纬度(批量)查询地名,google map运用geocoder.geocode实例](http://map.yanue.net/)

**基站定位**
- [基站定位查询 — 移动基站联通基站电信基站 LBS —GPSspg](http://www.gpsspg.com/bs.htm)
- [免费基站定位查询--通过lac,cellid进行基站位置和手机定位查询](http://www.cellid.cn/)
- [基站查询_免费基站查询_基站定位_基站位置查询_移动联通基站_电信基站](http://www.haoservice.com/freeLocation/)
- [minigps-基站定位查询](http://www.minigps.net/cellsearch.html)

**手机号码归属地**
- [[IP138]— 138查!](http://www.ip138.com:8080/search.asp)
- [手机号码定位](http://shouji.ip38.com/)
- [手机号码查询归属地、电话号码归属地查询 — GPSspg](http://www.gpsspg.com/phone/)

**IP 信息**
- [RIPEstat — Internet Measurements and Analysis](https://stat.ripe.net/)
- [IP Info](https://ip.voidsec.com/)
- [IP/DNS Detect - What is your IP, what is your DNS, what informations you send to websites.](https://ipleak.net/)
- [ip8 - IP Lookup Tool](https://ip8.com/)
- [查看自己的IP地址](https://whoer.net/zh)
- [IPList](https://iplist.cc/)
- [ASNIP.net - ASN Query](https://asnip.net/)
- [IP Addresses - Plot IP](http://plotip.com/ip)
- [IP Geolocation API and databases - DB-IP](https://db-ip.com/)
- [IPIP.NET_最专业的 IP 地址库](https://www.ipip.net/)
- [IP查询 | 查IP地址 | ip数据库 | 手机号码归属地 | 邮政编码 | worldclock 世界时间 calendar 万年历 Google PageRank Alexa rank domain whois](http://www.123cha.com/)
- [ip查询,ip地址查询,ip位置 - Hao7188](http://www.hao7188.com/)
- [MyIP.cn - 我的IP地址查询,网站综合信息查询,域名注册信息,搜索引擎收录,Alexa排名,Google PR,Sogou PR,反向链接,百度关键字指数](http://www.myip.cn/)
- [Whois](http://ipwhois.cnnic.net.cn/)
- [国家IP段查询、全球国家IP段--查错网](http://ipblock.chacuo.net/)
- [更精准的全球IP地址定位平台_IP问问 -埃文科技(ipplus360.com)](http://www.ipplus360.com/)
- [高精度IP定位 - openGPS.cn](https://www.opengps.cn/Data/IP/LocHighAcc.aspx)
- [IP地址查询 本机IP查询 — GPSspg](http://www.gpsspg.com/ip/)
- [IP地址查询--手机号码定位 | 万年历 | 身份证号码查询](http://ip38.com/)
- [多数据源IP地址查询 - HaoIP.CN 好IP在线工具 最好的IP位置查询](https://haoip.cn/)
- [微信IP地址查询 -- 如何查微信ip地址,查微信好友ip地址](http://www.wxip.me/)
- [IP查询 - IP地址查询 - IP精确定位](http://ip.lockview.cn/Default.aspx)
- [我们知道的IP地址](http://ip.womenzhidao.com/)
- [DeerCloud/IPList: IP CIDRs List / IP 地址列表](https://github.com/DeerCloud/IPList)
- [Get your IPv4 and IPv6 address instantly](https://eyep.dev/)
- [What is my IP Address :: WebBrowserTools](https://webbrowsertools.com/ip-address/)
- [What Is My IP Address? - ifconfig.me](https://ifconfig.me/)
- [ipapi - IP Address Location](https://ipapi.co/)
- [IP Address API and Data Solutions - geolocation, company, carrier info, type and more - IPinfo.io](https://ipinfo.io/)

---

# 保护手段
**文章**
- [GoogleAlternatives - FuckOffGoogle](https://wiki.fuckoffgoogle.de/index.php?title=GoogleAlternatives)
- [安全手册:这里是你需要的几乎所有安全上网工具;以及为什么建议不要使用以美国为基地的网络服务 — Steemit](https://steemit.com/life/@iyouport/7nfymr)
- [隱私工具 - 加密安全對抗全球大規模監控](https://privacytools.twngo.xyz/)
- [No More Google](https://nomoregoogle.com/)
- [Security Checklist](https://securitycheckli.st/)
- [终极在线隐私指南](https://www.bestvpn.com/guides/the-ultimate-privacy-guide/#avoidus)
- [隐私大爆炸,你得学几招保护自己](https://evilcos.me/yinsi.html)

## 操作系统
- [Tails](https://tails.boum.org/about/index.en.html)
- [Qubes OS](https://www.qubes-os.org/)
- [Whonix](https://www.whonix.org/)

---

## 软件-脚本
- **浏览器**
    - [Eloston/ungoogled-chromium](https://github.com/Eloston/ungoogled-chromium)

- **通讯**
    - [telegram](https://telegram.org/)

- **网络审计**
    - [W10Privacy](https://www.winprivacy.de/english-home/)
    - [abcnews/data-life](https://github.com/abcnews/data-life)

- **匿名**
    - [tor](https://www.torproject.org/)
    - [i2p/i2p.i2p](https://github.com/i2p/i2p.i2p)

---

## 浏览器扩展
- **chrome**
    - [Decentraleyes](https://chrome.google.com/webstore/detail/decentraleyes/ldpochfccmkkmhdbclfhpagapcfdljkj)
    - [Cookie AutoDelete](https://chrome.google.com/webstore/detail/cookie-autodelete/fhcgjolkccmbidfldomjliifgaodjagh)
    - [LastPass Password Manager](https://chrome.google.com/webstore/detail/lastpass-free-password-ma/hdokiejnpimakedhajhdlcegeplioahd)
    - [Privacy Badger](https://chrome.google.com/webstore/detail/privacy-badger/pkehgijcmpdhfbdbbnkijodmdjhbjlgp)
    - [User-Agent Switcher for Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-for-c/djflhoibgkdhkhhcedjiklpkjnoahfmg)
    - [HTTPS Everywhere](https://chrome.google.com/webstore/detail/https-everywhere/gcbommkclmclpchllfjekcdonpmejbdp)
    - [NoScript](https://chrome.google.com/webstore/detail/noscript/doojmbjmlfjjnbmnoijecmcbfeoakpjm)
    - [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)

- **firefox🦊**
    - [Decentraleyes](https://addons.mozilla.org/en-US/firefox/addon/decentraleyes/)
    - [Cookie AutoDelete](https://addons.mozilla.org/en-US/firefox/addon/cookie-autodelete/)
    - [LastPass Password Manager](https://addons.mozilla.org/en-US/firefox/addon/lastpass-password-manager/?src=search)
    - [Privacy Badger](https://addons.mozilla.org/en-US/firefox/addon/privacy-badger17/?src=search)
    - [User-Agent Switcher and Manager](https://addons.mozilla.org/zh-CN/firefox/addon/user-agent-string-switcher/?src=search)
    - [HTTPS Everywhere](https://addons.mozilla.org/zh-CN/firefox/addon/https-everywhere/?src=search)
    - [NoScript](https://addons.mozilla.org/zh-CN/firefox/addon/noscript/?src=search)
    - [uBlock Origin](https://addons.mozilla.org/zh-CN/firefox/addon/ublock-origin/?src=search)

- **stylish**
    - ["Stylish" browser extension steals all your internet history](https://robertheaton.com/2018/07/02/stylish-browser-extension-steals-your-internet-history/)
    - [Stylus is a Stylish fork without analytics](https://www.ghacks.net/2017/05/16/stylus-is-a-stylish-fork-without-analytics/)

## 安全删除
- [如何:在Windows上安全地删除数据](https://ssd.eff.org/en/module/how-delete-your-data-securely-windows)

---

## 加密
- [VeraCrypt](https://www.veracrypt.fr/en/Home.html)
- [VHD虚拟磁盘+BitLocker加密](https://bbs.kafan.cn/thread-2115703-1-1.html)

---

## flash
`最好的选择就是远离flash`
- [支持到32_0_0_223_Adobe{过}{滤}FlashPlayer去区域限制](https://bbs.kafan.cn/thread-2123485-1-1.html)

---

## 輸入法
- [RIME](https://github.com/rime)

---

## 搜索引擎
- [DuckDuckGo — Privacy, simplified.](https://start.duckduckgo.com/)
- [searx.me](https://searx.me/)
- [StartPage Web Search](https://www.startpage.com/)

---

## 身份生成
- [Generate a Random Name](https://www.fakenamegenerator.com/)
- [Fake Address Generator All Over the World - Fake Address, Random Address Generator](https://www.fakeaddressgenerator.com/Index/index)
- [在线身份证号码生成器](http://jbjb.zouri.jp/)
- [中国大陆内地姓名、身份证号、银行卡号生成器](http://jsrun.net/square?page=1&s=%E8%BA%AB%E4%BB%BD%E8%AF%81%E5%8F%B7)
- [在线身份证号码生成器](https://id.ifreesite.com/)
- [airob0t/idcardgenerator 身份证图片生成工具](https://github.com/airob0t/idcardgenerator)
- [gh0stkey/RGPerson](https://github.com/gh0stkey/RGPerson)

---

## 邮箱-信息
### 查邮箱存活
```
http://tool.chacuo.net/mailverify
https://verify-email.org/
http://www.emailcamel.com/
```

### 短信接码

`注:此类平台来的快,去的快,慎用`
```
https://www.chenweiliang.com/cwl-558.html
https://51.ruyo.net/7789.html
https://miracletele.com/sms/
http://sms.sellaite.com/
https://catchsms.com/
https://www.freeonlinephone.org/
https://smsnumbersonline.com/
https://www.textnow.com/
https://www.receive-a-sms.com/
http://receive-sms-now.com/
https://receive-sms.com/
https://www.receive-sms-online.info/
https://sms-online.co/receive-free-sms
http://receive-sms-online.com/
http://receivefreesms.com/
https://www.receivesmsonline.net/
https://smsreceivefree.com/
https://receive-a-sms.com/
http://www.afreesms.com/freesms/
https://textfree.us/#/login
https://www.pdflibr.com/
https://sms-empfangen.com/
https://sms.cngrok.com/receiving-sms
https://yunduanxin.net/
https://shouduanxin.com/
https://www.becmd.com/
http://www.z-sms.com/
http://www.114sim.com/
https://shouduanxin.com/en/
http://www.345sms.com/
https://receiveasms.com/
https://www.gsmchecker.com/receive-sms-online
http://receivesmsverification.com/
http://smsget.net/en
https://hs3x.com/
https://www.receivesms.net/
http://receivesmsonline.com/
http://freesmsverification.com/
https://sms.ndtan.net/
https://receivefreesms.net/
http://freereceivesmsonline.com/
http://receivesmsonline.in/
https://www.visitorsms.com/
```

### 临时邮箱

`注:此类平台来的快,去的快,慎用`
```
http://www.yopmail.com/zh/
http://gfan.gvoice.men/
https://10minutemail.com/
https://10minutemail.net/
http://mail.bccto.me/
http://www.bccto.me/
https://www.guerrillamail.com/zh/inbox
http://www.fakemailgenerator.com/#/dayrep.com/Firly1970/
https://tutanota.com/
https://temp-mail.org/en/
https://www.guerrillamail.com/
http://tool.chacuo.net/mailsend
https://maildrop.cc/
https://binmail.co/home
http://tool.chacuo.net/mailanonymous
https://tempmail.altmails.com/
```

### 匿名邮箱
- [ProtonMail](https://mail.protonmail.com/inbox)
- [Openmailbox](https://www.openmailbox.org/)
- [Get secure, reliable email hosting – FastMail](https://www.fastmail.com/)
- [xyfir/ptorx](https://github.com/xyfir/ptorx)

---

## 平台管控设置

- **Microsoft**
    - [产品和服务的隐私设置,以及查看和清除 Microsoft 保存到云的数据的位置](https://account.microsoft.com/privacy/activity-history)
    - [应用授权](https://account.live.com/consent/Manage)

- **github**
    - [应用授权](https://github.com/settings/applications)

- **google**
    - [广告个性化/谷歌眼中的你](https://adssettings.google.com/authenticated)
    - [活动记录](https://myactivity.google.com/myactivity)
    - [活动控件](https://myaccount.google.com/activitycontrols?pli=1)
    - [最近使用过的设备](https://myaccount.google.com/device-activity)
    - [应用授权](https://myaccount.google.com/permissions)
    - 扩展阅读
        - [自動刪除你的 Google 網路和應用程式活動紀錄設定教學](https://free.com.tw/google-automatically-delete-data/)

- **twitter**
    - 应用授权 [旧版](https://twitter.com/settings/sessions) [新版](https://twitter.com/settings/applications)
    - [興趣和廣告資料](https://twitter.com/settings/your_twitter_data/ads)
    - [密碼重設保護](https://twitter.com/settings/security)

- **tencent**
    - [广告个性化](https://privacy.qq.com/advertisement.htm)
    - [应用授权](https://connect.qq.com/manage.html#/appauth/user)
    - 微信应用授权 [设置 - 隐私 - 授权管理]

- **baidu**
    - [应用授权](https://passport.baidu.com/accountbind?tpl=)

---

# OSINT
**相关的网站与资源**
- [丁爸网](http://dingba.top/)
- 微信公众号 情报小蜜蜂 WeChat ID little_bee007

**案例**
- [Using Flight Tracking For Geolocation – Quiztime 30th October 2019 – NixIntel](https://nixintel.info/osint/using-flight-tracking-for-geolocation-quiztime-30th-october-2019/) - 通过一张照片中的飞机轨迹寻找到目标地址的案例
- [A Guide to Open Source Intelligence (OSINT) - Columbia Journalism Review](https://www.cjr.org/tow_center_reports/guide-to-osint-and-hostile-communities.php) - 一份 OSINT 指南,汇总了很多案例
- [Intelligence Gathering on U.S. Critical Infrastructure - Industrial Control Systems (ICS) Cyber Security Conference](https://www.icscybersecurityconference.com/intelligence-gathering-on-u-s-critical-infrastructure/) - 一篇对于美国工控领域设备的 OSINT 分析文章
- [bellingcat - A Beginner's Guide To Flight Tracking - bellingcat](https://www.bellingcat.com/resources/how-tos/2019/10/15/a-beginners-guide-to-flight-tracking/) - 一篇关于追踪飞机的文章
- [如果只知道一个电话号码，你能挖出多少有效信息？](https://www.iyouport.org/%e5%a6%82%e6%9e%9c%e5%8f%aa%e7%9f%a5%e9%81%93%e4%b8%80%e4%b8%aa%e7%94%b5%e8%af%9d%e5%8f%b7%e7%a0%81%ef%bc%8c%e4%bd%a0%e8%83%bd%e6%8c%96%e5%87%ba%e5%a4%9a%e5%b0%91%e6%9c%89%e6%95%88%e4%bf%a1%e6%81%af/)

**在线全能工具**
- https://intelx.io/tools

## 设备-语音助手
- **Alexa**
    - [除非手动删除,不然 Alexa 上的语音资料会被亚马逊一直保留](https://cn.engadget.com/2019/07/04/amazon-keeps-alexa-transcripts/)
    - [隔屏有耳调查｜亚马逊智能音箱有千人监听团队,曾听到性侵案](https://www.thepaper.cn/newsDetail_forward_3290014)
    - [亚马逊提供 Alexa 录音的非人工审听选项](https://www.solidot.org/story?sid=61594)

- **Cortana**
    - [继苹果谷歌后:微软被曝监听用户Skype和Cortana录音](https://tech.sina.com.cn/i/2019-08-08/doc-ihytcitm7662431.shtml)
    - [Revealed: Microsoft Contractors Are Listening to Some Skype Calls](https://www.vice.com/en_us/article/xweqbq/microsoft-contractors-listen-to-skype-calls)
    - [微软被指使用廉价合同工完成Cortana语音收听工作](https://www.cnbeta.com/articles/tech/879681.htm)
    - [微软:暂不会停止对 Skype 和 Cortana 对话的人工审查](http://hackernews.cc/archives/26954)

- **Google Home**
    - [谷歌承认通过语音助手收集用户谈话内容:仅用于开发](https://www.ithome.com/0/433/712.htm)
    - [Google admits workers listen to some smart device recordings](https://thehill.com/policy/technology/452620-google-admits-workers-listen-to-some-smart-device-recordings)

- **HP printers**
    - [惠普打印机被发现偷偷回传数据:隐藏极深](https://tech.ifeng.com/c/7q1bbVclnyh)
    - [HP printers try to send data back to HP about your devices and what you print](https://robertheaton.com/2019/09/15/hp-printers-send-data-on-what-you-print-back-to-hp/)

- **Siri**
    - [Siri被曝偷偷给用户隐私录音,还上传给苹果](https://www.ednchina.com/news/201907291202.html)
    - [苹果回应Siri录音用户谈话内容:使用了1%的用户录音](https://www.pingwest.com/w/191896)
    - [Siri 人工评估计划的员工说,自己每天要听 1000 条录音](https://www.ifanr.com/1251668)
    - [Apple to stop default practice of keeping Siri recordings](https://www.reuters.com/article/us-apple-privacy-siri/apple-says-to-restart-siri-reviews-with-new-controls-idUSKCN1VI1X3)

- **Misc**
    - [卖二手设备一定要注意,你的信息可能并没被删除](http://www.mottoin.com/detail/3933.html)

    - ![image](./assets/img/手机取证.jpg)

- **MIUI**
    - [1000字够不够？小米MIUI 10去广告教程](https://zhuanlan.zhihu.com/p/58415240)
    - [How to disable most push advertisement on MIUI China Version](https://telegra.ph/How-to-disable-most-push-advertisement-on-MIUI-China-Version-02-01)
    - 在「设置-小米账号-隐私协议等-系统广告」里关闭广告.
    ![image](./assets/img/xiaomiad.png)

- **ios**

    设置-->隐私-->定位服务-->系统服务-->重要地点

---

## 平台-软件
- **Airbnb**
    - [Airbnb上的OSINT信息收集](https://mp.weixin.qq.com/s/J8J6atXxhG4kqtXsG_9odw)

    ---

    - [I Accidentally Uncovered a Nationwide Scam on Airbnb](https://www.vice.com/en_us/article/43k7z3/nationwide-fake-host-scam-on-airbnb) - 一篇描述关于Airbnb上诈骗状况的文章,揭露了如今人们在 Airbnb 上被骗的种种方式

- **Chrome**
    - [谷歌崩溃报告究竟收集了哪些信息 个人信息如何处置](https://www.cnbeta.com/articles/tech/873763.htm)
    - [用户浏览器被互联网大厂私自[托管]？仔细一查,这事并不简单](https://www.ithome.com/0/437/940.htm)

    ---

    **隐身模式**
    - [Bypassing anti-incognito detection in Google Chrome](https://mishravikas.com/articles/2019-07/bypassing-anti-incognito-detection-google-chrome.html)
    - [Google Chrome Incognito Mode Can Still Be Detected by These Methods](https://www.bleepingcomputer.com/news/google/google-chrome-incognito-mode-can-still-be-detected-by-these-methods/)

- **EDGE**
    - [UWP版EDGE浏览器被发现将用户安全标识符和网址发送给微软分析](https://www.landiannews.com/archives/61675.html)
    - [Edge被吐槽向微软发送包含用户SID和访问站点完整URL等在内的信息](https://www.cnbeta.com/articles/tech/870695.htm)

- **facebook**
    - [facebook正在你下载的照片中嵌入跟踪数据](https://twitter.com/oasace/status/1149181539000864769)
    - [Facebook Embeds 'Hidden Codes' To Track Who Sees And Shares Your Photos](https://www.forbes.com/sites/zakdoffman/2019/07/14/facebook-is-embedding-hidden-codes-to-track-all-your-uploaded-photos-report/#736d099e1592)

    ---

    知情人士透露称,Facebook付费聘请几百名外部承包商,让他们转录音频片段,这些音频来自使用Facebook服务的用户.

    - [Messenger 发音频安全吗？FB 承认曾转录用户音频](http://hackernews.cc/archives/26923)
    - [彭博:Facebook雇人记录用户语音通话以改善AI技术](https://tech.sina.com.cn/i/2019-08-14/doc-ihytcitm8999002.shtml)

    ---

    - [harismuneer/Ultimate-Facebook-Scraper](https://github.com/harismuneer/Ultimate-Facebook-Scraper) - 一个抓取 facebook 用户信息的 python 脚本

- **firefox**
    - [Firefox火狐国际版和中文版的区别](http://www.177kan.com/html/2017033130.html)
    - [Firefox 如何查看和切换 本地服务 与 全球服务](http://mozilla.com.cn/forum.php?mod=viewthread&tid=330960)

- **google**
    - [Google accused of leaking personal data to thousands of advertisers](https://www.zdnet.com/article/google-accused-of-leaking-personal-data-to-thousands-of-advertisers/)

- **Instagram**
    - [Find an Instagram user ID](https://www.aware-online.com/en/find-an-instagram-user-id/) - 检索 Instagram 用户 ID

    ---

    - [sc1341/InstagramOSINT](https://github.com/sc1341/InstagramOSINT) - 对 Instagram 帐户进行基本的信息收集的 python 脚本.

- **kaspersky**

    安全研究人员在测试卡巴斯基杀毒软件时发现它会以安全的名义在用户访问的每一个网页注入它的脚本,而这个脚本还带有唯一ID,这个ID在不同计算机上是不同的,也就是说它可以作为跟踪代码使用.研究人员将这一发现报告给了卡巴斯基.卡巴斯基承认了数据泄漏,它释出了补丁修复了编号为CVE-2019-8286的问题.这个补丁去除了唯一ID,留下了相同的ID,也就是说网站仍然会知道有安装了卡巴斯基软件的用户访问了.
    - [卡巴斯基修复四年老漏洞 注入 HTML 源码的唯一标识符会泄露用户隐私](http://hackernews.cc/archives/26982)
    - [Unique Kaspersky AV User ID Allowed 3rd-Party Web Tracking](https://www.bleepingcomputer.com/news/security/unique-kaspersky-av-user-id-allowed-3rd-party-web-tracking/)

- **Netflix**
    - [Netflix 解释他们追踪用户活动数据的原因](https://cn.engadget.com/2019/08/01/netflix-physical-activity-android-test/)

- **Office 365**
    - [Office 365的Webmail在电子邮件中显示用户的IP地址](https://www.bleepingcomputer.com/news/microsoft/microsoft-office-365-webmail-exposes-users-ip-address-in-emails/)

- **Opera**

    Brave 的 Jonathan Sampson 在 Twitter 上发表了一系列帖子,他在 Windows 机器上第一次安装了 Google Chrome、Microsoft Edge (Chromium) Beta、Opera 和 Vivaldi 、Dissenter、Brave 和 Firefox,每个浏览器在安装之后都打开几分钟,期间他会对浏览器发出的请求进行抓包,对抓包结果进行一番分析.他发现 Brave 会发出 23 个请求,访问的都是 Brave.com 域名;Firefox 会发出 26 个请求,部分与 Google 的服务有关;Edge 会发出超过 130 个请求,有微软的还有 Google、Facebook 和 Twitter 的,Edge 在首次运行之后还收集了用户系统的详细信息;Opera 发出的请求有些特别,它有 19 个请求指向了俄罗斯的 yandex.ru,还有亚马逊、ebay 和阿里巴巴,它还预加载了十多个第三方网站的 cookies,它甚至已经开始与第三方共享用户信息,许多人声称这家中国公司拥有的挪威浏览器已经变成了间谍软件.
    - [第一次启动 Google Chrome 会发生什么？](https://www.solidot.org/story?sid=61874)

- **QQ**
    - [我根据QQ步数判断出我男朋友和我朋友出轨了](https://www.douban.com/group/topic/145419238/)

    **查看历史头像**

    貌似只有 QQ 可以,TIM 不行

    <p align="center">
        <img src=".//assets/img/qq.jpg">
    </p>

- **Skype**
    - [当Skype翻译器功能处于活动状态时 微软承包商可以获知对话内容](https://www.cnbeta.com/articles/tech/876211.htm)

- **telegram**

    这些网站可以分析出来聊天情况,活跃情况.
    - [Combot](https://combot.org/)
    - [tele.me: the front page of Telegram communities](https://tele.me/)

    ---

    频道索引
    - [Largest catalog of Telegram channels. Statistics, analytics, TOP chart. Telegram Analytics.](https://tgstat.com/)

    ---

    **Telegram 账号的"数字 id"是注册时间越晚就越大吗？**

    不是.如果多注册一些账号,可以发现有可能后注册的账号数字 id 是要小于先期注册的,因此通过数字 id 来判断一个账号是否为新号是没有依据的.出现这种现象,应该是由于旧账号注销后,该账号的数字 id 又被重新分配给新注册的账号.Telegram 官方客户端无法显示账号数字 id,若想查询自己的账号数字id可以用过机器人 @getidsbot ,还有其他的机器人也有类似的功能,某些第三方客户端也可以显示账号的数字id(请谨慎使用第三方客户端).

- **Twitter**
    - [Twitter承认未经允许将用户数据与广告商共享](https://www.cnbeta.com/articles/tech/877047.htm)

    ---

    - [从推特中挖掘真相不需要太复杂的工具：一个常用工具的全面指南](https://www.iyouport.org/%e4%bb%8e%e6%8e%a8%e7%89%b9%e4%b8%ad%e6%8c%96%e6%8e%98%e7%9c%9f%e7%9b%b8%e4%b8%8d%e9%9c%80%e8%a6%81%e5%a4%aa%e5%a4%8d%e6%9d%82%e7%9a%84%e5%b7%a5%e5%85%b7%ef%bc%9a%e4%b8%80%e4%b8%aa%e5%b8%b8%e7%94%a8/)

    ---

    - [twintproject/twint](https://github.com/twintproject/twint) - 使用 Python 编写,抓取 Twitter 的 OSINT 工具.

- **youtube**
    - [YouTube DataViewer](https://intelx.io/tools?tab=youtube) - 显示YouTube上任意视频的所有可用元数据。
    - [anvaka/yasiv-youtube](https://github.com/anvaka/yasiv-youtube) - 寻找相似视频关系

- **百度云**

    说不定某时某人就给你开了个自动备份呢？

    https://pan.baidu.com/disk/discovery

    <p align="center">
        <img src=".//assets/img/baiduyun.png">
    </p>

- **滴滴**

    我没下过 APP 版的,在支付宝中的滴滴是可以查询历史行程的.点击头像-->订单-->查看历史行程

    <p align="center">
        <img src=".//assets/img/dd.png">
    </p>

- **淘宝**

    **查看历史消费金额**

    `淘宝搜索 : 淘宝人生 点右上角[成就]`

    `淘宝搜索 : 看鬼故事`

- **网易云**

    **指纹**

    试着分享一个音乐 https://music.163.com/#/song/1346907833/?userid=48353

    注意一下 userid 变量,构造一下链接: `https://music.163.com/#/user/home?id=<!userid!>`

    `https://music.163.com/#/user/home?id=48353`

    ---

    **历史评论**

    ios 端、安卓端通用,账号-->关于我-->我的评论

- **微博**

    **微博图片反查**
    - https://wbimg.huyuaning.com/
    - http://tool.uixsj.cn/weibo-pic-check/

- **微信**

    阅读下面这个文章大致了解一下微信链接组成

    - [解读微信公众平台图文消息的链接组成](https://chuansongme.com/n/676997)

    那么类似 `https://mp.weixin.qq.com/s?__biz=MzIyAAANzY0OA==&mid=101111431&idx=1&sn=62accd1299d25d54d1f3ad3f3d7d214&chksm=683d2e402f6sa2dsa2d154058807d1xxxx151213131dasdasdsadasd675ce59fae94ff9908&scene=18&xtrack=1&key=917D458AS46D146SD14AF541DSA4FDSAF131DS31F31DSA31FDSAde153285841fdc398a67d61be441cb0e1898a08232811308bf31dfc92757c3d7d5e3SD54AD1SA1D351S3A1D31S3AD034f1cb34170ecd27b6d7d69&ascene=1&uin=MTk3ODkwODMxMA%3D%3D&devicetype=Windows+7&version=62055833&lang=zh_CN&pass_ticket=r6jSAD55SAF458F61A4S56F51BW2hfIQPocX2O0er0vUheGSD45ASD11DASD361SADAWDbiqW` 这么一串可以携带多少信息

    ---

    下面为阿里巴巴旗下的南华早报引用加拿大多伦多大学公民实验室的报告报道,腾讯的微信利用实时和追溯分析的方法审查用户的图片.报告发现,微信对用户对话中发送的图片进行实时自动检测和审查,审查是基于图片中包含的文字以及目标图片与系统数据库中的敏感图片的相似度匹配;微信通过建立哈希索引(Hash Index)实现过滤,该哈希索引由微信用户在聊天对话中发送的图像的 MD5 值组成;对比微信朋友圈,一对一聊天以及群组聊天的图片审查比例,发现这三项功能的敏感图片库并不相同,其中朋友圈和群组聊天所审查的范围要远大于一对一聊天;与关键词审查一样,微信图片审查与新闻事件相关.

    - [How unwitting users of WeChat aid the Chinese messaging app’s blacklisting of sensitive images](https://www.scmp.com/news/china/politics/article/3018725/how-unwitting-users-wechat-aid-chinese-messaging-apps)

- **支付宝**

    - [支fu宝可以查婚姻状况望周知](https://www.douban.com/group/topic/142322388/)

---

## 敏感信息
### EXIF信息
- [EXIF信息查看器](https://exif.tuchong.com/)
- [ExifShot App](https://exifshot.com/app/)
- [如何为老照片添加 Exif 日期数据？ - 小众软件](https://www.appinn.com/how-to-add-exif-date-for-old-picture/)

**文章**
- [Explainer: how law enforcement decodes your photos](http://theconversation.com/explainer-how-law-enforcement-decodes-your-photos-78828) - 作者描述了关于数字调查者如何拆解数码照片，寻找关于制造和模型线索的过程。

---

## 各类搜索

`下方所有搜索引擎不保证其安全性、隐私性,仅保证其功能性`

### 常用搜索引擎
- https://www.ask.com/
- https://start.duckduckgo.com/
- https://www.ecosia.org/
- https://www.google.com/
- https://www.qwant.com/
- https://so.mezw.com/
- https://searx.me/
- https://www.startpage.com/
- https://yandex.com/
- http://search.chongbuluo.com/
- http://www.subzin.com/
- https://magi.com/

### 航班
- [Flight Tracker | Flightradar24 | Track Planes In Real-Time](https://www.flightradar24.com/)
- [FlightAware - 航班跟踪/航班状态/飞行跟踪](https://zh.flightaware.com/)
- [Flightradar24 — how it works? / Habr](https://habr.com/en/post/440596/)
- [real-time flight tracking | Flightadsb | VariFlight](http://flightadsb.variflight.com/)
- [Direct Flights | Explore all non-stop flights from any airport](https://direct-flights.com/)

### 船舶
- [MarineTraffic: Global Ship Tracking Intelligence | AIS Marine Traffic](https://www.marinetraffic.com/)
- [Free AIS Ship Tracking of Marine Traffic - VesselFinder](https://www.vesselfinder.com/)
- [My Ship Tracking Free Realtime AIS Vessel Tracking Vessels Finder Map](https://www.myshiptracking.com/)
- [船舶动态查询_AIS船位_船舶跟踪_船舶定位_船舶位置查询-ShipTracker](http://www.chinaports.com/shiptracker/olv3/index.jsp)
- [Global Container Shipping Platform | Container Tracking, Ocean Schedules](https://shipsgo.com/)
- [Marine Vessel Traffic](https://www.marinevesseltraffic.com/)
- [Live AIS Ships Map!---shipfinder](http://www.shipfinder.com/)
- [船员证书查询](http://cyxx.msa.gov.cn/lycx/zslycx!init.action?flag=1)
- [船舶查询系统,全球最大的船舶数据库](http://app.cnss.com.cn/sochuan.php)

### 可信度
- [个人信用查询搜索_企业信息查询搜索_统一社会信用代码查询-信用中国](https://www.creditchina.gov.cn/)
- [统一社会信用代码查询_诚信体系实名制查询_组织机构代码-全国组织机构统一社会信用代码数据服务中心(原全国组织机构代码管理中心)](https://www.cods.org.cn/)
- **个人**
    - [中国执行信息公开网](http://zxgk.court.gov.cn/)
    - [银行卡号归属地查询-银行卡开户行查询-银行卡信息查询-银行卡号网-诈骗举报](http://www.2cha.com/)
    - [中国人民银行征信中心](http://www.pbccrc.org.cn/)
    - [个人与企业信息查询|失信被执行人查询|税务信息查询|行政处罚|法院判决|查公司|风险管理系统-风险信息网](https://www.lawxin.com/) - 可查询个人和企业工商信息以及法院判决、税务、海关、市场监管等各类关联信息。并且支持批量监控，并有短信通知功能。
    - [查企业工商_诉讼案件_失信被执行人_对外投资_催收公告信息_风险预警网](https://www.fengxian110.com/) - 被列入失信执行人的名单将在网站上展示。
    - [物业费催收|互联网催收平台|贷后催收系统|债务案源-催天下](https://www.cuitx.cn/) - 可以查询被催收人信息
    - [汇法网-网上法务平台：找律师、裁判文书、法律法规、合同、法律新闻](https://www.lawxp.com/) - 提供法律法规及裁判文书查询

- **企业**
    - [企查查_工商信息查询_公司企业注册信息查询_全国企业信用信息公示系统](https://www.qichacha.com/)
    - [国家企业信用信息公示系统](http://www.gsxt.gov.cn/index.html)
    - [天眼查-人人都在用企业信息调查工具_企业信息查询_公司查询_工商查询_信用查询平台](https://www.tianyancha.com/)
    - [启信宝-企业注册信息查询|企业工商信息查询|企业信用信息查询平台](https://www.qixin.com/)
    - [企业信用信息查询](http://www.ixy360.com/)
    - [悉知 - 专注企业信息查询 | 查企业 用悉知](http://www.xizhi.com/)
    - [信用视界-专业的企业信息查询_公司查询_企业信用信息查询_企业工商信息查询_企业注册信息查询_工商登记信息查询_征信公司](https://www.x315.com/)
    - [中国海关企业进出口信用信息公示平台](http://credit.customs.gov.cn/)
    - [看准网-查工资|聊面试|评公司|搜职位|中国领先的职场信息平台](https://www.kanzhun.com/)
    - [Crunchbase: Discover innovative companies and the people behind them](https://www.crunchbase.com/)

### 搜图
- [Google 图片](https://www.google.com/imghp)
- [Jeffrey Friedl's Image Metadata Viewer](http://exif.regex.info/exif.cgi)
- [TinEye Reverse Image Search](https://www.tineye.com/)
- [百度识图, "鉴"你所见](https://image.baidu.com/fr=shitu)
- [Google Art & Culture Experiment - Art Palette](https://artsexperiments.withgoogle.com/artpalette/)
- [Yandex.Images: search for images on the internet, search by image](https://yandex.com/images/)

#### acg
- [Multi-service image search](https://iqdb.org/)
- [SauceNAO Image Search](https://saucenao.com/)
- [二次元画像詳細検索](https://ascii2d.net/)
- [WAIT: What Anime Is This? - Anime Scene Search Engine](https://trace.moe/)

### hack
- [Censys](https://censys.io/)
- [DNSDB](https://www.dnsdb.io/zh-cn/)
- [FOFA Pro - 网络空间安全搜索引擎,网络空间搜索引擎,网络空间测绘,安全态势感知](https://fofa.so/)
- [Punk.sh](https://punk.sh/#/)
- [Shodan](https://www.shodan.io/)
- [ZoomEye - Cyberspace Search Engine](https://www.zoomeye.org/)
- [CertDB — SSL certificates search engine](https://certdb.com/)
- [searchcode | source code search engine](https://searchcode.com/)

#### wooyun
- https://bugs.shuimugan.com/
- https://www.secpulse.com/archives/category/vul
- https://github.com/hanc00l/wooyun_public
- https://drops.tuisec.win/
- http://wooyun.jozxing.cc/
- http://drops.xmd5.com/
- http://www.anquan.us/
- http://wy.zone.ci/index.php
- https://shuimugan.com/
- https://wooyun.js.org/
- http://drop.zone.ci/

### 学术
- [libgen](https://libgen.pw/)
- [Library Genesis](http://libgen.io/)
- [Semantic Scholar - An academic search engine for scientific articles](https://www.semanticscholar.org/)
- [远见搜索—站得更高,看得更远!](https://yuanjian.cnki.net/)

### 物流
- [快递100-查快递,寄快递,上快递100](http://www.kuaidi100.com/)
- [http://www.56888.net/comm/kuaidi.aspx](http://www.56888.net/comm/kuaidi.aspx)
- [中华人民共和国国家邮政局](http://www.spb.gov.cn/yzbmcx/)
- [快递查询_快递单号查询_查快递CKD.CN](http://www.ckd.cn/)
- [中华人民共和国国家邮政局](http://www.spb.gov.cn/yzbmcx/#)
- [全球物流查询平台 | 17TRACK](https://www.17track.net/zh-cn)

### 专利-商标
- [佰腾网](https://www.patexplorer.com/)
- [Dawei Innojoy Patent Search Engine](http://www.innojoy.com/search/index.html)
- [SooPAT 专利搜索](http://www1.soopat.com/Home/IIndex)
- [润桐RainPat专利检索---免费,绝对免费,永久免费](https://www.rainpat.com/)
- [专利信息服务平台](http://search.cnipr.com/)
- [权查查-商标查询-商标注册-商标监控-商标品牌保护-知识产权服务平台](https://www.qccip.com/)

### 报刊
- [梅子搜报网](http://mz.soubao.net/#/meizi/searchIndex)

### 图表
- [Grafiti | The Search Engine for Charts](https://beta.grafiti.io/)

### 数据
- [World Bank Open Data](https://data.worldbank.org.cn/)

### BGP
- [BGP Update Reports](http://bgp.potaroo.net/index-upd.html)
- [Collectors – Routeviews](http://www.routeviews.org/routeviews/index.php/collectors/)
- [Hurricane Electric BGP Toolkit](https://bgp.he.net/)

### 电子硬件相关
- [Search FCC ID Database](https://fccid.io/search.php)
- [BIOS Master Password Generator for Laptops](https://bios-pw.org/#)
- [无线电设备查询](http://www.srrc.org.cn/WP_Search.aspx)

### 快照
- [搜索引擎网页快照查询，支持手机移动端-网页快照网](http://2tool.top/)
- [Internet Archive: Digital Library of Free & Borrowable Books, Movies, Music & Wayback Machine](https://archive.org/)

### 社交-人际关系
- [Golgozar - Social Search Engine](https://www.golgozar.org/index.php)
- [Discover your ancestors - Genes Reunited](https://www.genesreunited.co.uk/)

---

## 天气-环境
- [Antiweather](https://bennettfeely.com/antiweather/)
- [亚洲空气污染:实时空气质量指数地图](https://aqicn.org/map/cn/)
- [earth :: a global map of wind, weather, and ocean conditions](https://earth.nullschool.net/)
- [Windy: Wind map & weather forecast](https://www.windy.com/)
- [台风路径实时发布系统](http://typhoon.zjwater.gov.cn/default.aspx)
- [Light pollution map](https://www.lightpollutionmap.info/)
- [PurpleAir | Real Time Air Quality Monitoring](https://www2.purpleair.com/)

---

## 地图
- [天地图](http://map.tianditu.gov.cn/)
- [高德地图](https://www.amap.com/)
- [百度地图](https://map.baidu.com/)
- [Bing 地图](https://cn.bing.com/ditu/)
- [Google Maps](https://www.google.cn/maps/)
- [Google Earth](https://www.google.com/earth/)
- [OpenStreetMap](https://www.openstreetmap.org/)
- [MapBoard](https://board.mapdevcode.co/)
- [HE 3D Network Map](https://he.net/3d-map/)
- [日本夜遊地圖 Japan Night Life - uMap](https://umap.openstreetmap.fr/zh-tw/map/japan-night-life_245233#6/37.892/140.361)
- [EarthExplorer](https://earthexplorer.usgs.gov/)
- [Submarine Cable Map](https://www.submarinecablemap.com/)
- [Mapped: The world's nuclear power plants | Carbon Brief](https://www.carbonbrief.org/mapped-the-worlds-nuclear-power-plants)
- [发现中国 - 地图分享知识](https://www.ageeye.cn/)

### 网络攻击地图

`偷偷告诉你,这里面,好几个,都是假的`

- [Fortinet Threat Map](https://threatmap.fortiguard.com/)
- [Live Cyber Attack Threat Map | Check Point Software](https://threatmap.checkpoint.com/ThreatPortal/livemap.html)
- [FireEye Cyber Threat Map](https://www.fireeye.com/cyber-map/threat-map.html)
- [BOTNET Connection Dashboard](https://botnet-cd.trendmicro.com/)
- [实时互联网监控器 | Akamai CN](https://www.akamai.com/cn/zh/resources/visualizing-akamai/real-time-web-monitor.jsp?tab=traffic&theme=dark)
- [MAP | Kaspersky Cyberthreat real-time map](https://cybermap.kaspersky.com/)
- [Digital Attack Map](https://www.digitalattackmap.com/)
