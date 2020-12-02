1、本文是一个小白对于科学上网的一些切身感受的整理，自己捋思路，同时也为方便他人。顺便会不断更新一些实用资源、工具等。发现错误的地方欢迎斧正。<br>
2、点击目录会跳转到相应内容，正文中点标题也可快速返回目录位置。点“回到顶部”快速回到文章开头<br>
3、`2020.8.9在实用工具iOS+Mac模块增加号称iOS上永久免费的VPN工具`<br>
`2020.8.11增加了对IPLC、IEPL的通俗理解和客观看待机场跑路及翻墙安全问题`
* <a id="h1" href="#c1">一、国内网络基本了解 </a> <br>
* <a id="h2" href="#c2">二、科学上网 </a> <br>
  * <a id="h2.1" href="#c2.1">No1、没落的“VPN” </a> <br>
    * <a id="h2.1.1" href="#c2.1.1">什么是VPN </a>
    * <a id="h2.1.2" href="#c2.1.2">VPN现状 </a>
  * <a id="h2.2" href="#c2.2">No2、关于机场 </a> <br>
    * <a id="h2.2.1" href="#c2.2.1">什么是机场 </a>
    * <a id="h2.2.2" href="#c2.2.2">机场的选择 </a>
      * <a id="h2.2.2.1" href="#c2.2.2.1">技术层面 </a>
        * <a id="h2.2.2.1.1" href="#c2.2.2.1.1">BGP中转和IPLC、IEPL的通俗理解 </a>
      * <a id="h2.2.2.2" href="#c2.2.2.2">主观层面 </a> 
        * <a id="h2.2.2.2.1" href="#c2.2.2.2.1">机场的外观设计 </a> 
        * <a id="h2.2.2.2.2" href="#c2.2.2.2.2">机场电报群观察交流 </a>
        * <a id="h2.2.2.2.3" href="#c2.2.2.2.3">机场的测速 </a>
        * <a id="h2.2.2.2.4" href="#c2.2.2.2.4">机场价格 </a>
    * <a id="h2.2.3" href="#c2.2.3">客观看待机场跑路及翻墙安全问题 </a>
* <a id="h3" href="#c3">三、我的机场及使用感受 </a> <br>
  * <a id="h3.1" href="#c3.1">SSR、V2ray机场：STC </a> <br>
  * <a id="h3.2" href="#c3.2">Trojan机场 </a> <br>
  * <a id="h3.3" href="#c3.3">机场综合使用感受 </a> <br>
* <a id="h4" href="#c4">四、主流科学上网工具下载(包含Win、Mac、Android三大平台) </a> <br>
  * <a id="h4.1" href="#c4.1">V2ray(含官方使用手册) </a> <br>
  * <a id="h4.2" href="#c4.2">clash(含CFW使用说明书) </a> <br>
    * <a id="h4.2.1" href="#c4.2">ClashR汉化版，支持SSR和V2订阅 </a> <br>
  * <a id="h4.3" href="#c4.3">Trojan </a> <br> 
  * <a id="h4.4" href="#c4.4">SSTAP </a> <br>
  * <a id="h4.5" href="#c4.5">Netch(Win) </a> <br>
  * <a id="h4.6" href="#c4.6">Mellow </a> <br>
  * <a id="h4.7" href="#c4.7">Pharos Pro(Android) </a> <br>
  * <a id="h4.8" href="#c4.8">shadowrocket基础教程及分组规则自动切换节点 </a> <br>
  * <a id="h4.9" href="#c4.9">Shadowsocks </a> <br>
  * <a id="h4.10" href="#c4.10">ShadowsocksR </a> <br>
* <a id="h5" href="#c5">五、其它实用资源、工具 </a> <br>  
 
***

