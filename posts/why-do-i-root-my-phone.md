```json
{
  "title": "从 root 手机说起",
  "url": "why-do-i-root-my-phone",
  "date": "2017-10-08",
  "parser": "Markdown",
  "cover": "https://oa3o2340x.qnssl.com/phone.jpg",
  "tags": ["Life", "Tech", "Thoughts"]
}
```

昨天在知乎上回答了一个问题

[如何评价魅族Flyme系统即将关闭root功能？](https://www.zhihu.com/question/65370132/)

问题的内容大致是，魅族计划以「安全」为理由去除系统中的 `root` 功能，请问大家如何看待。我在回答中主要提及了「用户对自己购买的手机的控制权」这一问题。当然，在知乎上发表这类言论，必然的引来了评论区的一场“大战”。由于知乎实在不是一个保存和展示文字内容的好地方，所以我选择把更详细的内容放在这篇文章里阐述。

### 写在前面

在讨论评论中一些人的问题之前，我想我有必要重新摆明我在这种事情上的立场。

第一，我认为自己购买的设备应当是完全属于自己，也就是说「购买」这个行为是针对所有权而不应该是使用权。当我购买手机的时候，我不是在购买手机这个设备的使用权，而是完整的所有权。我应该能够在这个设备上运行任何我希望且能够运行的软件而不受厂商的控制。当然，在今天，这个要求其实是很高的 —— 比如越狱就是一个合法性一直饱受争议的行为 [[1]](#References)，尽管从我的角度来看，「越狱违法」是很不可理喻的。同时，也有很多人提及，购买手机时立下的用户协议中，可能就是仅仅授予了使用权，而其他一切都与最终用户无关 —— 这正是我想要反对的东西。令人欣慰的是，EFF [[2]](#References) 等组织也一直在为了实现这个目标而努力。

第二，「Root」这一行为的目的是获取自己设备的更高控制权，这是正当而且合理的行为，而不是需要隐藏的不齿行为。「Root」不是为了破解别人的软件而存在，不是为了侵犯开发者的利益而存在，是用户为了保护自己的利益和获取自己应有的控制权的正当手段。通过「Root」可以更好地定制自己的 Android 设备，包括但不限于内核参数调节、使用主题或自定义字体、更方便地使用非官方应用市场、控制某些软件滥用权限或滥用后台等等。

第三，厂商应该通过为用户提供产品和服务获取利益，而不是通过限制用户的自由获取利益。在这里我想强调的是，用户花钱买的是产品和服务，而不是花钱去买“爹”。厂商的目标是切合用户需求而不是控制用户的需求，是听取用户想要什么而不是告诉用户应该要什么。所有举措，包括所谓安全举措，前提都必须是用户拥有知情权和选择权，他应当有选择拒绝的权利，哪怕是「拒绝安全」，这也都是自己的选择。厂商没有必要为用户的选择承担责任，但必须要确保用户有能力进行自己的选择。对于不能满足自己要求的厂商，用户可以选择不买，不买的同时更加有权利向他人说明自己拒绝该厂商的理由以供他人参考。

第四，本人关于该话题的所有观点，其重点都在于「能不能」，而不是「会不会」。也就是说，如果有的人，他追求的是简单方便，他没有那个心情去折腾什么自定义，也没有兴趣去获取更高的控制权，那么我完全不反对，因为这是他的选择。但是，同样也会有人不喜欢什么简单方便，什么傻瓜式设计，他需要运行他自己的软件，因此需要更高的权限，他也应该有这个能力去作出这样的选择 —— 毕竟，这是智能设备，不是大哥大板砖。「我不会去 root」「他也不会去 root」「我认识的人都不 root」都不能成为直接关闭这个功能的理由 —— 因为它不是一个简单的功能，它是用户控制设备的一个途径。

以上就是我对于这个问题的立场，以下所有讨论都是在上面的立场的基础上进行的。

### 苹果设备

发布了这些言论以后，最早收到的评论就是「那么苹果呢？」，更有人说我对苹果就“跪舔”而对 Android 就要求很多。老实说，我完全没有在知乎上发表过我对苹果设备的看法，因此我完全不知道他们是从哪里看出来我对苹果设备的态度，不过既然这样说了，我就可以顺便阐述一下自己对苹果设备（注：此处相应地只讨论 iOS 设备，即 iPhone, iPad, iPod Touch）的观点。

首先我完全不否认苹果在乔布斯时代的设计水平，乔布斯也是我比较佩服的人物之一，我自己和我的家人也使用过或者正在使用部分苹果产品。但是，这并不代表我认同他们的产品理念，也并不代表我认同他们在软件方面的策略。我不喜欢用「X宗罪」的形式评价一个产品，但是在这一点上我实在觉得自己有点数不清苹果究竟有多少「没法用」的地方。因此，我想概述 Richard M. Stallman 在自己的博客 [[3]](#References) 上写明的 __一部分__ 我认同的「不使用苹果设备的理由」

1. 苹果的应用商店有严格的审查制度，并且在正常的苹果设备上使用第三方商店是不可能的。苹果对于自己商店里的应有有比法律法规更严格的审查，直接导致有些应用是根本无法在苹果的设备上使用的。同时，这个审查制度也具有双重标准，比如 iOS 上至今没有一款非 Safari 内核的浏览器（因为可执行代码的问题），可是一些厂商的“热更新”技术却能在应用商店上架。

2. 苹果曾（且仍然在）尝试阻止用户修理自己的设备，并且试图阻止使其合法的法案通过 [[4]](#References)。iPhone 7 甚至有通过让设备“变砖”来阻止拆开修理的技术手段 [[5]](#References)。他们不把用户当成客户，而是当成自己控制的对象。他们想要成为你的「老大哥」。

这两点正是最重要的两点。总而言之，从这样的商家购买设备，你花钱买来的不是产品，也不是服务，而是一个远在千里之外的“爹”。也许有的人会喜欢这样，不需要自己动手或者动脑子，但是对不起，至少我很反感，而且我也不会再去购买苹果设备 —— 即使他们的设计再吸引人。

### 为什么不买个开发板

于是有人就问我，「你为什么不买个开发板，自己DIY一个手机出来用」。

这个问题非常有意思。答案是很简单的：因为我没有选择。

最重要的问题就是「基带」—— 手机的“移动通讯”功能的底层部件。现存的基带基本都是黑盒 [[6]](#References)，同时具有相当高的系统权限（它们本身甚至也运行了一套完整的操作系统），完全可以用于大规模监视。更严重的是，由于太过大量的通讯标准以及专利壁垒的存在，开源实现几乎是不可能的事情，这直接导致了目前市面上几乎不存在「能用的」开源实现的基带 —— 即使有，也基本上只实现了一万年前的协议和功能…… 我在 Indiegogo 上找到了一个通过逆向工程制造开源基带硬件的众筹项目 [[7]](#References)，但那是 2015 年的事情，众筹目标并没有达成，而且似乎很久没有后续更新了……

而没有了通讯功能，还做什么“手机”……做出来了也只是个板砖罢了。

什么？你说你想自己发明一套完全开放的标准？不好意思，你还得通过各大机构的认证，还得想办法让全世界，至少很多国家的通讯企业都接受这个标准 —— 可是这个行业是非常非常喜欢自己造轮子、自己搞自己的一套的。因为标准拿在手上就是利润，可以大肆向同行甚至竞争对手收取费用。在这些企业面前，开放的力量几乎是不存在的。

所以，对于这个问题，结论就是：不存在的。

### 大部分人不需要 ROOT

这是我也认同的一个观点。大部分人确实没有那个时间或者能力去折腾自己买来的手机，只要够用就好了。

可是我们这里讨论的问题是「能不能」，而不是「要不要」，「会不会」。对于一个手机小白，我也绝对不会跟他说「你买了手机先 ROOT 一下」，因为这本身是很危险的事情，他们自己都不一定知道自己在做些什么。自己不知道后果的选择不能称之为用户的选择。同理，我在这里再怎么说我 ROOT，也绝对不会给任何欺骗用户授权 ROOT 以获得更高权限的流氓软件带来任何的合理性。

换句话说，我所支持的不是 ROOT 这个行为本身，而是在关注我是否被允许、是否可以对自己购买的设备作出修改，是否能够在它上面运行官方之外的软件。你做不做这件事情不重要，那是你自己选择的事情，问题在于是否可以这么做。「是否可以」意味着身为一个用户的自由和被尊重，而自己放弃是完全合理而且没有任何问题的事情。

从另外一个角度，“大部分人”的论述真的能成立吗？比如，大部分人都不关心也搞不懂窃听之类的东西，搞不懂什么叫中间人攻击，搞不懂 HTTPS 和 HTTP 有什么区别，也搞不懂为什么使用无加密的公共 WiFi 非常危险，于是操作系统、浏览器里面实现的安全功能就能说是多余的吗？他们不关心自己的隐私和安全，就是作为软件开发者 / 厂商不关心用户的隐私和安全的理由吗？用户不关心自己是否拥有自己该有的权利和自由，就是厂商漠视这些的理由吗？不是的。作为开发者，作为厂商，当然需要（在一定程度上，在用户知情且有选择权的前提下）保护用户的权益（比如说，为了安全默认关闭 ROOT，同时允许部分用户 ROOT，但是给 ROOT 操作设置一定的门槛，让懂得后果的人才能执行），否则谈何“服务”呢。虽然作为用户，完全信任商业公司是一件比较危险的事情，但这也不能成为商业公司作恶的理由。

总而言之，关于这个问题，我想说的是

1. 用户做不做 ROOT 之类的事情和我讨论的「能不能」是无关的
2. 我尊重每个人自己选择
3. 「大部分人」这种论述方式存在一些问题

### 即使 ROOT 了，也仍然不能控制设备

是的，这正是现在的移动平台存在的问题。除了上面我提及的基带问题之外，现在 Android 设备上都存在大量的私有驱动，通过 HAL 绕过了 Linux 内核的协议限制。同时，很多设备的 bootloader 都是不开源的，这直接导致启动过程的第一环就已经不受控制。再加上 TrustZone 等私有固件，你想要完全控制你手上的那个设备，恐怕还有很远的路要走 —— 而且这里我还仅仅列举了软件部分。到了硬件层面，那就是个更加无解的复杂问题。

所以我们能做的，只能是

1. 争取到可能获取到的最多的权限
2. 拒绝那些不信任用户、不给用户合理的权限的厂商
3. 让人们知道这些不合理的东西的存在

至于更多的，就像我上面提及的关于自己做手机的问题一样，会变成非常非常困难的事情。虽然还是期待有人能够这么做，但是凭我自己的能力已经不可能了。

### 其他

上面已经讨论了之前评论区里被提及的几个很重要的问题。不过，评论区里还有一些我觉得非常可笑的问题，想要拿出来放在这里。

> 同理建议空客波音特斯拉开放系统硬件最高权限

以及

> 你在天朝跟政府和公司领导要root权限了嘛

首先，这完全就是不同的概念。政府和你的关系是一种契约，公司和你的关系是一种劳务关系，而你乘坐空客波音的时候仅仅是临时使用他们的服务而已。你本来就不可能拥有你的政府和你的公司，谈何索取权限？而关于波音的飞机，第一如果你只是临时乘坐，你当然不可能索取权限；第二如果你真的购买了一架飞机，你还要考虑到高权限可能给他人带来的人身损害（当然，如果你愿意把所有的锅都放到自己头上，为所有一切可能出现的问题埋单的话，你大可以这么做）。可是手机只是一个贴身的设备而已，即使真的发生了爆炸，基本上也只能损伤你自己而已。

> 好吧，也许你买的只是一堆没用的金属塑料玻璃材料，我们买的都是体验。

不好意思，我想我比你更注重体验。

> 你要那么多权限为的是什么啊？不折腾，手机就差到没法使用吗？

不好意思，我想我比你更懂手机。

> 手机丢了以后，root的就等着个人信息满天飞，指不定还有更有意思的发生

不好意思，你的个人信息很可能早就被你的可爱的手机厂商们、应用厂商们卖掉了 [[8]](#References) —— 而你的手机还在你的手上。另外，厂商的责任永远不是告诉我应该做什么，而是告诉我我的操作的后果，让我知道后果并且在我能够接受后果的前提下进行操作。况且，ROOT 之后真的说不定更安全（笑）。一个注重隐私的人，更应该对开放的硬件和软件有更高的需求。

> 在美国，公民拥枪是权利。但我感觉像中国这样，把公民的这个权利剥夺了更好。当然，如果某天政府的人对我实施非法侵害，我又希望能拥枪。但一般情况下，可能我成为那59个死者和那数百伤者中的一员的可能性要大得多

我一点也看不懂这个类比是怎么回事。ROOT 手机，和禁止持枪，有任何可比性吗？持枪不需要任何多余操作就可以危及他人的人身安全，可是 ROOT 一下手机会吗？你就算把手机的温度保护之类的措施强行去掉，也不能当成炸弹使用。再者，菜刀也能杀人，菜刀比一个 ROOT 之后的手机杀伤力要强得多，可是菜刀被禁止了吗？（菜刀确实是实名购买的，但是你的手机要入网，也需要实名）因此这根本就是一个很站不住脚的偷换概念……

### 补充

还有一个问题（不属于上面提及的可笑的问题）

> 反对。买手机并使用，是遵守用户协议的合同行为。买的不是手机本身，而是合同里面规定的内容。

是的，正是这样。但是我并不是在讨论是否应该遵守用户协议，而是这些严重限制用户的协议是否合理，或者说，用户在不知不觉间订立的这些协议到底给用户带来了什么，又让用户损失了些什么。如果一定要说是协议的话，那么我的结论是这样的协议不能去订立，也就是说我，从我的观点得出，我会拒绝购买这样的手机。

### <a name="References"></a>参考资料

1. [US government says it's now okay to jailbreak your tablet and smart TV](https://www.theverge.com/2015/10/27/9622066/jailbreak-unlocked-tablet-smart-tvs-dmca-exemption-library-of-congress)
2. [Jailbreaking Is Not A Crime—And EFF Is Fighting To Keep It That Way](https://www.eff.org/deeplinks/2014/11/jailbreaking-not-crime-and-eff-fighting-keep-it-way)
3. [Reasons not to use Apple](https://stallman.org/apple.html)
4. [Apple Is Fighting A Secret War To Keep You From Repairing Your Phone](http://www.huffingtonpost.com/entry/apple-right-to-repair_us_5755a6b4e4b0ed593f14fdea)
5. [The iPhone 7 Has Arbitrary Software Locks That Prevent Repair](https://motherboard.vice.com/en_us/article/kbjm8e/iphone-7-home-button-unreplaceable-repair-software-lock)
6. [The second operating system hiding in every mobile phone](http://www.osnews.com/story/27416/The_second_operating_system_hiding_in_every_mobile_phone)
7. [Free Software Cellular Baseband](https://www.indiegogo.com/projects/free-software-cellular-baseband#/)
8. [Privacy Change: Apple Knows Where Your Phone Is And Is Telling People](https://consumerist.com/2010/06/21/privacy-change-apple-knows-your-phone-is-and-is-telling-people/)