# <a id="c1" href="#h1">一、国内网络基本了解 </a> <br>
大家都知道，我们中国对网络的限制比较严格，不是所有的网站咱们都能浏览。国家主要通过GFW([dns劫持](https://baike.baidu.com/item/%E5%9F%9F%E5%90%8D%E5%8A%AB%E6%8C%81/7657893?fromtitle=DNS%E5%8A%AB%E6%8C%81&fromid=6739044&fr=aladdin)、[dns污染](https://baike.baidu.com/item/DNS%E6%B1%A1%E6%9F%93)和[ip封锁](https://baike.baidu.com/item/ip%E5%B0%81%E9%94%81)等手段)进行网络封锁。下图是百度百科对GFW（俗称“墙”）的介绍
![GFW](https://www.louimg.com/u/20200312/11050110.png "GFW的介绍")
大家主要看红圈里的文字，GFW的功劳：让国民政治觉悟提升了不少，所以GFW只会越来越完善。但对于大多数网民来说，网络是我们学习、工作、美好生活的重要工具，GFW一定程度上把好多对我们学习、工作有帮助的综合性很强的技术、学术网站、社交网站等也拒之门外。
<br>大家经常听说的网站如[油管YouTube](https://www.youtube.com)、[脸书Facebook](https://www.facebook.com/)、[推特Twitter](https://twitter.com)、[电报telegram](https://telegram.org/)、[谷歌google](https://www.google.com.hk/)、[维基百科](https://zh.wikipedia.org/)等，这些我们都是无法正常访问的。需要科学上网（俗称翻墙）才能上。所以，这种背景下，也就出现了各种各样的突破GFW限制的工具，突破网络审查的软件通常被称作翻墙软件，俗称梯子。翻墙软件并不只是大家理解的VPN软件，还有基于其它协议的代理软件。<br>[回到顶部](#readme)
***
# <a id="c2" href="#h2">二、科学上网 </a> <br>
## <a id="c2.1" href="#h2.1">1、没落的“VPN” </a> <br>
### <a id="c2.1.1" href="#h2.1.1">1.1、什么是VPN </a> <br>
VPN全称“虚拟私人网络（Virtual Private Network）”，VPN是一个统称。VPN是一种加密通讯技术，它被设计出来的目的是数据传输安全和网络匿名。所以它不是为了翻墙而生的，维基百科里关于VPN的介绍，说它的特殊使用才是翻墙。它的出现远早于GFW。
![VPN](https://www.louimg.com/u/20200312/15453995.png "VPN的维基介绍")
GFW机制加上劳动人民的无穷智慧，促使聪慧的劳动人民开始用VPN连接外国网络实现翻墙，随着使用人数的激增和网络环境的发展，商业化的一键VPN也逐渐成熟，一些免费VPN和付费VPN就这样诞生了。<br>[回到顶部](#readme)
### <a id="c2.1.2" href="#h2.1.2">1.2、VPN现状 </a> <br>
使用VPN，不足之处在于数据分流不灵活，会将开启了VPN的设备的所有数据流量全部导向至VPN服务器上；另外如果VPN服务器上有流量监视软件运行，那么用户所传输的数据将有信息安全威胁；进一步来说，由于VPN设计的初衷并不是用于翻墙，因此数据流量的特征非常明显，容易引起审查机构注意，导致被封。所以，VPN这种翻墙方式基本已经没落了。但是市场上还是有一些一键VPN软件，它们背后的原理其实已经背离了VPN的真正原理，这些一键VPN其实就是把一些机场节点融合到了自己的APP，所以现在好多得VPN其实也不算真正的VPN了。至于免费的VPN，由于用户人数与流量众多，常会暴露出了公共网络服务的特质，所以经常会被封，而且VPN也存在后台钓鱼的风险，虽然可能现在这种情况好多了（谁知道呢），但是之前毕竟存在过，所以本人主观上严重不建议长期使用这种一键VPN软件。<br>
VPN作为过去很长一段时间最主流最热门最常用最为人所知的翻墙手段，已然成为翻墙的代名词。即便是VPN已不再常用的今天，当人们谈及翻墙的时候，说得最多的仍是：“你有什么好用的vpn吗？”<br>
[回到顶部](#readme)<br>
***
## <a id="c2.2" href="#h2.2">2、关于机场</a> <br>
### <a id="c2.2.1" href="#h2.2.1">2.1、什么是机场</a> <br>
随着VPN的没落，现在主流的科学上网方式是大家经常听的SS（Shadowsocks）、ssr（ShadowsocksR）、V2(v2ray)、Trojan等等这些代理工具，还有基于这些代理工具的原理，扩展衍生出的在各平台使用且支持以上几种翻墙协议的科学上网工具，如clash、Netch、shadowrocket、Quantumult、Pharos Pro等等非常多。<br>
这些工具的统一特点就是：工具自身没有翻墙功能，需要自行在服务端和客户端上部署，优点就是更加安全、速度更快，看似比一键VPN方法“繁琐”，但实际操作非常简单，其中服务端的部署有两种情况：<br>
第一种是我们自己购买vps部署，这就是人们常说的我自己搭建节点，喜欢折腾的伙伴可以自己去购买vps搭建，网上教程非常多，我自己是在谷歌云搭建了Trojan服务，具体教程本文第五部分有。<br>
第二种，就是有人替我们部署好了，直接用就可以。这也是目前用的最多的科学上网方式，提供这项服务的就是[机场](https://123321.com/auth/register?code=9JIx)。<br>
服务端部署好后，我们只需将服务器地址、端口这些基本信息添加到我们电脑或手机上的代理工具里，这就是客户端部署，这就实现了科学上网。现在很多工具都支持一键订阅，多数机场也提供了订阅链接，不需要我们手动逐一添加节点。<br>[回到顶部](#readme) 
### <a id="c2.2.2" href="#h2.2.2">2.2、机场的选择 </a> <br>
#### <a id="c2.2.2.1" href="#h2.2.2.1">2.2.1、技术层面 </a> <br>
##### <a id="c2.2.2.1.1" href="#h2.2.2.1.1">BGP中转和IPLC、IEPL的通俗理解 </a> <br>
大家在购买机场时候，会经常见到BGP中转、IPLC、IEPL专线这些名词。至于他们的专业意义，自行google查询。对于很多不是专业研究这个的伙伴，就算我们查询了，也可能是似懂非懂的状态，所以这里不会给大家去深挖那些专业概念，我们尽量从小白角度出发，明白他们的所起的作用就行。<br>
首先，我们要了解的就是我们的电脑、手机通过机场翻墙，数据经历了一个什么过程，大致有以下几种类型（从专业角度讲，有些地方可能不是很恰当，但很形象）：
* 直连<br>
  * 用户 -> ss、ssr等协议 -> 公网传输穿过GFW -> 国外服务器<br>
大多数机场节点都是这种，尤其是一些免费节点。此方式成本低，因为是协议直接过GFW，虽然协议本身也做了技术处理，但大流量还是很容易被GFW识别，这也就是为什么有的机场节点经常会出现不稳定现象，或者干脆就被封不能用了。而且公网传输，使用人多，流量拥挤就会速度变慢。<br>
好点的机场主可能会单独购买一条线路，这也就是我们说的独享线路机场，速度还稍微快点。有些功利性的机场主会租一条线路，意味着这一条线路同时被租给N个机场，这是我们常说的共享线路机场，速度和稳定性就得碰运气了。<br>[回到顶部](#readme)
* BGP中转<br>
  * 用户 -> ss、ssr等协议 -> 国内中转服务器 -> 公网或内网穿过GFW ->  国外服务器<br>
中转服务器到GFW这一段，一般会使用一些隧道协议，以实现负载均衡、高可用、防止被墙等效果，且对传输速度也做了优化，而且多数机场还是公网过GFW。加BGP中转是比较昂贵的，所以能发现机场中带BGP中转的节点价格会比普通节点的价格贵一点。
* 专线内网中转（IPLC和IEPL）<br>
  * 用户 -> ss、ssr等协议 -> 专线服务器A（自带中转功能）-> 内网传输 -> 国外专线服务器B<br>
    * 这种方式你会发现，少了一个环节，就是它没有过GFW，就是传说中的不会被墙，因为它压根就不过墙，而且是点对点直接传输，速度相对也是最快的。虽然说是专线，但如果在进入专线之前，由于你自身的网络硬件或者网络环境导致延迟非常高，那么再快的专线也没用，所以专线的选择也要结合你自身情况去看，不是说是专线就一定速度非常快。
    * IPLC和IEPL这些专线主要是用于银行、证券、大型跨国公司这样的大型组织，严格来说，IPLC和IEPL专线本身是没有上网功能的，它们只是给前边说的那些大型组织提供内网传输服务，只有在接入相应的网络设备，才有了咱们说的上网功能，而且我们从机场买的专线，不是说直接就连到了专线入口，是经过多次跳跃中转到达专线入口，除非你住的地方正好在专线入口所在地，那中间经过的跳跃中转就少很多了，速度相对来说就更快了。<br>
    * 专线的价格相对来说也是较贵的，为什么说相对贵，因为要看你找谁买，你如果公司有资质，可直接从电信、联动等运营商手中拿到专线，那价格还是算便宜的，大多数机场其实是没有这样的资质的，个人就更不会有资质了，多数机场也是从N级代理经销商手中拿到专线，所有价格偏贵。而且像沪日专线、深港专线、美西专线等价格差距都非常大，这里给大家放一张机场供应商，注意，是机场供应商的专线价格，方便大家了解。通过机场供应商价格图我们心里大概也有个概念，为什么IPLC和IEPL的价格会偏贵点。
    ![机场供应商价格](https://www.nsaimg.com/2020/08/11/de04733555d60.jpg "机场供应商价格")
    * IPLC和IEPL专线也不是在任何时候速度都快，同一时间线路用的人有多少，机场的均衡负载技术是否做得好，线路的带宽有多大等，这些都是影响专线速度的因素。举个例子，一条专线一个月的价格是100万（其实是专线的真实价格），首先，机场需要回本，假如一个人收1000元，就需要1000个这样的客户才能回本，但光回本不够，要赚取利润，所以就需要更多的人购买，但是使用人数上升以后就可能造成机场的拥堵，这时候就看机场的技术能力了，有的机场技术好，能够做到2000人使用效果也很好，可有的机场技术不行，可能1000人使用，线路就超负载导致拥堵速度慢。这样，一些技术能力不怎么样的机场为赚取利润，就压低价格，获取大量客户，就会出现超卖的现象，导致网络拥堵，体验感极差，最终恶性循环，导致经营不下去。所以建议大家尽量去买一些大机场。
<br>[回到顶部](#readme)
#### <a id="c2.2.2.2" href="#h2.2.2.2">2.2.2、主观层面 </a> <br>
除了技术层面，我们选择一个机场就是靠我们的主观判断，我个人是从以下几个方面判断的，只能供大家参考，不是绝对正确，毕竟这个行业鱼龙混杂，只要不怕担风险，是个人就可以开机场去捞金，水也较深。<br>
##### <a id="c2.2.2.2.1" href="#h2.2.2.2.1">2.2.2.1、机场的外观设计 </a> <br>
大家会发现，几乎所有机场的界面布局都长得差不多，那是因为99%的机场用的模板代码都是同一套代码，细心的话，进机场的网站，看右下角（一般在右下，也有可能在左下），都有个staff的标志，没有staff的，会有SSPANEL，点进去也会看到staff。所以怎么去设计更换更精美的皮肤，也能侧面反映出机场主的用心程度。
##### <a id="c2.2.2.2.2" href="#h2.2.2.2.2">2.2.2.2、机场电报群观察交流 </a> <br>
大多数的机场都会提供电报群链接，机场主一般也会在里边，购买前可进电报群，肯定会有用过的人对机场的优点问题等进行交流，也可从机场主日常在群中的活跃程度、答疑解惑、日常交流等方面去感受一个机场主是否真正用心在建设这个机场。<br>[回到顶部](#readme)
##### <a id="c2.2.2.2.3" href="#h2.2.2.2.3">2.2.2.3、机场的测速 </a> <br>
有些机场有试用，可试用测速。但个人建议测速的话，可以先尝试按流量去购买机场的服务，一般1G也就不到1元，管够测速使用了。这里建议测试分多个时间段去测，再把每个时间段的测速结果去做个平均，看是否满足你心理预期。多数人喜欢用YouTube测速，其实YouTube测速只能做个参考，想得到更精确的数据，还是用SPEEDTEST或FAST测，测速时候开启全局代理，把其它会走代理的程序全部关闭。
##### <a id="c2.2.2.2.4" href="#h2.2.2.2.4">2.2.2.4、机场价格 </a> <br>
这个其实不好评判，因为每个人心理的标准都不一样，个人感觉，只要体验感和机场的价格对称就行。没有哪个贵，哪个便宜之说，都是相对的。要根据自己的实际需求去购买，这跟咱们平时买车一样，好车就是体验好，但价格也不便宜。<br>
[回到顶部](#readme)
### <a id="c2.2.3" href="#h2.2.3">2.3、客观看待机场跑路及翻墙安全问题 </a> <br>
看完前文，大家对机场也有了一定的了解，前段时间有一家大型机场跑路，其实也不能算作跑路，是被迫关闭经营，因为该机场的其中一个用户的行为引起了相关部门的重视，机场做配合调查，最后结果就是机场的支付业务受到影响，不得不停止营业，这个机场最后做的好的地方，就是把它的用户转给了其他机场。从这个事件结合前文说到的机场价格，我们看出，其实现在这个环境，好多机场主观上不是想卷钱跑路的，多数跑路的机场是经营不善或者遇到客观条件限制，导致被迫关闭。<br>
再说我们个人的翻墙行为，大家要明确自己翻墙的目的，我们翻墙是为了方便我们自己的学习、生活和工作，不是去做一些违反国家法律政策的行为，也不要好奇心很重，去浏览一些明显违规内容，让别人以为你动机不纯，那不找你喝茶找谁。大家要相信现在技术的发达程度，从几亿网民中找出你是分分钟的事儿，除非你与这个互联网世界隔绝。大家有时候看到网上说某某人因为使用某某软件翻墙浏览色情内容被请喝茶这种新闻，其实仔细想，全国有多少人每天通过翻墙浏览色情内容，为什么偏偏那个人被喝茶了，是因为他浏览的量大？是因为他使用的工具不对？是因为机场举报他了？原因你们想吧，所以，翻墙出来后一定注意约束自己的行为。
# <a id="c3" href="#h3">三、我的机场及使用感受 </a> <br>
## <a id="c3.1" href="#h3.1">1、SSR、V2ray机场：STC </a> <br>
[机场官网](https://123321.com/auth/register?code=9JIx)，用了将近一年半时间，我经历了三次机场升级，给我的体验感也由一般过渡到还行再到现在的好。也跟机场主聊过，去提一些建议，服务质量与价格还算对等。每次升级都是在大多客户反馈高峰期体验感不好的时候去考虑升级，去扩充升级一些宽带设备，以带来更好的体验感。这也是**我看中的第一点**。毕竟它是从客户角度出发去考虑的，符合我上边说的主观层面判断，所以一直坚持用到现在。<br>
唯一可能不友好的一点就是价格也在随着升级在上涨，我觉得这个也可以理解，毕竟服务成本也在提高。**我看中的第二点**就是：涨价是不针对老客户的，就是你买了之后，不管以后机场涨价多少次，你永远都可用原来的价格去续费。还有，看YouTube4K视频、Netflix等视频网站没有任何问题。<br>
**我现在用的是STC机场的企业IPLC专线，就是价格有点感人，但好在它给我的体验感对得起这个价格，基础跟进阶的属于一类，都不是IPLC专线，主要差别就是流量的多少；旗舰跟企业属于一类，都是IPLC专线，主要区别也是流量的多少。大家要是准备买的话，建议基础或旗舰二选一，当然你要是土豪，直接上企业那更爽**
![STC价格](https://www.nsaimg.com/2020/08/16/d0115be020eb7.jpg "STC价格")<br>
[回到顶部](#readme)
## <a id="c3.2" href="#h3.2">2、Trojan机场 </a> <br>
[Trojan机场官网](https://123321.com/28409)，原来的老牌shadowsocks机场，在2020年2月份所有节点全部升级为Trojan，也是为了规避GFW，目前机场的名字还叫shadowsocks。这个机场我是从2015年开始使用，升级之后速度和稳定性都有了很大提升。该机场如果遇到重大特殊情况无法使用，后期还会给客户进行降价或者延时补偿，感觉也是从客户角度出发在考虑做更好的服务。<br>
**Trojan机场支持订阅的工具如下图**
![Trojan机场](https://www.nsaimg.com/2020/04/23/fb6508b7ece3e.jpg "Trojan机场")<br>
[回到顶部](#readme)
## <a id="c3.3" href="#h3.3">3、机场综合使用感受 </a> <br>
* 我用的移动300M家用宽带，手机套餐免费送的宽带，平时翻墙会看Netflix和YouTube多点，而且经常会下载一些视频资源，两个机场配合使用完全能满足我的日常需求，用起来的区别就是：
  * 在一些晚高峰时段，[Trojan机场](https://123321.com/test)看YouTube4K偶尔会出现卡顿，但看1080P还是没什么问题的。[STC](https://mqk4azjxg8skg6gfelpb.stc-cloudserver.com/auth/register?code=9JIx)看4K完全不卡、但看8K偶尔也会出现卡顿。<br>
  * 下载视频时候，下载工具IDM，按照我的带宽，[STC](https://mqk4azjxg8skg6gfelpb.stc-cloudserver.com/auth/register?code=9JIx)是完全秒杀Trojan机场的，STC的下载速度平均下来能达到8M-13M不等,但[Trojan机场](https://123321.com/test)的下载速度平均下来只有3M-5M不等。<br>
    2020.7.19补充，经过近段时间的体验，Trojan机场的速度已经得到了很大的提升，截图是clash的速度统计，如下
![Trojan机场下载速度](https://www.nsaimg.com/2020/07/19/71a2aff860e3e.jpg "Trojan机场下载速度")
  * 当然[STC](https://mqk4azjxg8skg6gfelpb.stc-cloudserver.com/auth/register?code=9JIx)的价格也比[Trojan机场](https://123321.com/test)的价格高出很多。[STC](https://mqk4azjxg8skg6gfelpb.stc-cloudserver.com/auth/register?code=9JIx)的基础套餐**每月38元**，还有其它的更高等级套餐，可自行到[STC官网](https://mqk4azjxg8skg6gfelpb.stc-cloudserver.com/auth/register?code=9JIx)查看。[Trojan机场](https://123321.com/test)的价格是`每年19.95AUD`（按现在汇率折合人民币86元）。价格标准请以机场官网最新价格为准。<br>
  
**以上机场的使用教程见各自官网的帮助中心，各平台工具的配置步骤都非常详细。**
  
[回到顶部](#readme)
***

# <a id="c4" href="#h4">四、主流科学上网工具下载(包含Win、Mac、Android三大平台) </a> <br>
> 以下整理的工具大多都有详细的图文教程和GitHub下载地址，点详情可查看

## <a id="c4.1" href="#h4.1">1、V2ray（简称V2）</a> <br>

<details>
  <summary>详情</summary>
  支持VMESS协议的图形界面工具挺多的，下面给大家列举几个常用的<br>
  1、<a href="https://github.com/2dust/v2rayN/releases">V2ray的Windows端图形界面工具V2RayN下载</a>，顺便附上一个
  <a href="https://github.com/233boy/v2ray/wiki/V2RayN%E4%BD%BF%E7%94%A8%E6%95%99%E7%A8%8B">V2RayN详细图文教程。</a><br>
  2、V2ray的Windows端图形界面工具<a href="https://github.com/Cenmrev/V2RayW/releases">V2RayW下载</a><br>
  3、V2ray的Mac端图形界面工具<a href="https://github.com/Cenmrev/V2RayX/releases">V2RayX下载</a>、
  <a href="https://github.com/yanue/V2rayU/releases">V2RayU下载</a><br>
  4、<a href="https://github.com/2dust/v2rayNG/releases">V2ray（Android）下载</a><br>
  5、<a href="https://www.v2ray.com/">V2ray官方使用手册文档</a><br>
</details>

## <a id="c4.2" href="#h4.2">2、Clash</a> <br>

<details>
  <summary>详情</summary>
  1、clash也是一款不错的代理工具，支持VMESS和Trojan协议，但不支持ssr。它的衍生版clashR支持ssr、vmess协议。clash想要实现真正的全局代理，除了开启
  System Proxy外，还需要安装TAP虚拟网卡设备。<br>
  clash的Windows客户端叫做clash For Windows，简称CFW，<a href="https://github.com/Fndroid/clash_for_windows_pkg/releases">CFW下
  载。</a>给大家附上CFW的<a href="https://docs.cfw.lbyczf.com/">【文档教程】</a> 
  <br>
  2、<a href="https://github.com/yichengchen/clashX/releases">clash（Mac）下载</a><br>
  3、<a href="https://github.com/Kr328/ClashForAndroid/releases">clash（Android）下载</a>、
  <a href="https://play.google.com/store/apps/details?id=com.github.kr328.clash&hl=en_US">Clash in Google Play安装</a><br>
  4、<a href="https://sxcool1024.lanzous.com/i9zpaji">ClashR汉化版，支持SSR和V2ray订阅</a><br>
  5、<a href="https://docs.nameless13.com/shr/">ClashR各平台相关教程</a><br>
</details>

## <a id="c4.3" href="#h4.3">3、Trojan</a> <br>

<details>
  <summary>详情</summary>
  1、支持Trojan协议的工具并不多，电脑端的图形界面工具有<a href="https://github.com/TheWanderingCoel/Trojan-Qt5/releases">Trojan-
  Qt5(Win+Mac+Linux)下载</a>，TrojanQt5支持一键订阅导入，只要你有Trojan机场订阅链接，即可一次性导入所有节点。工具界面如下图：<br>
  <img src="https://www.nsaimg.com/2020/05/08/7e444c1ec6dfb.png" alt="Trojan工具"><br>
  2、安卓端目前支持Trojan协议的工具<a href="https://github.com/trojan-gfw/igniter/releases">igniter下载</a><br>
  3、<a href="https://trojan-tutor.github.io/2019/04/10/p41.html">自建梯子教程--Trojan版本</a><br>
  4、喜欢用黑屏命令风格的伙伴可下载<a href="https://github.com/trojan-gfw/trojan/releases">Trojan的Windows、macOS、Linux三大平台命令行工具
  </a><br>
  5、<a href="https://portal.shadowsocks.nl/knowledgebase/151/Trojan-%E6%9C%8D%E5%8A%A1%E5%AE%A2%E6%88%B7%E7%AB%AF%E8%AE%BE%E7%BD%AE%E6%95%99%E7%A8%8B%E7%B4%A2%E5%BC%95.html">以上Trojan工具的设置教程索引</a><br>
</details>

## <a id="c4.4" href="#h4.4">4、Sstap</a> <br>

<details>
  <summary>详情</summary>
  1、真正的全局代理工具sstap，虽然是游戏加速器，但功能非常实用，通过专属虚拟网卡，真正实现系统内所有程序全部走代理，还可以根据自己需求选择内置代理
  DNS，让科学上网速度更快，安全性更高，具体见下图<br>
  <img src="https://www.nsaimg.com/2020/05/08/98abce621e6c5.jpg" alt="SSTAP">
  <img src="https://www.nsaimg.com/2020/05/08/6a7fd9ec22033.jpg" alt="SSTAP">
  2、<a href="https://sxcool1024.lanzous.com/iIvPbge7utg">SSTAP下载</a><br>
</details>

## <a id="c4.5" href="#h4.5">5、Netch</a> <br>

<details>
  <summary>详情</summary>
  1、Netch是一个开源游戏加速器。与需要添加规则以用作黑名单代理的SSTap不同，Netch更类似于SocksCap64，可以扫描需要代理的程序的安装目录，来专门获取其进程
  名称，从而实现真正分应用代理。 Netch也可以实现 SSTap那样的全局 TUN/TAP 代理。Netch现在支持Socks5，Shadowsocks，ShadowsocksR，VMess、Trojan协
  议，也是目前为数不多的几乎支持所有协议的工具。<br>
  <img src="https://www.nsaimg.com/2020/05/09/86fba7f8b2272.jpg" alt="netch">
  <img src="https://www.nsaimg.com/2020/05/09/39bc0a5b907f3.jpg" alt="netch">
  <img src="https://www.nsaimg.com/2020/05/09/3bb66a8cf22a7.jpg" alt="netch">
  2、<a href="https://github.com/NetchX/Netch/releases">Netch下载</a><br>
</details>

[回到顶部](#readme)

## <a id="c4.6" href="#h4.6">6、Mellow</a> <br>

<details>
  <summary>详情</summary>
  1、Mellow 是一个基于规则的全局透明代理工具，可以运行在 Windows、macOS 和 Linux 上，也可以配置成路由器透明代理或代理网关，支持 SOCKS、HTTP、
  Shadowsocks、VMess 等多种代理协议。<br>
  2、<a href="https://github.com/mellow-io/mellow/releases">Mellow安装文件下载(Win+Mac+Linux)</a><br>
</details>

## <a id="c4.7" href="#h4.7">7、Pharos Pro</a> <br>

<details>
  <summary>详情</summary>
  1、<a href="https://github.com/PharosVip/Pharos-Android-Test/releases">Pharos Pro(Android)下载</a><br>
  2、Pharos Pro(iOS)，登录非大陆AppleID下载，不会的可加电报群咨询我
</details>

## <a id="c4.8" href="#h4.8">8、shadowrocket</a> <br>

<details>
  <summary>详情</summary>
  1、<a href="http://laob.me/2300/">ShadowRocket基础教程</a><br>
  2、<a href="https://blog.minirplus.com/14472/">ShadowRocket分组、规则自动切换节点</a><br>
  3、shadowrocket是iOS上的专属收费翻墙工具，购买需要登录非国区AppleID。
</details>

## <a id="c4.9" href="#h4.9">9、Shadowsocks（简称SS）</a> <br>

<details>
  <summary>详情</summary>
  1、<a href="https://github.com/shadowsocks/shadowsocks-windows/releases">Shadowsocks（Win）下载</a><br>
  2、<a href="https://github.com/shadowsocks/ShadowsocksX-NG/releases/">Shadowsocks（Mac）下载</a><br>
  3、<a href="https://github.com/shadowsocks/shadowsocks-android/releases">Shadowsocks（Android）下载</a><br>
</details>

## <a id="c4.10" href="#h4.10">10、ShadowsocksR（简称SSR）</a> <br>

<details>
  <summary>详情</summary>
  1、<a href="https://github.com/shadowsocksrr/shadowsocksr-csharp/releases">ShadowsocksR（Win）下载</a><br>
  2、<a href="https://github.com/qinyuhang/ShadowsocksX-NG-R/releases">ShadowsocksR（Mac）下载</a><br>
  3、<a href="https://github.com/shadowsocksrr/shadowsocksr-android/releases">ShadowsocksR（Android）下载</a><br>
</details>

***
`关于iOS平台的科学上网工具，目前支持协议较完善的有shadowrocket、suerge、Quantumult、Pharos等，需要用非大陆AppleID下载且收费，请大家自行注册购买，不会的加群找我`

[回到顶部](#readme)
***



[回到顶部](#readme)



