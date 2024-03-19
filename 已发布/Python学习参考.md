[TOC]

# ⭐️写在前面的话⭐️
> CSDN主页：[程序员好冰](https://blog.csdn.net/m0_67689541?spm=1000.2115.3001.5343)
>
> 目前在学习：操作系统
>
> 技术栈：SpringBoot项目
>
> 推荐书籍：《Java虚拟机》、《Java编程思想》
>
> 博客网站：暂无
>
> ==旅途的意义亦在旅途中。==
>
> 🎉欢迎 【点赞👍 关注🔎 收藏⭐️ 留言📝】
> 📌本文由 程序员好冰 原创，CSDN 首发！
> 📆入站时间： 🌴2022 年 07 月 13 日🌴
>
> 🍭<strong><font color = orange> 作者水平很有限，如果发现错误，一定要及时告知作者哦！感谢感谢！</font></strong>🍭

--- ---



# 一、Python的历史与发展

## 1、历史

> 本段转载于[Python简介及发展历史 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/169624095)

Python，读作`['paɪθɑn]`，翻译成汉语是蟒蛇的意思，并且Python的logo也是两条缠绕在一起的蟒蛇的样子，然而Python语言和蟒蛇实际上并没有一毛钱关系。

Python的口号是：“人生苦短，我用Python”被Python业界广泛使用，快成了广告词一类的存在了。

![image-20231018074424607](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018074424607.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

Python语言是由**荷兰程序员Guido van Rossum**，江湖人称“龟叔”，独立开发完成初版的。“龟叔”曾供职于google，现任职于dropbox 。1989年圣诞节期间，在阿姆斯特丹，为了打发圣诞节的无趣，决心开发一个新的**脚本解释语言**，作为ABC语言的一种继承，然后他就这么做了，并实现了（大神的能力）。之所以选中Python作为该编程语言的名字，是因为他是一个叫Monty Python喜剧团体的爱好者，其本意并不是想选条蟒蛇。

Python第一个公开发行版发行于**1991年**，所以这年被当作Python的诞生年。

Python 源代码遵循 **GPL**(GNU General Public License)协议，这是一个开源的协议，也就是说你可以免费使用和传播它，而不用担心版权的问题。

目前Python是由一个核心开发团队在维护，龟叔属于太上皇职位，仍然占据着至关重要的作用，指导其进展。

## 2、发展

> 本段转载于[Python三十年技术演变史 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/74621819)

【导语】一切都始于1989年的那个圣诞节，Python的诞生并不算恰逢其时，它崛起充满了机遇巧合，也有其必然性。三十年间，Python技术不断更迭，生态逐渐完善，加上互联网、大数据、以及人工智能这一波波浪潮的推波助澜，Python渐渐从小众最终站上了现在的高度。
		从历史发展的角度出发，我们才能看清Python崛起的偶然性和必然性。

### Python 1.0时代：起源与诞生

Guido van Rossum（下面简称Guido）是Python语言之父，他于1982年从阿姆斯特丹大学获得了数学和计算机硕士双学位，期间他接触了很多的语言，包括Pascal，C，Fortran等。

在那个计算机资源贫乏的年代，像计算机一样思考并编程是每个程序员必须面对的事情，这让他非常苦恼；同时他又非常欣赏shell，shell简单易编程的特性让程序员更加专注于设计和逻辑本身，但shell本质上是一个功能的调用，它**没有自己的数据类型**，更无法全面调用计算机功能，因此**shell也不算是一门“语言”**。

因此，他希望找到一种语言既可以像使用shell一样简单，又可以和C语言的功能相媲美。不过这种语言在那个年代并不存在。

1989年的圣诞节，Guido开始编写Python语言的编译器。Python这个名字来源于他喜欢的电视剧Monty Python’s Flying Circus，而不是表面意义上的“蟒蛇”。他希望这个新的语言，能符合他的理想：==介于C和shell之间，功能全面、易学、易用又可拓展==。

1991年，第一个Python编译器诞生，这标志着Python的第一个版本正式诞生。**它基于C语言，并具备了基础的类、函数、异常处理等功能特性，同时具备可扩展性。**Python语法很多来自C，但又受到ABC语言的强烈影响。例如来源于ABC语言强制缩进的规定本身可以让Python容易读，但如果缩进出错却会影响编译和执行。**Python本身不以性能为重，但当确实需要考虑性能时，Python程序员却可以深入底层来编写C程序，并编译为.so文件引入到Python中使用。**

Python语言的魅力在于让程序员可以花更多的时间用于思考程序的逻辑，而不是具体的实现细节，这一特性也得到Guido同事的欢迎。他们在反馈使用意见的同时也参与到Python的改进中来，因此最初Guido和一些同事构成了Python的核心团队，当然，核心决策者还是Guido本人。随后，Python的使用拓展到研究所之外，并吸引了越来越多的程序员。

但是，最初Python的使用非常小众，因为在那个计算机资源非常有限的年代，大家都倾向于最大化榨取计算机资源并提升运算效率，而Python显然不是为此而生。

### Python 2.0时代：崛起

最初发布时，Python在设计层面存在一些缺陷，例如**以满足跨语言**、**跨平台进行文本转换**、**处理的要求的Unicode字符编码标准**在1994年才正式公布，所以一直以来Python 2及之前的版本对Unicode的支持并不完全。相信大家在使用Python 2版本处理中文时都遇到过各种问题。

2000年发布的Python 2.0标志着Python的框架基本确定。重要框架方向包括：

- **简单明确**。在设计Python语言时，开发者倾向于选择没有或者很少有歧义的语法。由于这种设计观念的差异，Python源代码通常被认为比Perl具备更好的可读性，并且能够支撑大规模的软件开发。

- **面向对象**。任何Python的元素都可以视为对象，包括数据类型、类、函数、实例化元素等，完全支持继承、重载关系，这有益于增强代码的复用性。

- **动态类型**。任何对象的数据类型都无需提前定义，拿来即用。即使在之前已经预先定义，后期也可随时修改。

- **胶水特性**。Python本身被设计为可扩充的，并非所有的特性和功能都集成到语言核心。Python提供了丰富的API和工具，以便程序员能够轻松地使用C、C++、Cython来编写扩充模块。例如在Google对于Google Engine使用C++编写性能要求极高的部分，然后用Python或Java/Go调用相应的模块。

- **可嵌入**。你可以把Python的功能嵌入到C/C++程序中，从而实现Python功能在其他语言中的功能实现。

- **生态系统**。Python有强大的标准库，同时支持第三方库和包的扩展应用，甚至可以自定义任何库和包。Pypi（[https://pypi.org/](https://link.zhihu.com/?target=https%3A//pypi.org/)）是其第三方库的仓库，在这里你几乎可以找到任何领域内的功能库。

- **解释器机制**。Python支持多种解释器，例如CPython（官方版本，基于C语言开发，也是使用最广的Python解释器）、IPython（基于CPython之上的一个交互式解释器）、PyPy（一个追求执行速度的Python解释器，采用JIT技术对Python代码进行动态编译）、Jython（运行在Java平台上的Python解释器，可以直接把Python代码编译成Java字节码执行）、IronPython（和Jython类似，只不过运行在微软.Net平台上）。

1965年，戈登·摩尔提出了著名的**摩尔定律**，其内容为：当价格不变时，集成电路上可容纳的元器件的数目，约每隔18-24个月便会增加一倍，性能也将提升一倍。在随后超过半个世纪的时间里，个人计算机的发展日新月异，已经由资源不足向资源过剩转变。这客观上为Python的应用提供了基础条件——只有在资源过剩的条件下，程序员才不会过度关注榨取性能。

随着Python自身功能的完善以及生态系统的扩展，Python在Web开发、网络爬虫、数据分析与数据挖掘、人工智能等应用方面逐渐崭露头角。

- #### Django和Flask引领的WEB开发模式

2004年，目前最流行的**WEB框架Django**诞生。2010年，另一个流行的轻量级**WEB框架Flask**诞生。Django是一个WEB解决方案“全家桶”，其功能大而全，包含了几乎所有WEB开发相关的组件和功能，它可以大大节省开发者在基础组件、选型、适配等方面的时间和精力；而Flask只包含基本的配置，默认依赖于两个外部库也可以自由替换，给开发者提供最大的自主空间。**这两类完全相反方向上的WEB开发模式，几乎可以为所有开发者提供了很好的选型参照物**：无论开发者想要一站式还是最大化自主解决方案，Python都能满足。

此后，以豆瓣、春雨医生、知乎、Dropbox、YouTube、CIA（美国中情局）等为代表的企业和机构都基于Python做网站开发，预示着Python应用到WEB开发领域逐渐成为一种新兴趋势。

- #### 人人都能胜任的网络爬虫

Python自带的标准库中，urllib、urllib2、requests库对于简单网页的抓取实现非常简单，即使在面对海量数据抓取需求时，第三方库Scrapy也能应对自如；再配合正则表达式库re、网页代码解析BeautifulSoup、html和xml解析库lxml、多线程库threading等特性，使得Python在应用到网络爬虫任务上时，只需要很少的开发量便能迅速完成任务。基于Python简单易学的特性，几乎人人都能开发网络爬虫。

- #### 比shell更好用的自动化运维工具

Python是跨语言和平台的，几乎所有Linux系统和MAC系统都自带Python库，Windows系统也可以自定义安装。Python默认的os、sys等库可实现与操作系统的交互和执行功能，更重要的是Python还能直接执行系统终端命令。因此，使用Python编写的系统运维和管理脚本在可读性、性能、代码重用度、扩展性几方面都优于普通的shell脚本，在自动化运维方面应用广泛。

- #### 数据分析与科学计算三剑客

2008年发布的Numpy、scipy和2009年发布的pandas是数据分析与科学计算的三剑客。

**NumPy**（Numeric Python的简称）是Python科学计算的基础工具包，也是Python做数据计算的关键库之一，同时又是很多第三方库的依赖库。

**Scipy**（Scientific Computing Tools for Python的简称）是一组专门解决科学和工程计算不同场景的主题工具包，它提供的主要功能侧重于数学、函数等，例如积分和微分方程求解。Pandas（Python Data Analysis Library的简称）是一个用于Python数据分析的库，它的主要作用是进行数据分析和预处理。

**Pandas**提供用于进行结构化数据分析的二维表格型数据结构DataFrame，类似于R中的数据框，能提供类似于数据库中的切片、切块、聚合、选择子集等精细化操作，为数据分析提供便捷。另外，Pandas还提供了时间序列的功能，用于金融行业的数据分析。

除此之外，很多大型公司也都在使用Python完成不同类型的其他工作，其中不乏世界知名公司，如国外的Google、Facebook、NASA 、雅虎、YouTube等，国内的网易、腾讯、搜狐、金山等。例如谷歌在Google Groups、Gmail、Google Maps等项目中将Python用作网络应用的后端；在Google Cloud Platform中的Google Cloud Storage本地部署环境中，gsutil也在Python 2基础上开发和应用。

### 后Python2与Python3时代：AI让Python大放异彩

2008年12月，Python 3发布。**Python 3**相对于Python 2的早期版本（主要是Python2.6之前）是一个较大的升级，它在设计的时候**没有考虑向下兼容**，所以很多早期版本的Python程序无法在Python 3上运行。为了照顾早期的版本，推出过渡版本2.6——基本使用了Python 2.x的语法和库，同时考虑了向Python 3.0的迁移，允许使用部分Python 3.0的语法与函数。同时，Python还提供了Python 2到Python 3的Python文件转换功能，以帮助开发者升级。

2010年7月发布了**Python 2.x系列的最后一个版本，主版本号为2.7**。大量Python 3的特性被反向迁移到了Python 2.7，2.7版本比2.6版本进步非常多，同时拥有大量Python 3中的特性和库，并且照顾了原有的Python开发人群。**Python2.7**也是当前绝大多数Linux操作系统最新版本的默认Python版本。

从2008年开始，Python 2与Python 3是并存发展的。但在2018年3月，Guido在邮件列表上宣布==Python 2.7将于2020年1月1日终止支持==，这意味着之后Python 2将不再被统一维护，与之对应的是主流第三方库也不会再提供针对Python 2版本的开发支持。Python 2的时代即将过去。

这一时期，Python继续以其独特魅力吸引更多的开发者加入，但真正让Python大放异彩的却是AI（人工智能）的爆发。

AI并不是一个新生事物，而是从20世纪50年代就开始出现，随后经过了大概20年的黄金时期，又分别在20世纪70年代和90年代两次进入寒冬期。从2006年开始，神经网络、深度学习的出现，让AI进入爆发期。



在AI领域，Python拥有很多相关库和框架。其中最著名的是：

- **sklearn**：一个老牌机器学习库，其neural_network库可用来做神经网络训练。

- **PyTorch**：由Facebook于2016年发布，它基于曾经非常流行的Torch框架而来，为深度学习的普及迈出了重要一步，到目前为止它已经是人们用来做学术研究的首选方案。

- **TensorFlow**：谷歌于2015年研发的第二代人工智能学习系统。借助谷歌的强大号召力以及在人工智能领域的技术实力，它已经成为目前企业真实生产环境中最流行的开源AI框架。更重要的是，==它也是第一个（应该也是唯一一个）经过真实大规模生产环境（Google）检验过的框架==。

在互联网领域，Facebook和Google都是全球IT企业的标杆，具备行业领导力和风向指示意义。他们基于Python开发的AI库（PyTorch和TensorFlow）已经成为目前最流行的AI库，而且“到底选择PyTorch还是Tensorflow”仍然是一个具有争议性的话题。



在AI时代，主要应用场景包括：

- **计算机视觉**：通过特定的图片模式训练，让计算机理解图像中的物体甚至内容。在这一领域我们熟悉的场景包括图像识别、目标识别和跟踪。例如人脸识别便是图像识别的典型领域，广泛应用到企业员工考勤、门店客户识别、机场等公共领域反恐识别等。2011年，吴恩达创立的谷歌大脑项目，能够在没有任何先验知识的情况下，仅仅通过观看无标注视频学习到识别高级别的概念就能知道哪个是猫。

- **语音识别**：该过程是计算机将人类的自然语言识别并转换为文字的过程，广泛应用工业、家电、通信、汽车电子、医疗、家庭服务、消费电子产品等各个领域。身边熟悉的场景例如通过语言对导航、APP、车载设备等做指令输入，以及电信客服系统中的语音业务查询和办理。

- **自然语言理解**：自然语言理解是一类任务的总称，而并非是单一任务。它旨在让计算机理解人类的语言所表达的表层和深层含义。目前场见的应用场景包括自动问答系统、机器翻译、信息检索和过滤、信息抽取等。

- **个性化推荐**：个性化推荐是一个相对成熟的领域，但基于深度学习和神经网络，可以将大量的复杂、抽象特征的数据预处理工作最大程度的简化，甚至可以将海量特征经过简单处理后便直接丢到模型中便能获得比例理想的效果。

- **游戏和竞技**：在该领域，很多科技公司用经过训练后的AI与人类进行对弈。早在20世纪90年代，由IBM开发的“深蓝”与卡斯帕罗夫的世纪之战已经引起了世界的轰动；在2017年AlphaGo又击败排名世界围棋冠军柯洁，再一次让世人感受到AI的强大威力。

在不同的领域，Python都能扮演非常重要的角色，因此，在国外的各大榜单中，Python都已经成为最受欢迎的语言（或至少是之一）。不只在商业领域流行，国内很多地区和教育机构正将Python纳入教材之中。比如Python进入山东小学六年级的教材，浙江信息技术教材将放弃VB，改用Python 语言，Python列入全国计算机二级等级考试大纲等。

### Python的未来发展

在Python发展过程中，Guido一直是核心人物，甚至被称为“终身仁慈独裁者”，但在2018年经历了退出管理层风波之后，他又在2019年以五大指导委员之一的身份重回决策层。这为Python迎来了新的治理方案：指导委员会模式。这种模式意味着Python的未来将从Guido一人决定变为5人决定，虽然比很多开源语言仍然有民主化空间（例如PHP的改进由社区投票决定），但也算是一种从专制到民主的进步。

有关Python的每个提升计划，都是在PEP（Python Enhancement Proposal）列表中——每个版本新特性和变化都通过PEP提案经过社区决策层讨论、投票决议，最终才有我们看到的功能。

目前，**Python的最新稳定的主版本是3.7**，Python 3.8也已经有了预览版，大概在2023年左右Python 4便会问世。在之后的时间里，Python会如何发展？我们可以从Python软件基金会的董事会成员、CPython的核心开发人员Nick Coghlan的信息中略知一二：

**首先**，Python的PEP流程和制度没有任何变化，通过增加新模块和功能来增强的基础能力。随着Python 2在2020年不再维护，社区在Python 3的资源和投入会相应增加。

**其次**，不同解释器的实现和功能扩展还将继续增强，方向包括PyPy关于JIT编译器生成和软件事务内存的尝试，以及科学和数据分析社区，对面向数组编程的探索等。

**再次**，嵌入式应用的增强，核心是与其他虚拟机运行时（如JVM和CLR）的集成和改进，尤其是在教育领域取得的进展，可能会让Python作为更受欢迎的嵌入式脚本语言，在更大的应用程序中运行。

**最后**，对于为了兼容和维持Python 2的部分功能而存在于Python 3中的原有代码，在后续版本中应该会逐步优化甚至去掉。而对于其他更改，则会根据情况弃用、提出警告、逐步替代以及保留。

目前最新版本：

![image-20231018083419453](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018083419453.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



# 二、正确了解Python

> 本段转载于[python语言的优点和缺点通俗易懂-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/2096787)
>
> [Python的3个主要缺点及其解决方案 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/138091695)

## 1、优点

1. 作为初学python的科班出身的小白，python非常简单，非常**适合人类阅读**。阅读一个良好的Python程序就感觉像是在读英语一样，尽管这个英语的要求非常严格！Python的这种伪代码本质是它最大的优点之一。它使你能够专注于解决问题而不是去搞明白语言本身。
2. 易学。python虽然是用c语言写的，但是它摈弃了c中非常复杂的指针，**简化了python的语法**。
3. Python是FLOSS（自由/**开放**源码软件）之一。简单地说，你可以自由地发布这个软件的拷贝、阅读它的源代码、对它做改动、把它的一部分用于新的自由软件中。Python希望看到一个更加优秀的人创造并经常改进。
4. **可移植性**————由于它的开源本质，Python已经被移植在许多平台上（经过改动使它能够工作在不同平台上）。如果你小心地避免使用依赖于系统的特性，那么你的所有Python程序无需修改就可以在下述任何平台上面运行。这些平台包括Linux、Windows、FreeBSD、Macintosh、Solaris、OS/2、Amiga、AROS、AS/400、BeOS、OS/390、z/OS、Palm OS、QNX、VMS、Psion、Acom RISC OS、VxWorks、PlayStation、Sharp Zaurus、Windows CE甚至还有PocketPC、Symbian以及Google基于linux开发的Android平台！
5. ==在计算机内部，Python解释器把源代码转换成称为字节码的中间形式，然后再把它翻译成计算机使用的机器语言并运行。==事实上，由于你不再需要担心如何编译程序，如何确保连接转载正确的库等等，所有这一切使得使用Python更加简单。由于你只需要把你的Python程序拷贝到另外一台计算机上，它就可以工作了，这也使得你的Python程序更加易于移植。
6. Python既支持**面向过程的函数编程**也支持**面向对象的抽象编程**。在面向过程的语言中，程序是由过程或仅仅是可重用代码的函数构建起来的。在面向对象的语言中，程序是由数据和功能组合而成的对象构建起来的。与其他主要的语言如C++和Java相比，Python以一种非常强大又简单的方式实现面向对象编程。
7. **可扩展性和可嵌入性**。如果你需要你的**一段关键代码运行得更快**或者**希望某些算法不公开**，你可以把你的部分程序用C或C++编写，然后在你的Python程序中使用它们。你可以把Python嵌入你的C/C++程序，从而向你的程序用户提供脚本功能。
8. **丰富的库**。Python标准库确实很庞大。python有可定义的第三方库可以使用。它可以帮助你处理各种工作，包括正则表达式、文档生成、单元测试、线程、数据库、网页浏览器、CGI、FTP、电子邮件、XML、XML-RPC、HTML、WAV文件、密码系统、GUI（图形用户界面）、Tk和其他与系统有关的操作。记住，只要安装了Python，所有这些功能都是可用的。这被称作Python的“功能齐全”理念。除了标准库以外，还有许多其他高质量的库，如wxPython、Twisted和Python图像库等等。
9. Python确实是一种十分精彩又强大的语言。它合理地结合了**高性能**与使得**编写程序简单有趣**的特色。
10. 规范的代码。Python采用**强制缩进**的方式使得代码具有极佳的可读性。
11. **动态类型**。Python不会检查数据类型，在声明变量时不需要指定数据类型。

## 2、缺点

### **不能将程序连写成一行**

如import sys;for i in sys.path:print i。而perl和awk就无此限制，可以较为方便的在shell下完成简单程序，不需要如Python一样，必须将程序写入一个.py文件。（对很多用户而言这也不算是限制）

即使在Python诞生30年后，Python依然没有很好的方法来生成可执行文件（exe程序等）

我们只能通过第三方工具解决。而且用起来比较麻烦。

### **运行速度慢**

有速度要求的话，用C++改写关键部分吧。不过对于用户而言，机器上运行速度是可以忽略的。因为用户根本感觉不出来这种速度的差异。

Python 整体性能缓慢，有限的线程和多处理能力是其未来发展的主要障碍。

Python长期以来一直重视编程的易用性而不是运行时的速度。当通过使用C或C++编写的高速外部库（如Numpy和Numba）在Python中完成如此多的性能密集型任务时，你会发现Python重视编程的易用性也是一种不错的选择。但是尽管如此，Python的开箱即用的性能速度依然落后于其他语言，比如说具有同样简单语法的Nim和Julia，却可以被编译为机器代码，具有更高的性能优势。

Python==无法全面利用多核处理器==是其长久以来的问题，它确实具有线程功能，但它的线程功能是局限于单个核心的。虽然Python可以使用多进程，但是调度和同步这些子进程的结果并不总是有效的

### **代码公开不加密**

既是优点也是缺点，python的开源性是的Python语言==不能加密==，但是目前国内市场纯粹靠编写软件卖给客户的越来越少，网站和移动应用不需要给客户源代码，所以这个问题就是问题了。随着时间的推移，很多国内软件公司，尤其是游戏公司，也开始规模使用他。

### **构架选择太多**

（没有像C#这样的官方.net构架，也没有像ruby由于历史较短，构架开发的相对集中。Ruby on Rails 构架开发中小型web程序天下无敌）。不过这也从另一个侧面说明，python比较优秀，吸引的人才多，项目也多。

### **Python 包管理、项目管理复杂**

当你想将一个本地比较复杂的Python工程移植到服务器上的时候，你就知道Python项目管理是有多蛋疼了

你需要不断地安装项目依赖，依赖的依赖可能还有依赖，就像俄罗斯俄罗斯套娃一样，恨不得直接把键盘吃了。

# 三、Python环境搭建以及Pycharm安装

> 参考文章：[【精选】（超详细）Python+PyCharm的安装步骤及PyCharm的使用（含快捷键）_python pycharm_IT路上的军哥的博客-CSDN博客](https://blog.csdn.net/junleon/article/details/120698578)

# 四、编写和运行程序

**交互方式**：

​	指我们每写一行Python代码，就可以敲回车来运行代码。

**文件方式**：

​	指先编写好Python代码文件（*.py），然后通过Python指令运行它，如果程序比较复杂，一般采用文件方式。

## 1、使用Python Shell（交互）

python shell其实简单来说，就是安装完python后它**自带的编译器**，不是特指某一项命令，而是一种命令行环境。我们可以在可以在shell里面调用库、执行语句。



<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018090743802.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231018090743802" style="zoom:50%;" />



![image-20231018090825773](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018090825773.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**可以直接编写代码语句**

![image-20231018091614918](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018091614918.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 2、使用IDLE（交互）

IDEL提供了有文本编辑器功能的菜单，在编写代码时还有一些语法提示。

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018091151257.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231018091151257" style="zoom:50%;" />



![image-20231018091712710](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018091712710.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



同样可以直接编写代码语句，而且还有代码提示和高亮

![image-20231018091933310](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018091933310.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 3、使用文本编辑工具-记事本（文件）

**注意事项**：在保存文件石，文件命名推荐全部采用小写英文字母，后缀名必须为py。另外，文件编码应该采用UTF-8。

![image-20231018093353870](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018093353870.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20231018093442874](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018093442874.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 4、使用IDE工具-Pycharm（文件）

**优点**：可以运行和调试代码

![image-20231018093721276](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018093721276.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231018093847560](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018093847560.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20231018101324383](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018101324383.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



# 五、基础知识

## 1、标识符

> 本段转载于[Python标识符-Python标识符是什么-Python标识符命名规范-Python合法标识符-嗨客网 (haicoder.net)](https://haicoder.net/python/python-identifier.html)
>
> [python——标识符及其命名规则 - 童话Bluebells - 博客园 (cnblogs.com)](https://www.cnblogs.com/Bluebells/p/14321930.html)

==Python3的字符采用了双字节Unicode编码。==

Unicode编码叫做统一编码制，包含了亚洲文字编码，如：中文、日文、韩文等字符。

所以，**中文也可以作为Python的标识符**。

**Python** 对各种 **变量**、**方法**、函数等命名时使用的字符序列称为标识符。

也可以说凡是自己可以起名字的地方都叫标识符，简单地理解，标识符就是一个名字，它的主要作用就是作为变量、函数、类、模块以及其他对象的名称。

### Python标识符的命名规则

- Python 标识符由 `26` 个英文字母大小写，0-9 ，_ 组成。
- Python 标识符不能以数字开头，可以是下划线或字母。
- Python 标识符**严格区分大小写**。
- Python 标识符不能包含空格、@、% 以及 $ 等特殊字符。
- 不能以系统保留关键字作为标识符（一共有25 个）。
-  在 Python 中，所有标识符可以包括英文、数字以及下划线(_)，但不能以数字开头。
- 不要使用Python的内置函数作为自己的标识符。

### Python标识符的命名注意事项

- Python 标识符尽量采取有意义的包名，简短，有意义，**不要和系统保留关键字冲突**。
- Python 标识符以单下划线开头的标识符，表示不能直接访问的类属性，其无法通过 import 的方式导入。
- 以双下划线开头的标识符表示类的私有成员。
- 以双下划线作为开头和结尾的标识符，是专用标识符。
- Python 标识符是**允许使用汉字作为标识符**的。

### Python标识符规范

- 当标识符用作**模块名**时，应尽量短小，并且**全部使用小写字母**，可以**使用下划线**分割多个字母。
- 当标识符用作**包的名称**时，应尽量短小，也**全部使用小写字母**，不推荐使用下划线。
- 当标识符用作**类名**时，应采用单词**首字母大写**的形式。
- 模块内部的**类名**，可以采用 “**下划线+首字母大写**” 的形式。
- 函数名、类中的属性名和方法名，应全部使用小写字母，多个单词之间可以用下划线分割。
- **常量命名应全部使用大写字母**，单词之间可以用下划线分割。

## 2、关键字

python的**keyword模块**记录了python所有的关键字，

它的作用是避免因为变量命名冲突而造成异常。他所有的关键字都已列表的形式存放在kwlist属性中。

![image-20231018110238735](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018110238735.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```python
import keyword

list = keyword.kwlist

for i in range(0, len(list)):
    print(list[i].ljust(10), end="")
    if (i+1) % 5 == 0 and (i-1) != 0:
        print()
```

==待之后慢慢填充==


|  关键字   | 作用 | 用例 |
| :-------: | :--: | :--: |
|   False   |      |      |
|   None    |      |      |
|   True    |      |      |
|    and    |      |      |
|    as     |      |      |
|  assert   |      |      |
| **async** |      |      |
| **await** |      |      |
|   break   |      |      |
|   class   |      |      |
| continue  |      |      |
|    def    |      |      |
|    del    |      |      |
|   elif    |      |      |
|   else    |      |      |
|  except   |      |      |
|  finally  |      |      |
|    for    |      |      |
|   form    |      |      |
|  global   |      |      |
|    if     |      |      |
|  import   |      |      |
|    in     |      |      |
|    is     |      |      |
|  lambda   |      |      |
| nonlocal  |      |      |
|    not    |      |      |
|    or     |      |      |
|   pass    |      |      |
|   raise   |      |      |
|  return   |      |      |
|    try    |      |      |
|   while   |      |      |
|   with    |      |      |
|   yield   |      |      |

## 3、变量

> 本段转载于[Python语法入门之变量 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/108679428)
>
> [Python变量：变量的定义、赋值、修改、删除等操作 (zhihu.com)](https://www.zhihu.com/tardis/zm/art/615176094?source_id=1005)

### 为什么需要变量

变量就是**可以变化的量**，量指的是事物的状态，比如人的年龄、性别，游戏角色的等级、金钱等等

为了让计算机能够像人一样去记忆事物的某种状态，并且状态是可以发生变化的
		详细地说：**程序执行的本质就是一系列状态的变化**，变是程序执行的直接体现，所以我们需要有一种机制能够反映或者说是保存下来程序执行时状态，以及状态的变化。

Python变量是**用于存储数据的标识符**。变量可以存储各种类型的数据，例如数字、字符串、列表、字典等。在Python中，变量的定义、赋值、修改、删除等操作非常简单。

在Python中为一个**变量赋值的同时就声明了该变量**，可以推导出来

该变量的数据类型就是赋值数据所属的类型，该变量==还可以接收其他类型的数据==（容易导致严重的Bug）。



### 变量的定义

在Python中，可以使用任何名称来定义变量，只要满足以下条件：

- 变量名**只能包含字母、数字和下划线**。
- 变量名**必须以字母或下划线开头**。
- 变量名不能是Python关键字，如if、while、for等。

变量的定义非常简单，只需要指定变量名，然后使用等号将其赋值给一个值。例如：

```python
x = 5
y = "Hello, world!"
```

在上面的示例中，变量x被赋值为5，变量y被赋值为字符串"Hello, world!"。

### 变量的赋值

可以通**过简单地为变量赋值来修改变**量的值。例如：

```python
x = 5
x = 6
```

在上面的示例中，变量x的值由5更改为6。

### 变量的修改

Python中的变量是可变的，这意味着可以修改变量的值。例如：

```python
x = [1, 2, 3]
x[0] = 4
```

在上面的示例中，变量x的值由[1, 2, 3]更改为[4, 2, 3]。

### 变量的删除

可以使用del语句删除变量。例如：

```python
x = 5
del x
```

在上面的示例中，变量x被删除了。

### 变量的类型

Python中的变量不需要事先声明其类型，它们是**动态类型**的。这意味着**变量可以在程序执行期间分配任何类型的值**。可以使用**type()函数获取变量的类型**。例如：

```python
x = 5
y = "Hello, world!"
print(type(x))
print(type(y))
```

在上面的示例中，输出是：

```shell
python
<class 'int'>
<class 'str'>
```

这意味着变量x是整数类型，变量y是字符串类型。

### 变量的命名规范

在Python中，有一些命名规范应该遵循：

- 变量名应该是**描述性**的，易于阅读。
- 变量名应该使用**小写字母和下划线**。
- 变量名应该以单词之间的**下划线分隔**，而**不是使用驼峰命名法**。
- 变量名**应该避免使用缩写**，除非它们是广泛理解的缩写。



### 变量的作用域

在Python中，变量的作用域指的是可以访问变量的代码块。Python中有三种类型的变量作用域：

- 局部变量：定义在函数内部，只能在函数内部访问。
- 全局变量：定义在函数外部，可以在整个程序中访问。
- 嵌套作用域变量：定义在一个函数内部的函数中，只能在这个函数内部和嵌套的函数中访问。

以下是一个使用局部变量和全局变量的示例：

```python
x = 5  # 全局变量

def my_func():
    x = 10  # 局部变量
    print("x = ", x)

my_func()
print("x = ", x)
```

在上面的示例中，函数my_func()中的变量x是一个局部变量。当函数被调用时，Python将在函数内部创建一个名为x的新变量，并将其值设置为10。当函数返回时，这个变量将被销毁。在函数外部，变量x仍然是全局变量，并且它的值仍然是5。

### 变量的多重赋值

在Python中，可以使用**多个变量同时赋值**。例如：

```text
x, y = 1, 2
```

在上面的示例中，变量x被赋值为1，变量y被赋值为2。这与以下代码

的效果是一样的：

```text
x = 1
y = 2
```

可以在**多个变量之间交换它们的值**。例如：

```text
x, y = y, x
```

在上面的示例中，变量x和变量y的值被交换了。

### 变量的命名约定

在Python中，有一些命名约定应该遵循：

- 变量名应该尽量短，但仍然保持描述性。
- 变量名应该使用小写字母和下划线。
- 变量名应该以单词之间的下划线分隔，而不是使用驼峰命名法。
- 变量名应该避免使用单个字符，除非它们是循环计数器或其他简单用途的变量。
- 变量名应该避免使用Python内置函数和关键字的名称。

例如，下面是一些良好的变量名：

```python
name = "John"
age = 30
is_valid = True
```

而下面是一些不好的变量名：

```python
n = "John"  # 变量名过短，缺少描述性
a = 30  # 变量名过短，缺少描述性
valid = 1  # 变量名不够描述性
if = True  # 变量名使用了Python关键字
```

## 4、语句

在Python中，一行代码表示一条语句，在一般情况下**语句结束时不加分号**

链式赋值语句可以给多个变量赋相同的数值

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018144821104.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231018144821104" style="zoom: 50%;" />



同时给多个变量赋值，用逗号隔开

![image-20231018145210836](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018145210836.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



![image-20231018145451168](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018145451168.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 5、代码注释

### 单行注释

![image-20231018152909435](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018152909435.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 多行注释

**多行注释通常用来为 Python 文件、模块、类或者函数等添加版权或者功能描述信息。**

- Python 多行注释不支持嵌套

- 不管是多行注释还是单行注释，当注释符作为字符串的一部分出现时，就不能再将它们视为注释标记，而应该看做正常代码的一部分

![image-20231018160255370](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018160255370.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 注释可以帮助调试程序

**给代码添加说明**是注释的基本作用，除此以外它还有另外一个实用的功能，就是用来**调试程序**。

举个例子，如果你觉得某段代码可能有问题，可以先把这段代码注释起来，让 Python 解释器忽略这段代码，然后再运行。如果程序可以正常执行，则可以说明错误就是由这段代码引起的；反之，如果依然出现相同的错误，则可以说明错误不是由这段代码引起的。

在调试程序的过程中**使用注释可以缩小错误所在的范围**，提高调试程序的效率。

### 文件头部声明  # coding=utf-8

> 本段转载于[python文件头部声明# coding=utf-8_python coding=utf-8_冰美式QAQ的博客-CSDN博客](https://blog.csdn.net/daningliu/article/details/121617391)

python2默认的编码格式是**ASCII**格式，python3默认的编码格式是**utf-8**格式。

**注意**：# coding=utf-8 的 = 号两边不要空格。

python3环境中，源码文件默认使用utf-8编码，可以正常解析中文，不需要开头加上面的代码，但是**为了代码的可移植性，建议在编写程序的时候加上**。

另外，使用编辑器编写python程序时，还需要设置py文件存储的格式为UTF-8，否则会出现乱码或者报错。

```python
import sys
print("当前环境的默认编码格式为:"+sys.getdefaultencoding())
```

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018161718263.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231018161718263" style="zoom: 33%;" />

## 6、模块和包

> 本文转载于[详解Python中模块(Module)和包(package)的概念和用法 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/70556072)
>
> [Python中“if __name__=='__main__':”详细解析 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/340997807)

实际上，Python中的==函数==(Function)、==类==(Class)、==模块==(Module)、==包库==(Package)，都是为了实现模块化引用，让程序的组织更清晰有条理。

👉通常，函数、变量、类存储在被称为模块(Module)的.py文件中，一组模块文件又组成了包(Package)。

👉将函数、变量、类存储在存储在独立的.py文件中，可隐藏代码实现的细节，将不同代码块重新组织，与主程序分离，简化主程序的逻辑，提高主程序的可读性。

👉 有了包和模块文件，可以在其他不同程序中进行复用，还可以使用其他人开发的第三方依赖库。

### （1）模块化编程

了解这两个概念，有助于我们更好地使用python进行**模块化编程**，通过模块化编程，我们能把大的工程拆分成小的子任务和子模块，在比较大的项目中，进行模块化编程的好处有以下几点：

1. 简化编程，不必把重点放在整个项目上了；
2. 可维护性好，即使出了问题也便于排查；
3. 复用性好，直接使用编写好的模块去实现功能，当需要重复实现时，再次调用即可，不必再重新编写了；
4. 范围性好，这个的意思就是每个模块都有单独的命名空间，避免发生一些例如变量命名上的冲突

在编程中多多使用函数，**模块和包能够提升模块化编程**。

### （2）命名与命名空间

#### 命名

每个变量都拥有一个名字，这个就是命名，**给变量命名**。变量命名也是让很多程序员头疼的一件事情，怎么样能起一些有意义，又高大上的名字。在Python中，**一切皆对象**，我们甚至可以给一个函数一个命名，命名就可以理解**为所有对象的一个引用的名称**。

#### 命名空间

命名空间就是用来**保证命名之间不发生冲突**的规则，分为：

- 局部命名空间：在一个程序中为每个函数创建的命名空间，当函数执行完毕就失效
- 全局命名空间：在程序中为所有模块创建的命名空间，当程序执行完毕失效
- 内置命名空间：也就是默认的一些命名，退出程序失效

### （3）模块

`python`给我们提供了十分简单的方法去创建一个模块，我们只需要写一个`python`文件即可，也就是说写一个`.py`为后缀的文件，不必用额外的语法。

在Python中**一个模块就是一个文件**，模块是保存代码的最小单位，在模块中可以声明变量、函数、属性和类等Python代码元素。

三种从模块之间相互访问的方式：

例如：==现在我们要在in中访问out中的cat==

out:

```python
cat = "我是out中的一只猫"
```


- import <模块名>   （**用于导入别人模块中的所有元素**）

in:

```python
import out

print(out.cat)
```

- form <模块名> import <代码元素>   （**用于导入别人模块中的某个元素**）

in:

```python
from out import cat

print(cat)
```

- form <模块名> import <代码元素> as <元素别名>    （**用于某个变量或函数命名存在冲突**）

```python
from out import cat as cat_out

cat = "我是in中的一只猫"
print(cat_out)
```

#### 扩展

在 **import out** 时，Python解释器都干了什么？

解释器主要是在如下几个路径中搜索`mod.py`文件：

1. 首先在当前执行的文件所在的文件夹中查看是否存在，如果当前文件夹不包含`mod.py`文件，那么这个搜索就失败了；
2. 在系统设置的python环境变量下的一些文件夹里面；
3. 一些在python安装时指定的文件夹下面；

可以使用以下命令查看：

```python
import sys

for i in range(0, len(sys.path)):
    print(sys.path[i])
```

```xml
D:\Program\AllCode\Python-Code\hello2\test\Scripts\python.exe D:\Program\AllCode\Python-Code\hello2\in.py 
D:\Program\AllCode\Python-Code\hello2
D:\Program\AllCode\Python-Code\hello2
D:\Program\Tools\PyCharm\PyCharm 2023.2.2\plugins\python\helpers\pycharm_display
D:\Program\Environments\Python\python312.zip
D:\Program\Environments\Python\DLLs
D:\Program\Environments\Python\Lib
D:\Program\Environments\Python
D:\Program\AllCode\Python-Code\hello2\test
D:\Program\AllCode\Python-Code\hello2\test\Lib\site-packages
D:\Program\Tools\PyCharm\PyCharm 2023.2.2\plugins\python\helpers\pycharm_matplotlib_backend
```

来查看在路径搜索时，都有哪些路径，当然搜索的结果因为安装，版本和操作系统的原因都不会相同，每个人的结果可能都不会相同。

因此，当我们`import`一些模块出现问题的时候，我们可以查看这个模块文件是不是在搜索路径中。

当我们想要把自己写的文件作为一个模块的时候，但是**又不在搜索路径中**，我们可以**自己添加**进去。

```python
import sys

sys.path.append("C:\\Users\\15879")
print(sys.path[len(sys.path) - 1])
```

```xml
C:\Users\15879
```

单独运行模块
如果我们想单独测试下模块，可以在模块中添加以下代码，就可以既用作脚本，也可用作可导入模块：

```python
if __name__ == "__main__":
    import sys
    fib(int(sys.argv[1]))
```

单独运行模块：

```python
python fibo.py 100
```

这段解析命令行的代码仅在**模块作为“主”文件执行时**才运行。

__name__属性是Python的一个内置属性，记录了一个字符串。

- 若是在当前文件，__name__ 是__main__。
- 在demo2文件中打印本文件的__name__属性值，显示的是__main__
- 若是导入的文件，__name__是模块名。
- demo2文件导入demo模块，在demo2文件中打印出demo模块的__name__属性值，显示的是demo模块的模块名。

因此__name__ == '__main__' 就表示在当前文件中，可以在if __name__ == '__main__':条件下写入测试代码，如此可以避免测试代码在模块被导入后执行。

![image-20231019101753916](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019101753916.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### （4）包

> 本段转载于[【精选】详解Python模块化——模块（Modules）和包（Packages）_python包与模块-CSDN博客](https://blog.csdn.net/Bit_Coders/article/details/119318000)

简单来说，包就是多个模块的集合。当项目较大，模块较多时，我们就可以把模块放在包中，便于管理。

在python3.3版本之前，初始化一个包必须包含`__init__.py`文件，之后这就不必备的文件了，但是一般都会包含，不过需要配置，我们就在这个文件中写入一些指令，如果不需要的话，空文件也可以。在引用包中的模块时，使用`.`操作符即可，**前提是在不同的包中**，同样也要注意是不是在搜索路径中。

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018191325854.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231018191325854" style="zoom: 67%;" />



```python
from animals.dog import dog
print(dog)
```

`__init__.py` 必须有这个文件，才能使 Python 将包含该文件的目录视为包（Package）。`__init__.py`可以是一个空文件，也可以执行包的初始化代码或设置`__all__`变量

`from animals.dog import dog`语句会先测试item是否在包中定义；如果包中没有找到定义，会假定item是一个模块并尝试加载它。如果依旧找不到item， 就会引发我们常见的`ImportError异常`。

#### 利用相对路径引用包和模块

在orange中

```python
from . import apple
from .. import animals
from ..animals import dog
```


这里的 ==.== 可以访问同级目录下的包（Package）或者模块（Module）。
这里的 ==..== 可以访问上一级目录下的包（Package）或者模块（Module）。

#### 利用__ all __提供包的显式索引

当我们直接采用from sound.effects import *时，可能会引用一些不需要的内容，或者导致加载速度过慢。

这时我们可以通过在__init__.py中定义一个_all__列表，来指定用 * 时应导入的模块名称列表：

```python
__all__ = ["echo", "surround", "reverse"]
```

这样我们就可以维护在import * 时需要导入的模块列表，在发布不同版本的包时很有用。

## 7、动态类型(==候补==)

> 本段转载于[Python动态强类型解释型语言原理解析-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1742333)
>
> [强类型与动态类型的Python - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/91117079)

# 六、内置数据类型

使用函数 **type( )**可查看变量的类型

## 1、数字
> 本段转载于[Python中的数字类型格式与运算 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/135287353)
>
> [【精选】Python整数类型（int）、小数/浮点数（float）、复数类型（complex）_学不会is dog的博客-CSDN博客](https://blog.csdn.net/yelitoudu/article/details/117407685)
>
> [Python六大基本数据类型介绍_python数据类型有哪些-CSDN博客](https://blog.csdn.net/qq_39787513/article/details/106939265)

### （1）整数类型

**int**

在Python中整数类型（简写为int）又称为整型，由正整数、0、负整数构成，不包括小数、分数。在Python中整数的长度不受限制，但是**受到可用内存的限制**。

**注意**：二进制、十进制、八进制、十六进制的数均为整型数

- 有些强类型的编程语言会提供多种整数类型，每种类型的长度都不同，能容纳的整数的大小也不同，开发者要根据实际数字的大小选用不同的类型。例如`C语言`提供了 `short、int、long、long long` 四种类型的整数，它们的长度依次递增，初学者在选择整数类型时往往比较迷惑，有时候还会导致数值溢出。
- 而 Python 则不同，它的整数不分类型，或者说它只有一种类型的整数。`Python 整数的取值范围是无限的，不管多大或者多小的数字，Python 都能轻松处理`。

`当所用数值超过计算机自身的计算能力时，Python 会自动转用高精度计算（大数计算）。`

#### 数字分隔符

- 为了提高数字的的可读性，Python 3.x 允许使用下划线_作为数字（包括整数和小数）的分隔符。通常每隔三个数字添加一个下划线，类似于英文数字中的逗号。下划线不会影响数字本身的值。

![image-20231018203351549](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018203351549.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （2）浮点类型

**float**

浮点数（float）又称为小数，在数学中对应的是实数，在Python中浮点数是带小数点的数字。由于电脑内存中存储的浮点数的位数有限，所以超过指定长度后，末尾将采取近似值。所以浮点数并不一定是精确值。**双精度浮点类型**

**表达式中存在浮点数，计算结果一定是浮点数。**

在编程语言中，小数通常以浮点数的形式存储。浮点数和定点数是相对的：小数在存储过程中如果小数点发生移动，就称为浮点数；如果小数点不动，就称为定点数。

**注意，只要写成指数形式就是小数，即使它的最终值看起来像一个整数。例如 14E3 等价于 14000，但 14E3 是一个小数。**

![image-20231018204509467](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018204509467.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**Python 能容纳极小和极大的浮点数。print 在输出浮点数时，会根据浮点数的长度和大小适当的舍去一部分数字，或者采用`科学计数法`。**

==特例==：

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018204019610.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231018204019610" style="zoom:50%;" />



原因：**这是因为小数在内存中是以二进制形式存储的，小数点后面的部分在转换成二进制时很有可能是一串无限循环的数字，无论如何都不能精确表示，所以小数的计算结果一般都是不精确的**。

### （3）复数类型

**complex**

复数（Complex）由实部和虚部组成，把实数扩展到虚数，它的数学表示形式为a+bj(a、b均为实数)。a称为实部，b称为虚部，j（J）为虚数单位（j²=-1），bj称为虚数。

- **复数（Complex）** 是 [Python](http://c.biancheng.net/) 的内置类型，直接书写即可。换句话说，Python 语言本身就支持复数，而不依赖于标准库或者第三方库。
- **复数由实部`（real）`和虚部`（imag）`构成，在 Python 中，复数的虚部以j或者J作为后缀**，具体格式为：

```python
a + bj # a 表示实部，b 表示虚部。
```

#### 显式声明

```python
complexvar = 3-91j
print (complexvar,type(complexvar))
```

#### 隐式声明

```python
complexvar = complex(3,-91)
print (complexvar,type(complexvar))
```

**两种声明方式，结果一样**

### （4）布尔类型

**boolean**

布尔(Boolean)又称为逻辑值，在Python中用**True和False**表示，可以用于逻辑判断。这种数据类型是一种特殊的整数类型。True可以用1替换，代表为"真"；False可以用0替换，代表为"假"。

Python中任何类型的数据都可以通过**bool( )**函数转换为布尔值，

那些被认为**没有的**、**空的**值会被转换为**False**

反之被转换为**True**

### （5）数字类型的相互转换

除复数外，其他3个两两之间可以相互转换

1. 隐式转换

**浮点数 > 整数 > 布尔**

![image-20231018210829097](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018210829097.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



2. 显式转换

函数 **int( )**、**float( )**、**bool( )**

一般默认**向下取整**

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018211436026.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" style="zoom: 50%;" />



## 2、序列（sequence）

> 本段转载于[Python 数据类型：序列（Sequence） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/616818060)

**容器类型**：可以容纳多项数据

序列是一种可迭代的、**元素有序** 、**可重复** 的容器类型的数据

包括列表、字符串、元组、字节序列（bytes）

### 序列的索引操作

- 序列中每个元素都有属于自己的编号（索引）。从起始元素开始，索引值从 0 开始递增：

![动图封面](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/v2-ab685bd9dabbff15666b1f4fb83b5660_b.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





- Python 还支持索引值是负数，此类索引是从右向左计数（从最后一个元素开始计数，从索引值 -1 开始）。



![动图](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/v2-789a5072877eb122b75ed4b39e4b9f0c_b.webp?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)





- 注意：使用负值作为列序中各元素的索引值时，是从 -1 开始，而不是从 0 开始。无论是采用正索引值，还是负索引值，都可以访问序列中的任何元素。

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019142431462.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231019142431462" style="zoom:50%;" />

max( )、min( )两个函数用于返回在序列s中ASCII码最大、最小字符

![image-20231019170828723](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019170828723.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 类型转换函数

1.内置函数 **list()** # 转换为列表。

2.内置函数 **tuple()** # 转换为元组。

3.内置函数 **dict()** # 转换为字典。

4.内置函数 **set()** # 转换为集合。

 5.内置函数 **str()** # 转换为字符串。

### 序列的加和乘

- **加**操作：类似于拼接
- **乘**操作：类似于幂值

<img src="https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019171256163.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10" alt="image-20231019171256163" style="zoom: 50%;" />



### 切片操作

切片操作是访问序列中元素的另一种方法，它可以访问**一定范围内**的元素，通过切片操作，可以生成一个**新的序列**。

**语法格式**：sname [ start  **:**  end  :  step ]

==下面的参数中，若为-1，说明是从右往左开始数==

==序列的最后一个值的位置，即是len(s)-1，也是-1==

```python
s = 'hello'
print(s[len(s) - 1])
print(s[-1])
```

```xml
o
o
```

- `sname`：序列的名称
- `start`：切片的开始索引位置（**包括该位置**），此参数也可以不指定，会**默认为 0**，也就是从序列的开头进行切片
- `end`：表示切片的结束索引位置（**不包括该位置**），如果不指定，则**默认为序列的长度**。
- `step`：表示在切片过程中，隔几个存储位置（包含当前位置）取一次元素，也就是说，**如果 step 的值大于 1**，则在进行切片去序列元素时，会“跳跃式”的取元素。如果省略设置 step 的值，则最后一个冒号就可以省略；**如果step的值为负数**，将会**从右往左**获取元素。**默认为1**。

### 序列成员检测

Python 中可以使用 **in 关键字**检查某元素是否为序列的成员，返回一个布尔类型的值

语法格式：

==value in sequence==

- `value`：要检查的元素
- `sequence`：指定的序列

**not in** 和 in 关键字用法相同，功能恰好相反

![image-20231019181438653](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019181438653.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 3、字符串（str）

> 本段转载于[Python语法必备篇——Python字符串 学习-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1915438)
>
> [Python入门 字符串处理（字符串连接\转义\字符串运算\字符串的多种引号区分\切片\常用函数） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/28879694)
>
> [Python基础教程之Python 字符串(String) 详解_python string-CSDN博客](https://blog.csdn.net/Soinice/article/details/109330172)
>
> [A-Z,a-z,0-9的unicode编码表 - Andhui - 博客园 (cnblogs.com)](https://www.cnblogs.com/huigebj/p/11424684.html)
>
> [转义字符对照表 - TabKey9 - 博客园 (cnblogs.com)](https://www.cnblogs.com/tabkey9/p/15930390.html)
>
> [python格式化字符串的三种方法（%，format，f-string)-CSDN博客](https://blog.csdn.net/zjbyough/article/details/96466658)
>
> [python字符串格式化深入详解（四种方法）_怎么表示{} 格式化python-CSDN博客](https://blog.csdn.net/qq_27825451/article/details/105652244)

序列的一种

一种不可变的字符序列

`字符串`的意思跟字面意思很像，就是“**一串字符**”，字符串是 Python 中最常用的数据类型。

Python 要求字符串必须使用引号括起来，使用**单引号**也行，使用**双引号**也行，只要**两边的引号能配对即可**。

Python3 直接支持 **Unicode**，可以**表示世界上任何书面语言的字符**。

Python3 的字符默认就是 16 位 Unicode 编码，ASCII 码是 Unicode 编码的子集。

### （1）字符串的表示方式

- 普通字符串

```python
s1 = 'hello'
s2 = "hello"
s3 = "hello '你好' "
s4 = 'hello "你好" '
s5 = '\u0068\u0065\u006c\u006c\u006f'
s6 = 'hello "你好"我是张三""'
print(s1)
print(s2)
print(s3)
print(s4)
print(s5)
print(s6)
```

```xml
hello
hello
hello '你好' 
hello "你好" 
hello
hello "你好"我是张三""
```



![image-20231021152320408](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021152320408.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



- 原始字符（raw string）

![image-20231021152517543](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021152517543.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**那如何在字符串中打印 \n 这种字符呢？**

在普通字符串前加r就是原始字符串了

```python
s1 = "hello\nworld"
s2 = r"hello\nworld"
print(s1)
print(s2)
```

```xml
hello
world
hello\nworld
```

==拓展：==

![image-20231021152604411](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021152604411.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 长字符串

![image-20231021153848265](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021153848265.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （2）字符串与数字的相互转换

数字和字符串是两种 **不兼容** 的数据类型，不能进行 **隐式转换**，

只能够通过 **函数** 进行 **显式转换**。

int(字符串,需要转换的进制)、float(字符串)、str(整型数、浮点型数、布尔型数)

### （3）格式化字符串

Python格式化字符串有三种方法，第一是早期就有的%，其次是2.5之后的format(),还有就是3.6添加的f字符串调试

- 使用str()函数直接拼接

```python
result = "3 * 4 = " + str(3*4)
print(result)
```

```xml
3 * 4 = 12
```

- %格式化字符串

![image-20231021171438148](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021171438148.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

%格式化字符串是python最早的，也是能兼容所有版本的一种字符串格式化方法，在一些python早期的库中，建议使用%格式化方式，他会把字符串中的格式化符按顺序后面参数替换

另外，比如我要**固定字符的宽度**，**小数精度**等，可以用如下的方式，对格式进行进一步的控制：

**%[ ( name ) ] [ flags ] [ width ].[precision] typecode**

（1）(name)为命名：即参数的名称，可以没有这个，怎么使用呢？注意（name需要使用括号括起来哦！！！）

​		注意：这里的name，num括号不能掉

```python
'Hey %(name)s, there is a %(num)f number!' % {"name": name, "num": number }
```

（2）flags可以有+,-,' '或0。+表示右对齐。-表示左对齐。' '为一个空格，表示在正数的左侧填充一个空格，从而与负数对齐。0表示左侧使用0填充。

（3）width表示显示宽度

（4）precision表示小数点后精度

**注意：百分号% 来格式化字符串是最早出现的，python里面称之为printf风格的字符串格式化**

```python
"xxxxxx %s xxxxxx" % (value1, value2)
```

其中 %s就是格式化符，意思是把后面的值格式化为字符类型，类似的格式化符还有%d,%f等，具体参考文章[Python字符串格式化](https://www.cnblogs.com/nutix/p/4504899.html)

后面的value1,value2就是要格式化的值，不论是字符还是数值，都会被格式化为格式化符对应的类型

当然可以不用以元组的形式传值，你可以直接写这样："xxxxx %s" % value，不过不建议这样写，一是应为这样只能传递一个参数，二是如果value是元组或列表等类型，这样会触发TypeErrer

如果只传一个参数，并且很确定参数类型不会触发异常，可以使用上面的写法，否则，我建议你提供一个单元素元组，就像"xxxx %s " % (value,)

```python
name = "张三"
age = 18
print("%s今年%d岁了" % (name, age))
```

```xml
张三今年18岁了
```

- ####  format()

> 本段转载于[python格式化字符串的三种方法（%，format，f-string)-CSDN博客](https://blog.csdn.net/zjbyough/article/details/96466658)

(1)使用默认的占位符

```python
name = "张三"
age = 18

print('{}今年{}岁了'.format(name,age))
```

```xml
张三今年18岁了
```

(2)使用序号占位符

```python
name = "张三"
age = 18

print('{0}今年{1}岁了'.format(name, age))
```

```xml
张三今年18岁了
```

(3)使用参数名占位符

```python
name = "张三"
age = 18

print('{name}今年{age}岁了'.format(name=name, age=age))
```

```xml
张三今年18岁了
```



字符串类型格式化**采用format()方法**，基本使用格式是：

```python
 <模板字符串>.format(<逗号分隔的参数>)
```

format()方法中<模板字符串>的槽除了包括参数序号，还可以包括**格式控制信息**。

此时，槽的内部样式如下：

{<参数序号>: <格式控制标记>}   # **中间使用了一个冒号**哦！eg:**{1,d}**

其中，<格式控制标记>用来控制参数显示时的格式，包括：**<填充><对齐><宽度><,><.精度><类型>6 个字段**，这些字段都是可选的，可以组合使用，逐一介绍如下。

![image-20231021172535895](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021172535895.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- ####  f-string

**f'{}'**

f-string是2015年python 3.6 根据PEP 498新添加的一种字符串格式化方法，

f-string实际上是**在运行时计算的表达式**，而不是常量值。

在Python源代码中，f-string是一个文字字符串，前缀为’f’，其中包含大括号内的表达式。

表达式会将大括号中的内容替换为其值。

```python
import datetime
name = "zings"
age = 17
date = datetime.date(2019,7,18)
print(f'my name is {name}, this year is {date:%Y},Next year, I\'m {age+1}')  
# my name is zings, this year is 2019,Next year, I'm 18
```



==居中对齐==

![image-20231021214503597](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021214503597.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

除非**定义了最小字段宽度**，否则字段宽度将始终与填充它的数据大小相同，因此在这种情况下，对齐选项没有意义。

如果指定了align值，则可以在其前面加上可以是任何字符的填充字符，如果省略则默认为空格。 

无法使用文字大括号（“{”或“}”）作为格式化字符串文字中的填充字符或使用str.format（）方法。 

但是，可以插入带有嵌套替换字段的大括号。

```python
name = "张三"
print(f'{name:^18}')
```

```xml
        张三        
```

==对数字进行操作==

![image-20231021214919012](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021214919012.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （4）操作字符串

**注意：**在Python文档中[ ]表示可以省略部分内容，find()方法的参数[,start[,ebd] ]表示start和end都可以省略。

![image-20231021215504696](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021215504696.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231021215529336](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021215529336.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231021215551436](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021215551436.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231021215619608](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021215619608.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （5）案例：统计单词出现的次数

```python
passage = """
Afraid only afraid the light is suddenly put out in 
the-endless dark night and Countless loneliness.
"""


def count_word(passage):
    passage = str(passage)
    passage = passage.replace(',', '').replace('!', '').replace('.', '').replace('?', '')

    word_list = passage.split()

    count = []
    for word in word_list:
        count.append(word_list.count(word))
    return dict(zip(word_list, count))


print(count_word(passage))
```

```xml
{'Afraid': 1, 'only': 1, 'afraid': 1, 'the': 1, 
'light': 1, 'is': 1, 'suddenly': 1, 'put': 1, 
'out': 1, 'in': 1, 'the-endless': 1, 'dark': 1,
'night': 1, 'and': 1, 'Countless': 1, 'loneliness': 1}
```

### （6）拓展

==字符串切片==

![image-20231021230149164](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021230149164.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

==字符串的成员检测==

![image-20231021230240845](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021230240845.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

==三引号的作用==

Python三引号允许一个字符串跨多行，字符串中可以包含换行符、制表符以及其他特殊字符

![image-20231021230447836](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021230447836.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

==input（）函数==

input() 函数用于向用户生成一条提示，然后获取用户输入的内容。

由于 input() 函数总会将用户输入的内容放入字符串中，因此用户可以输入任何内容，input() 函数总是**返回一个字符串**。

```python
msg = input("请输入一个正整数:")
print(type(msg))
print(msg)
```

```xml
请输入一个正整数:8
<class 'str'>
8
```

## 4、列表（list）

> 本段转载于[Python基础知识点——list（列表）讲解 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/185015796)
>
> [python之列表（列表的所有操作）详细！！！_python列表命令-CSDN博客](https://blog.csdn.net/f066314/article/details/126944263)

**容器类型**

序列的一种

列表是一种可变的、**有序**的数据结构，可以随时追加、插入、删除和替换其中的元素。

列表非常适合利用顺序和位置定位某一元素，尤其是当元素的顺序或内容经常发生改变时。与字符串不同，列表是可变的。你可以直接对原始列表进行修改：添加新元素、删除或覆盖已有元素。

![image-20231019184629866](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019184629866.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （1）创建列表

- 方式1：**list( iterable )函数**

参数iterable是可迭代对象，如：字符串、列表、元组、集合和字典

- 方式2：**[元素1，元素2，元素3，...]**

列表中可以放**多种不同类型**的数据

![image-20231019184148782](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019184148782.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### （2）追加元素

![image-20231019191633354](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019191633354.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 追加单个元素

**append（x）**，x为单个元素的值，类型不确定

- 追加多个元素

使用 **+** 运算符，或者 **extend（t）**方法 ，其中 t 是一个可迭代对象

```python
list = [1, 2, 3]
print(list)

list.append(4)
print(list)

t = [4, 5, 6]
list += t
print(list)

list.extend(t)
print(list)
```

```xml
[1, 2, 3]
[1, 2, 3, 4]
[1, 2, 3, 4, 4, 5, 6]
[1, 2, 3, 4, 4, 5, 6, 4, 5, 6]
```

==拓展==：

在Python中方法和函数是有区别的。

**方法 **属于类，通过类或对象调用方法，例如在 **list.append(x)**中，list是列表对象；

**函数**不隶属于任何类，直接调用即可，例如 **list(iterable)**

### （3）插入元素

**insert(索引位置 , 要插入的元素)**

```python
list=[1,2,3,4]
list.insert(3,3)
print(list)
```

```xml
[1, 2, 3, 3, 4]
```

### （4）替换元素

```python
list=[1,2,3,4]
list[1]=3
print(list)
```

```xml
[1, 3, 3, 4]
```

### （5）删除元素

![image-20231019193103520](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019193103520.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （6）查找元素

**index(obj,start,stop)**

![image-20231019193444144](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019193444144.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （7）其它操作

|    函数     |                             作用                             |                       示例                        |
| :---------: | :----------------------------------------------------------: | :-----------------------------------------------: |
|   sort()    | sort()：默认对列表中的元素从小到大排序。sort(reverse = True) ：列表中的元素按从大到小进行排序。 |             list.sort(reverse = True)             |
|  reverse()  |                      使列表中的元素反转                      |                  list.reverse()                   |
|   count()   |                      统计元素出现的个数                      |                  list.count('a')                  |
|     for     |                          列表推导式                          |       list2 = [nums ** 2 for nums in list1]       |
| for...if... |                          列表推导式                          | list2 = [nums ** 2 for nums in list1 if nums > 2] |

#### 列表推导式

**在for循环后面可以再嵌套for循环**

![image-20231019194218165](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019194218165.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 5、元组（tuple）

> 本段转载于[元组(Tuple) | 不可改变的 Python 数据类型 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/193072837)
>
> [Python教程(10)——Python变量类型元组tuple的详细用法-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/2319734)
>
> [【译】全面深入介绍Python中的元组 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/106170499)
>
> [【说站】python元组如何打包和解包-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/2172901)
>
> [Python 元组的装包与拆包 (runoob.com)](https://www.runoob.com/note/65812)

**容器类型**

序列的一种，有序且不可变序列，==因此继承了序列的所有功能==

元组中的元素不允许被修改，因此元组也被称作**只读列表**。

元组使用小括号 `()` 包裹，元素间使用逗号 `，` 分隔，元组中的元素可以是字符串、数字、列表、元组等其他数据类型。

元组不支持修改，但支持索引、拼接、成员检查、重复等相关操作

元组的不可变性意味着无法向元组中添加、删除或修改元素。这种特性使得**元组适合用于存储一组常量值**，或**作为函数的返回值，以防止意外的修改**。

元组在Python中作为一种不可变的有序数据类型，用于存储不希望被修改的数据。它们能够提供数据保护、函数返回多个值、元组拆包等功能，使代码更加可靠、高效和安全。

### （1）创建元组

- 使用 **tuple(iterable)** 函数创建元组

```python
t = tuple("hello")
print(t)
```

- 直接使用圆括号创建元组，这也是比较常用的一种方式:**(元素1，元素2，元素3，...)**

```python
t = (1,2,3)
print(t)
```

- 使用逗号创建元组

**任何无符号的对象，以逗号分割，默认被视为元组**

```python
t = 1,2,3
print(t)
```

- 元组可以嵌套定义

使用 **二维数组** 的方式可以访问到嵌套元组

```python
t = ("hello", ("张三", "李四"))
print(t)

print(t[0])

print(t[1][0])
```

```xml
('hello', ('张三', '李四'))
hello
张三
```

**需要注意的是**，如果元组只包含一个元素，需要在元素后面**加上一个逗号**，以区分元组和表达式中的括号。

```python
t = 1,
print(t)
```

```python
t = (1,)
print(t)
```

创建元组后，可以使用索引来访问元组的元素，也可以使用拆包操作将元组的值分配给多个变量。

**打包**：创建元素，并将多个数据放到元组中；

Python自动完成打包操作

```python
t = 1,2,3,4
print(t)
```

**拆包(解包)**：将元组中的元素去出，分别赋值给不同的变量;

Python自动完成打包操作

解包时，如果解包出来的元素数目与变量数目不匹配，就会引发ValueError异常。

错误信息为：too many values to unpack（解包的值太多）或not enough values to unpack（解包的值不足）。

```python
a,b,c = 1,2,3
print(a)
print(b)
print(c)
```

![image-20231020003524396](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020003524396.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

创建后的元组是不可变的，即元组的元素无法被修改、删除或添加。

如果需要修改元组中的元素，可以**先将元组转换为列表**，进行相应的操作，然后**再将列表转换回元组**。

### （2）访问元组中的元素

**类似列表**

使用负索引访问元素：可以使用负索引来从元组的**末尾开始访问**元素。

```python
t = (1,2,3,4,5)
print(t[2])
print(t[1:4])
print(t[0:4:2])
```

```xml
3
(2, 3, 4)
(1, 3)
```

### （3）更改元组中的元素

元组是不可变的（immutable），这意味着无法直接修改元组中的元素。如果需要更改元组中的元素，可以通过以下方法实现：

- 创建一个新的元组，包含需要更改的元素以及其他不需要更改的元素。

```python
t = (1, 2, 3)
new_t = (4,) + t[1:]  # 创建一个新的元组，将第一个元素更改为 4
print(new_t)  # 输出 (4, 2, 3)
```

- 将元组转换为列表，对列表进行修改后再转换回元组。

```python
t = (1, 2, 3)
l = list(t)  # 将元组转换为列表
l[0] = 4  # 修改列表中的元素
t = tuple(l)  # 将列表转换回元组
print(t)  # 输出 (4, 2, 3)
```

**需要注意的是**，无论哪种方法，都会创建一个新的元组或列表来储修改后的结果，而不会直接修改原始的元组对象。

因为元组是不可变的数据类型，在创建后无法修改其内部的元素。

总结起来，要更改一个元组的值，需要创建一个新的元组并将修改后的值添加进去，

或者将元组转换为列表进行修改后再转换回元组，

因此**如果需要频繁地对元素进行修改，建议使用列表代替元组**。

==拓展==：

**元素不允许被修改**，但其元素的元素为可变类型时则支持修改

```python
t = ("hello", ["张三", "李四"])
print(t)

t[1][0]="王五"

print(t[1])
```

```xml
('hello', ['张三', '李四'])
['王五', '李四']
```

### （4）删除元组或元组中的元素

由于元组是不可变的数据结构，所以**无法直接删除元组的元素**。不过可以通过以下几种方式来实现元组的删除操作：

- 使用del关键字删除整个元组：

```python
t = (1, 2, 3)
del t
print(t)  # 报错：NameError: name 't' is not defined
```

后再尝试访问元组会引发NameError，因为**元组已经被删除**。

- 创建一个新的元组，不包含需要删除的元素：

```python
my_tuple = (1, 2, 3)
new_tuple = tuple(element for element in my_tuple if element != 1)  # 创建新的元组，跳过需要删除的素
print(new_tuple)  # 输出: (2, 3)
```

- 将元组转换为列表进行删除后再转换回元组：

```python
my_tuple = (1, 2, 3)
my_list = list(my_tuple)  # 将元组转换为列表
my_list.remove(1)  # 从列表中删除需要删除的元素
new_tuple = tuple(my_list)  # 将列表转换回元组
print(new_tuple)  # 输出: (2, 3)
```

转换为列表后可以使用`remove()`方法删除元素。

需要注意的是，以上方法都会创建新的元组或列表，因为元组是不可变的数据结构，无法直接修改原始的元组对象。

因此，删除操作实际上是创建一个新的元组，不包含需要删除的元素。

### （5）元组元素排序

![image-20231020002330732](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020002330732.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （6）枚举

![image-20231020003012159](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020003012159.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```xml
0 Steve
1 Rachel
2 Michael
3 Monica
```

### （7）元组相对于列表的优点

列表和元组是按序列存储值的内置Python数据类型。元组是不可变的，而列表是可变的。与列表相比，元组还有其他一些优点（部分来自堆栈溢出）

- 元组比列表快。如果要定义一个恒定的数值集合，并且你所要做的只是遍历它，请使用元组而不是列表。使用`timeit`可以测量性能差异，该模块允许你对Python代码计时。下面的代码为每种方法执行100万次，并输出以秒为单位的总时间。

```python
import timeit 
print(timeit.timeit('x=(1,2,3,4,5,6,7,8,9,10,11,12)', number=1000000))

print(timeit.timeit('x=[1,2,3,4,5,6,7,8,9,10,11,12]', number=1000000))
```

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/v2-cb34c4bfdbc85e41c8b4f01d18cde69e_1440w.webp?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- **元组可以用作字典键**（特别是包含不可变值的元组，如字符串、数字和其他元组）。列表永远不能用作字典键，因为列表是可变的。

![image-20231020002708246](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020002708246.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 元组可以用作集合中的值，而列表不能。

## 6、集合（set）

> 本段转载于[Python 集合是什么，为什么应该使用以及如何使用？ - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/40854901)
>
> [【python】集合set详解（超详细）_python的set函数_devil_son1234的博客-CSDN博客](https://blog.csdn.net/devil_son1234/article/details/128930682)
>
> [一文带你了解Python集合与基本的集合运算 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/38442300)

**容器类型**

**可迭代、无序、不能包括重复元素**

序列中的元素是有序的，集合中的元素是无序的。

集合是一个*无序*集合，没有*重复元素*。

基本用途包括*==成员测试==*和*==消除重复的条目==*。

集合对象还支持数学运算，如*并集*、*交集*、*差集*和*对等差分*。

每次打印**返回的顺序并不和初始的一致**

### （1）创建集合

- set(iterable)内置函数

```python
s = set("hello")
print(s)
```

```xml
{'e', 'l', 'o', 'h'}
```

在使用`set()函数`创建集合时，一定要注意**双括号**

```python
my_set = set(("water","animal")) #等价于 my_set = {"water", "animal"}

print(my_set)
```

- {元素1，元素2，元素3，...}

```python
s = {1,2,3,4,3,2}
print(s)
```

```xml
{1, 2, 3, 4}
```

- 空 { } 可以得到一个空集合吗？

```python
s = {}
print(type(s))
```

```xml
<class 'dict'>
```

**得到的是一个字典**

如何得到一个空集

```python
my_set = set()
print(my_set)
```

==拓展==：

集合可以包含 Python 支持的所有 ***[可哈希的](https://link.zhihu.com/?target=https%3A//docs.python.org/3/glossary.html%23term-hashable)(hashable)* 数据类型**。

换句话说，即**整数**、**字符串**和**元组**，而不是*列表*或*字典*这样的可变类型。

否则，会报

```xml
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unhashable type: 'list'
```

![image-20231020090435069](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020090435069.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （2）添加集合元素

- add(elem) 添加单个元素

- update(iterable)  添加多个元素

```python
my_set = {1,2,3}

my_set.add(4)
print(my_set)

my_set.update([3,5,6])
print(my_set)
```

```xml
{1, 2, 3, 4}
{1, 2, 3, 4, 5, 6}
```

### （3）修改集合和集合中的元素

- remove(elem)

删除集合中的对应元素，若元素不存在，则抛出错误

- discard(elem)

删除集合中的对应元素，若元素不存在，不会报错

- pop()

随机弹出一个元素,需要注意的是，如果集合是空的，该方法会返回一个「KeyError」。

- clear()

清空集合中的所有元素

- del

删除集合

### （4）交并补或运算

#### union()

`union()` 或者 `|` 将创建一个新集合，其中包含我们提供集合中的所有元素：

```python
>>> s1 = {1, 2, 3}
>>> s2 = {3, 4, 5}
>>> s1.union(s2)  # 或者 's1 | s2'
{1, 2, 3, 4, 5}
```

#### intersection()

`intersection` 或 `&` 将返回一个由集合共同元素组成的集合：

```python
>>> s1 = {1, 2, 3}
>>> s2 = {2, 3, 4}
>>> s3 = {3, 4, 5}
>>> s1.intersection(s2, s3)  # 或者 's1 & s2 & s3'
{3}
```

#### difference()

使用 `diference()` 或 `-` 创建一个新集合，其值在 “s1” 中但不在 “s2” 中：

```python
>>> s1 = {1, 2, 3}
>>> s2 = {2, 3, 4}
>>> s1.difference(s2)  # 或者 's1 - s2'
{1}
```

#### symmetric_diference()

`symetric_difference` 或 `^` 将返回集合之间的不同元素。

```python
>>> s1 = {1, 2, 3}
>>> s2 = {2, 3, 4}
>>> s1.symmetric_difference(s2)  # 或者 's1 ^ s2'
{1, 4}
```

### （5）父集合与子集合

![image-20231020094701216](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020094701216.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- issubset() 方法用于判断集合的所有元素是否都包含在指定集合中，如果是则返回 True，否则返回 False;
- issuperset() 方法用于判断指定集合的所有元素是否都包含在原始的集合中，如果是则返回 True，否则返回 False。

```python
fu_set = {1, 2, 3, 4, 5}
zi_set = {2, 3, 4}
print(zi_set.issubset(fu_set))
print(fu_set.issuperset(zi_set))
```

```xml
True
True
```

### （6）集合特性总结

- 集合中的元素是无序的

所以无法使用 **索引** 和 **切片** 的方式来操作集合中的元素

- 集合中的元素不可以重复

可以用来删除某一堆元素中的重复元素

==拓展==：**三种方式实现检查并删除列表中的重复元素**

方法一：使用 for 和 if 成员检测

```python
my_list = [1,1,3,9,3,7,6,0,8,1]

new_list=[]

for i in my_list:
    if i not in new_list:
        new_list.append(i)

print(new_list)
```

```xml
[1, 3, 9, 7, 6, 0, 8]
```

方法二：列表推导式

```python
my_list = [1,1,3,9,3,7,6,0,8,1]

new_list=[]

[new_list.append(i) for i in my_list if i not in new_list]

print(new_list)
```

```xml
[1, 3, 9, 7, 6, 0, 8]
```

方法三：**先转集合，在转列表**

```python
my_list = [1,1,3,9,3,7,6,0,8,1]

new_list = list(set(my_list))

print(new_list)
```

```xml
[0, 1, 3, 6, 7, 8, 9]
```

**注意**：请记住集合是无序的，因此**无法保证**在将它们转换回列表时，元素的顺序不变。

- 集合成员检测的效率要高于列表

![image-20231020095347635](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020095347635.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 7、字典

> 本段转载于[Python精讲：python中字典的概念、特征、创建和删除详解 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/433698841)
>
> [Python字典及基本操作（超级详细） (biancheng.net)](https://c.biancheng.net/view/2212.html)
>
> [Python 字典用法详解（超全） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/355443925)
>
> [Python3 zip() 函数详细使用方式 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/354924536)

**容器类型**

字典（dictionary）是**无序的**、**可变的**、保存的内容是以“**键-值对**”的形式存储的序列。

字典由 **键视图** 和 **值视图** 。

键视图不能包含重复的元素

值视图能够包含重复的元素

应牢记字典包含多个 key-value 对，而 key 是字典的关键数据，因此程序对字典的操作都是基于 key 的。

![image-20231020230357746](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231020230357746.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （1）字典的特性

- 通过键而不是通过索引来读取

字典有时也称为**关联数组**或者**散列表**（hash）。

它是通过键将一系列的值联系起来的，这样就可以通过键从字典中获取指定项，但**不能通过索引**来获取。

- 字典是任意对象的无序集合

字典是无序的，各项是从左到右随机排序的，即保存在字典中的项没有特定的顺序。这样可以提高查找顺序。

- 字典是可变的，并且可以任意嵌套

字典可以在原处增长或者缩短（**无须生成一份拷贝**），并且它支持任意深度的嵌套（即它的值可以是列表或者其他的字典）。

- 字典中的键必须唯一

不允许同一个键出现两次，如果出现两次，则后一个值会被记住。

- 字典中的键必须不可变

字典中的键是不可变的，所以可以使用数字、字符串或者元组，但不能使用列表。

- 字典的 key 是它的关键。

换个角度来看，字典的 key 就相当于它的索引，只不过这些索引不一定是整数类型，字典的 key 可以是任意不可变类型。

  可以这样说，**字典相当于索引是任意不可变类型的列表**：而列表则相当于 key 只能是整数的字典。因此，如果程序中要使用的字典的 key 都是整数类型，则可考虑能否换成列表。

- 字典的key 索引

  此外，还有一点需要指出，列表的索引总是从 0 开始、连续增大的；但字典的索引即使是整数类型，**也不需要从 0 开始**，而且**不需要连续**。因此，列表不允许对不存在的索引赋值：但字典则允许直接对不存在的 key 赋值，这样就会为字典增加一个 key-value 对。

### （2）创建字典

- dict(参数)字典

参数可以是：字典、元组、列表、用zip()函数打包成的元组。

```python
a = dict(A = 1, B = 2, C =3)
print(a)

b = dict({'A': 1, 'B': 2, 'C': 3})
print(b)
```

```xml
{'A': 1, 'B': 2, 'C': 3}
{'A': 1, 'B': 2, 'C': 3}
```

**zip()** 函数用于将可迭代的对象作为参数，将对象中对应的元素打包成一个个元组，然后返回由这些元组组成的列表。

用于将多个列表或元组**对应位置的元素组合为元组**，并返回包含这些内容的zip对象。

如果各个迭代器的元素个数不一致，则返回列表长度与最短的对象相同，利用 * 号操作符，可以将元组解压为列表。

这样做的好处是**节约了不少的内存**

```python
d = dict(zip([0, 1, 2], ["张三", "李四", "王五"]))

print(d)
```

```xml
{0: '张三', 1: '李四', 2: '王五'}
```

- {key1:value1,key2:value2,...,keyn:valuen}

key1, key2, ..., keyn：表示元素的键，必须是**唯一的**，并且**不可变**，例如可以是字符串、数字或者元组；

value1, value2, ..., valuen：表示元素的值，可以是**任何数据类型**，**不是必须唯一**。

- 通过二元组列表

```python
list = [('A', 1), ('B', 2), ('C', 3)]
a = dict(list)
print(a)
```

- 通过dict对象的fromkeys()方法创建字典

创建带有默认值的字典

**dictionary =  dict.fromkeys(list，value=None)**

其中，list 参数表示字典中所有键的列表（list）；

value 参数表示默认值，如果不写，则为空值 None。

```python
course = ['语文','数学','英语']
d = dict.fromkeys(course,100)
print(d)
```

```xml
{'语文': 100, '数学': 100, '英语': 100}
```

- 通过字典推导式创建

```python
d = {i : i*2 for i in range(3)}
print(d)
```

```xml
{0: 0, 1: 2, 2: 4}
```

### （3）添加或替换

- 字典中不存在这个key键

```python
d = {"张三": 18, "李四": 20, "王五": 19}
d["赵六"] = 20
print(d)
```

```xml
{'张三': 18, '李四': 20, '王五': 19, '赵六': 20}
```

- 字典中存在这个key值

```python
d = {"张三": 18, "李四": 20, "王五": 19}
d["张三"] = 20
print(d)
```

```xml
{'张三': 20, '李四': 20, '王五': 19}
```

### （4）删除

- 删除整个字典

不再需要的字典也可以使用 **del** 命令删除，del 删除整个字典

- 删除字典中全部元素

删除字典的全部元素，可以使用字典对象的 **clear()** 方法，执行clear()方法后，原字典将变为空字典。

- 删除字典中指定键的元素

使用字典对象的 **pop()** 删除并返回指定“键”的元素

**del(key)**：可以删除指定键的键值对

- 删除并返回字典中的一个元素

使用字典对象的popitem()方法删除并返回字典中的一个元素

```python
d = {i : i*2 for i in range(3)}
print(d)
dd = d.popitem()
print(d)
print(dd)
```

```xml
{0: 0, 1: 2, 2: 4}
{0: 0, 1: 2}
(2, 4)
{0: 0}
```

### （5）访问

通过**键值**来访问

```python
d = {"张三":18,"李四":20,"王五":19}
print(d["张三"])
```

### （6）成员检测

如果要判断字典是否包含指定的 key，则可以使用 **in 或 not in** 运算符。

需要指出的是，对于 dict 而言，in 或 not in 运算符都是**基于 key** 来判断的。

```python
d = {"张三": 18, "李四": 20, "王五": 19}

print("张三" in d)
print("赵六" not in d)
```

```xml
True
True
```

### （7）字典中的方法

使用 **dir(dictory)** 查看

```python
d = {"张三": 18, "李四": 20, "王五": 19}
j=0
for i in range(0, len(dir(d))):
    if dir(d)[i] >= 'a':
        j+=1
        print("%d、%-11s\t" %(j,dir(d)[i]), end="")
        if (i-1) % 3 == 0:
            print()
```

```xml
1、clear      	2、copy       	3、fromkeys   	
4、get        	5、items      	6、keys       	
7、pop        	8、popitem    	9、setdefault 	
10、update     	11、values  
```

#### clear()方法

clear() 用于**清空字典中所有的 key-value 对**，对一个字典执行 clear() 方法之后，该字典就会变成**一个空字典**。例如如下代码：

```python
cars = {'BMW': 8.5, 'BENS': 8.3, 'AUDI': 7.9}
print(cars) # {'BMW': 8.5, 'BENS': 8.3, 'AUDI': 7.9}
# 清空cars所有key-value对
cars.clear()
print(cars) # {}
```

#### copy()方法

![image-20231021102015245](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231021102015245.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

#### get()方法

get() 方法其实就是**根据 key 来获取 value**，它相当于方括号语法的增强版，**当使用方括号语法访问并不存在的 key 时，字典会引发 KeyError 错误**；但如果**使用 get() 方法访问不存在的 key，该方法会简单地返回 None，不会导致错误**。例如如下代码：

```python
cars = {'BMW': 8.5, 'BENS': 8.3, 'AUDI': 7.9}# 获取'BMW'对应的value
print(cars.get('BMW')) # 8.5
print(cars.get('PORSCHE')) # None
print(cars['PORSCHE']) # KeyError
```

#### update()方法

update() 方法可使用一个字典所包含的 key-value 对来**更新己有的字典**。在执行 update() 方法时，如果被更新的字典中己包含对应的 key-value 对，那么**原 value 会被覆盖**；如果被更新的字典中不包含对应的 key-value 对，则该 key-value 对被添加进去。例如如下代码：

```python
cars = {'BMW': 8.5, 'BENS': 8.3, 'AUDI': 7.9}
cars.update({'BMW':4.5, 'PORSCHE': 9.3})
print(cars)
```

从上面的执行过程可以看出，由于被更新的 dict 中己包含 key 为“AUDI”的 key-value 对，因此更新时该 key-value 对的 value 将被改写；但如果被更新的 dict 中不包含 key 为“PORSCHE”的 key-value 对，那么更新时就会为原字典**增加一**个 key-value 对。

#### items()、keys()、values()

items()、keys()、values() 分别用于获取字典中的**所有 key-value 对**、**所有 key**（字典键视图）、**所有 value**（字典值视图）。

这三个方法依次返回 dict_items、dict_keys 和 dict_values 对象，**Python 不希望用户直接操作这几个方法**，但可通过 list() 函数把它们转换成列表。

如下代码示范了这三个方法的用法：

```python
cars = {'BMW': 8.5, 'BENS': 8.3, 'AUDI': 7.9}# 获取字典所有的key-value对，返回一个dict_items对象
ims = cars.items()
print(type(ims)) # <class 'dict_items'>
# 将dict_items转换成列表
print(list(ims)) # [('BMW', 8.5), ('BENS', 8.3), ('AUDI', 7.9)]
# 访问第2个key-value对
print(list(ims)[1]) # ('BENS', 8.3)
# 获取字典所有的key，返回一个dict_keys对象
kys = cars.keys()print(type(kys)) # <class 'dict_keys'>
# 将dict_keys转换成列表
print(list(kys)) # ['BMW', 'BENS', 'AUDI']
# 访问第2个key
print(list(kys)[1]) # 'BENS'# 获取字典所有的value，返回一个dict_values对象
vals = cars.values()# 将dict_values转换成列表
print(type(vals)) # [8.5, 8.3, 7.9]
# 访问第2个value
print(list(vals)[1]) # 8.3
```

从上面代码可以看出，程序调用字典的 items()、keys()、values() 方法之后，都需要调用 list() 函数将它们转换为列表，这样即可把这三个方法的返回值转换为列表。

在 Python 2.x 中，items()、keys()、values() 方法的返回值本来就是列表，完全可以不用 list() 函数进行处理。当然，使用 list() 函数处理也行，列表被处理之后依然是列表。

#### pop方法

pop() 方法用于**获取指定 key 对应的 value，并删除这个 key-value 对**。如下方法示范了 pop() 方法的用法：

```python
cars = {'BMW': 8.5, 'BENS': 8.3, 'AUDI': 7.9}
print(cars.pop('AUDI')) # 7.9
print(cars) # {'BMW': 8.5, 'BENS': 8.3}
```

此程序中，第 2 行代码将会获取“AUDI”对应的 value，并删除该 key-value 对。

#### popitem()方法

popitem() 方法用于**随机弹出字典中的一个 key-value 对**。

此处的**随机其实是假的**，正如列表的 pop() 方法总是弹出列表中**最后一个元素**，实际上字典的 popitem() 其实也是**弹出字典中最后一个 key-value 对**。由于字典存储 key-value 对的顺序是不可知的，因此开发者感觉字典的 popitem() 方法是“随机”弹出的，但实际上字典的 popitem() 方法总是弹出**底层存储的最后一个 key-value 对**。

如下代码示范了 popitem() 方法的用法：

```python
cars = {'AUDI': 7.9, 'BENS': 8.3, 'BMW': 8.5}
print(cars)# 弹出字典底层存储的最后一个key-value对
print(cars.popitem()) # ('AUDI', 7.9)
print(cars) # {'BMW': 8.5, 'BENS': 8.3}
```

由于实际上 **popitem 弹出的就是一个元组**，因此程序完全可以通过**序列解包**的方式用两个变量分别接收 key 和 value。例如如下代码：

```python
# 将弹出项的key赋值给k、value赋值给vk,
v = cars.popitem()
print(k, v) # BENS 8.3
```

#### setdefault()方法

setdefault() 方法也用于**根据 key 来获取对应 value 的值**。但该方法有一个额外的功能，即==当程序要获取的 key 在字典中不存在时，该方法会先为这个不存在的 key 设置一个默认的 value，然后再返回该 key 对应的 value==。

总之，setdefault() 方法总能返回指定 key 对应的 value；如果该 key-value 对存在，则直接返回该 key 对应的 value；如果该 key-value 对不存在，则先为该 key 设置默认的 value，然后再返回该 key 对应的 value。

如下代码示范了 setdefault() 方法的用法：

```python
cars = {'BMW': 8.5, 'BENS': 8.3, 'AUDI': 7.9}
# 设置默认值，该key在dict中不存在，新增key-value对
print(cars.setdefault('PORSCHE', 9.2)) # 9.2
print(cars)
# 设置默认值，该key在dict中存在，不会修改dict内容
print(cars.setdefault('BMW', 3.4)) # 8.5
print(cars)
```

#### fromkeys()方法

fromkeys() 方法**使用给定的多个 key 创建字典**，这些 key 对应的 value 默认都是 None；也可以额外传入一个参数作为默认的 value。该方法一般不会使用字典对象调用（没什么意义），通常会使用 dict 类直接调用。例如如下代码：

```python
# 使用列表创建包含2个key的字典
a_dict = dict.fromkeys(['a', 'b'])
print(a_dict) # {'a': None, 'b': None}
# 使用元组创建包含2个key的字典
b_dict = dict.fromkeys((13, 17))
print(b_dict) # {13: None, 17: None}
# 使用元组创建包含2个key的字典，指定默认的value
c_dict = dict.fromkeys((13, 17), 'good')
print(c_dict) # {13: 'good', 17: 'good'}
```

### （8）使用字典格式化字符串

在格式化字符串时，如果要**格式化的字符串模板中包含多个变量，后面就需要按顺序给出多个变量**，这种方式对于字符串模板中包含少量变量的情形是合适的，但如果字符串模板中包含大量变量，这种按顺序提供变量的方式则有些不合适。

可改为在字符串模板中按 key 指定变量，然后通过字典为字符串模板中的 key 设置值。

- 字符串模板中使用key,使用字典为字符串模板中的key传入值

```python
temp = '%(name)s今年%(age)d岁了'
people = {'name': '张三', 'age': 18}
print(temp % people)
```

```xml
张三今年18岁了
```

### （9）遍历字典

- 遍历键视图

```python
d ={'张三':16,'李四':15,'王五':18,'赵六':20}

for name in d.keys():
    print('名字:%s'%name)
```

```xml
名字:张三
名字:李四
名字:王五
名字:赵六
```

- 遍历值视图

```python
d ={'张三':16,'李四':15,'王五':18,'赵六':20}

for age in d.values():
    print('年龄:%s'%age)
```

```xml
年龄:16
年龄:15
年龄:18
年龄:20
```

- 同时遍历所有视图

```python
d = {'张三': 16, '李四': 15, '王五': 18, '赵六': 20}

for name, age in d.items():
    print('姓名:%s,年龄:%d' % (name, age))
```

```xml
姓名:张三,年龄:16
姓名:李四,年龄:15
姓名:王五,年龄:18
姓名:赵六,年龄:20
```

## 8、总结

> 本段转载于[【精选】【Python】推导式（列表推导式、元组推导式、字典推导式、集合推导式）详解_一个写湿的程序猿的博客-CSDN博客](https://blog.csdn.net/qq_32727095/article/details/118959610)



![python 列表，元组，字典，集合，字符串相互转换](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/v2-bcd8f96b3228355852923eb12991f46c_b.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



# 七、运算符

> 本段转载于[Python 运算符详解 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/102451172)

## 1、算术运算符

操作数是整型或浮点型

结果也是相应的整型和浮点型

### 一元运算符

+（正号）、-（负号，**取反**操作）

### 二元运算符

![image-20231018231345011](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018231345011.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 2、比较运算符

操作数是表达式

结果是布尔类型

![image-20231018232758406](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018232758406.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

比较运算符可用于任意类型的数据，但是参与比较的两种类型的数据要**相互兼容**，即能够**进行隐式转换**。

**比较字符串的大小**：即逐一比较字符Unicode编码的大小，如果两个字符串的第一个字符不能比出大小，则比较两个字符串的额第二个字符，直到比较有了结果才结束比较；

**比较列表大小**：即逐一比较其中元素的大小，如果两个列表中的第一个元素不能比出大小，则比较两个列表中的第二个元素，直到比较有了结果才结束比较。注意：**两个列表中的元素类型要兼容**。

## 3、逻辑运算符

操作数是布尔类型

结果也是布尔类型

![image-20231018234356319](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018234356319.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

Python中默认采用了 **短路设计**，and 短路与、or 短路或。

“短路”指在计算过程中只要结果确定，则==不再计算后面的表达式==，从而提高效率，有点像电路短路。

## 4、位运算符

操作数是整型

结果也是整型

**位运算是以二进位（bit）为单位进行运算的**

![image-20231018235336218](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018235336218.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 5、赋值运算符

![image-20231018235940402](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231018235940402.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

==补充一个==：

![image-20231019000034002](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019000034002.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 6、成员运算符

除了以上的一些运算符之外，Python还支持成员运算符，测试实例中包含了一系列的成员，包括字符串，列表或元组。

![image-20231019000253289](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019000253289.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

运算符描述实例

in如果在指定的序列中找到值返回True，否则返回False。x 在 y序列中 , 如果x在y序列中返回True。

not in如果在指定的序列中没有找到值返回True，否则返回False。x 不在 y序列中 , 如果x不在y序列中返回True。

```python
list = [1, 2, 3, 4, 5]
while 1:
    a = int(input("请输入一个整数:"))
    if a in list:
        print("%d在list中" % a)
    if a not in list:
        print("%d不在list中" % a)
```

```xml
请输入一个整数:2
2在list中
请输入一个整数:5
5在list中
请输入一个整数:7
7不在list中
```

## 7、身份运算符

身份运算符用于比较两个对象的存储单元

![image-20231019000839840](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019000839840.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

运算符描述实例

is是判断两个标识符是不是引用自一个对象x is y, 如果 id(x) 等于 id(y) ,**is**返回结果 1

is not是判断两个标识符是不是引用自不同对象x is not y, 如果 id(x) 不等于 id(y).**is not**返回结果 1

## 8、运算符的优先级

**算术运算符 > 位运算符 > 关系运算符 > 逻辑运算符 > 赋值运算符 **

==补充==：括号（）优先级最高

![image-20231019001251586](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231019001251586.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

# 八、程序流程控制

> 本段转载于[Python基础（循环及流程控制）_python 1:100-CSDN博客](https://blog.csdn.net/qq_36068496/article/details/123021959)
>
> [超干货！Python流程控制 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/303178905)
>
> [Python中break/continue/pass的区别 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/398281537)

## 1、顺序执行语句

Python代码在执行过程中，遵循下面的**基本原则**：

普通语句，直接执行；

碰到函数，将函数体载入内存，并不直接执行

碰到类，执行类内部的普通语句，但是类的方法只载入，不执行

碰到if、for等控制语句，按相应控制流程执行

碰到@，break，continue等，按规定语法执行

碰到函数、方法调用等，转而执行函数内部代码，执行完毕继续执行原有顺序代码

## 2、分支语句（条件语句）

**Python中没有switch语句**

允许嵌套使用

```python
score = int(input("请输入你的成绩:"))
if score < 60:
    print("你的成绩不及格")
else:
    if score < 70:
        print("你的成绩及格")
    elif score > 90:
        print("你的成绩优秀")
    else:
        print("你的成绩优秀")
```

## 3、循环语句

### while

允许**嵌套使用**

else子语句在循环体正常结束时执行

其中，**else子语句**在遇到 **break**、**return**和 **有异常发生**时会出现中断，不执行。

```python
i = 0
while i < 3:
    i += 1
    print(i)
else:
    print("结束")
```

### for

允许**嵌套使用**

**可以遍历任意可迭代对象中的元素**

可迭代对象包括：字符串、列表、元组、集合、字典。

else子语句在循环体正常结束时执行

其中，**else子语句**在遇到 **break**、**return**和 **有异常发生**时会出现中断，不执行。

```python
for s in 'hello':
    print(s)
else:
    print("结束")
```

*如果在循环提中不需要使用到自定义的变量，可将自定义变量写为“_”*

```python
for _ in range(6):
    print("人生苦短，我用Python")
```

```python
人生苦短，我用Python
人生苦短，我用Python
人生苦短，我用Python
人生苦短，我用Python
人生苦短，我用Python
人生苦短，我用Python
```

#### ==拓展==

##### range的使用：

range类型的优点：不管range对象表示的整数序列有多长，所有range对象占用的内存空间都是相同的，因为仅仅需要存储start,stop和step，只有当用到range对象时，才会去计算序列中的相关元素。返回值是一个迭代器对象。

==range( start , stop , step )==

- 一个参数

```python
for i in range(10):
    print("%d "%i,end="")
```

```python
0 1 2 3 4 5 6 7 8 9 
```

- 两个参数

```python
for i in range(2,10):
    print("%d "%i,end="")
```

```python
2 3 4 5 6 7 8 9 
```

- 三个参数

```python
for i in range(2,10,2):
    print("%d "%i,end="")
```

```python
2 4 6 8 
```

## 4、跳转语句

**跳转语句能够改变程序的执行顺序**

### （1）break语句

break只能用于**循环体内**。

其效果是**直接结束并退出当前循环**，剩下的未循环的工作全部被忽略和取消。

 Python的break**只能退出一层循环**，对于多层嵌套循环，不能全部退出。

```python
for i in range(6):
    if i == 3:
        break
    print(i)
```

```python
0
1
2
```

### （2）continue语句

continue语句用于**跳过当前循环的剩余部分代码**，直接开始下一轮循环。

它**不会退出和终止循环**，只是提前结束当前轮次的循环。

同样的，continue语句只能**用在循环内**。

```python
for i in range(6):
    if i == 3:
        continue
    print(i)
```

```python
0
1
2
4
5
```

### （3）return语句（==候补==）

用于**函数**中

### （4）pass语句

pass语句在循环、函数、类和if语句中用作占位符，不做任何事情，是一个空操作。

使用场景：

假设你有一个函数或者一个空的类。您计划在将来编写代码。如果Python解释器遇到一个空的对象，它将抛出一个错误。pass语句可以在函数体或类体内部使用。在执行过程中，当解释器遇到pass语句时，会忽略并继续执行，而不会给出任何错误。

```python
for i in range(6):
    if i == 3:
        pass
    print(i,end="")
```

```xml
012345
```

## 5、案例1：计算水仙花数

水仙花数时一个三位数，且各位的立方之和等于这个数本身。

```python
for i in range(100, 1000):
    bai = i // 100
    shi = (i - bai * 100) // 10
    ge = i - bai * 100 - shi * 10
    if i == bai ** 3 + shi ** 3 + ge ** 3:
        print(i)
```

```xml
153
370
371
407
```

## 6、案例2：打印九九乘法表

```python
for j in range(1, 10):
    for i in range(1, 10):
        if j >= i:
            print("%d * %d = %d\t" % (i, j, i * j),end="")
    print()
```

```xml
1 * 1 = 1	
1 * 2 = 2	2 * 2 = 4	
1 * 3 = 3	2 * 3 = 6	3 * 3 = 9	
1 * 4 = 4	2 * 4 = 8	3 * 4 = 12	4 * 4 = 16	
1 * 5 = 5	2 * 5 = 10	3 * 5 = 15	4 * 5 = 20	5 * 5 = 25	
1 * 6 = 6	2 * 6 = 12	3 * 6 = 18	4 * 6 = 24	5 * 6 = 30	6 * 6 = 36	
1 * 7 = 7	2 * 7 = 14	3 * 7 = 21	4 * 7 = 28	5 * 7 = 35	6 * 7 = 42	7 * 7 = 49	
1 * 8 = 8	2 * 8 = 16	3 * 8 = 24	4 * 8 = 32	5 * 8 = 40	6 * 8 = 48	7 * 8 = 56	8 * 8 = 64	
1 * 9 = 9	2 * 9 = 18	3 * 9 = 27	4 * 9 = 36	5 * 9 = 45	6 * 9 = 54	7 * 9 = 63	8 * 9 = 72	9*9=81
```

# 九、函数

> 本段转载于[Python入门：什么是函数 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/271840916)
>
> [Python 中函数（function）的用法_func函数-CSDN博客](https://blog.csdn.net/qdPython/article/details/106285841)

函数是组织好的，可重复使用的，用来实现单一，或相关联功能的代码段。

函数能提高**应用的模块性**，和代码的**重复利用率**。

Python提供了许多内建函数，比如print()、input()，也可以自己创建函数，这被叫做**用户自定义**函数。

## 1、函数分类

- 普通函数

在模块中且类之外定义，作用域是当前模块

- 嵌套函数

在别的函数中定义

- 方法

在类中定义

## 2、函数的定义

**def 函数名 (形参列表)：**

​	**函数体**

​	**[ return 返回值 ]**



- 不带表达式的return相当于返回 None

## 3、函数的调用

定义一个函数只给了函数一个名称，指定了函数里包含的参数，和代码块结构。

这个函数的基本结构完成以后，可以通过另一个函数调用执行，也可以直接从Python提示符执行。

在调用函数时传递的实参与定义函数时的形参顺序一致。

==传递参数==

```python
def area(width,height):
    return width*height

area(300,200)
area(width=300,height=200)
area(height=200,width=300)
```

**三种方式等价**

## 4、参数的默认值

**了解**：函数的重载

可以定义多个同名函数，但是参数列表 不同，这样在调用时可以传递不同的实参。

Python中没有函数重载的概念，原因：**函数重载会增加代码量**。

==在定义函数时，自己可以在参数列表中自定义一个参数的值==

如果函数调用时没有传入参数，则使用自定义那个默认的参数

如果自定义的函数**不需要参数**或者**有默认参数**也可以**不填括号中的内容**

如果传入了参数，自定义的默认参数就会失效，而使用提供的参数。

```python
def find_something(name="身份证"):
    return '{0}找到了'.format(name)

s1 = find_something()
print(s1)
s2 = find_something("书包")
print(s2)
```

```xml
身份证找到了
书包找到了
```

## 5、可变参数

**用于接收不确定数量的参数**

- 基于元组的可变参数（*可变参数）

**多个参数被组装**

```python
sum(*nums):
    total=0
    for num in nums:
        total+=num
    return total

print(sum(3,5,2,7,2))
```

```xml
19
```

- 基于字典的可变参数（**可变参数）

```python
def show_info(**info):
    print('------show info------')
    for key, value in info.items():
        print('{0}--{1}'.format(key, value))


show_info(name='张三', age=18, set='男')
show_info(stu_name='李四', stu_no='1000001')
```

```xml
------show info------
name--张三
age--18
set--男
------show info------
stu_name--李四
stu_no--1000001
```

## 6、函数中变量的作用域

> 本文转载于[一文读懂Python变量作用域 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/622596840)
>
> [【精选】【Python】Python中令人头疼的变量作用域问题，终于弄清楚了_风度78的博客-CSDN博客](https://blog.csdn.net/fengdu78/article/details/116617923)
>
> [零基础学Python：作用域详解_python作用域_Python热爱者的博客-CSDN博客](https://blog.csdn.net/qdPython/article/details/119805255)

在 Python 程序中,变量的作用域主要由其定义位置决定。

Python中的变量名可以指代变量、函数、类、对象等。一般来说，每个对象都有一个变量名**指向**，更准确说是 **绑定**。

变量可以有全局作用域和局部作用域两种。

**全局变量**:定义在函数外部的变量拥有全局作用域,可以在整个文件内使用。

全局变量的作用域跨越函数边界,所有函数都可以访问全局变量。

若在函数内修改全局变量,需要使用 global 关键字进行声明,否则会在函数内创建一个局部变量:

**局部变量**:定义在函数内部的变量拥有局部作用域,只能在函数内部使用。局部变量的作用域只在函数内,外部函数无法访问局部变量

#### 作用域的必要性

为啥变量要有作用域呢？

我们在Python里遇到的内置、局部、全局及自由变量，就是说变量的作用域。

语言区分作用域，是**为了复用变量名**。引入作用域，相当于给变量**划分了各自的“隔离区”**，在不同”隔离区“里，查找变量变得很容易。

正是因为有了作用域，我们在函数内才可以随意使用变量名，而不担心其与全局变量、其他函数中的变量冲突——因为这两个作用域是分割的。

==拓展==

BASIC语言只有全局变量，你能想象吗？你在一个函数里命名的循环变量`i`，很可能跟全局变量冲突。写起程序来，举步维艰。且会导致很多修改、检索问题，维护很困难。

#### Python变量定义的时间和空间

Python 有哪些作用域呢？

**Python是动态类型语言，变量是在定义的时候赋值的。**这句话的意思我们分以下几个方面来理解：

- a = 1 赋值时定义变量
- from tools import cubie 导入时定义变量 cubie
- def fun():pass 定义函数，绑定变量fun
- def fun(name=None):pass 定义变量name为函数fun的形式变量（也是局部变量），同时定义函数，绑定便令fun
- class Car:pass 定义类，绑定类名Car

以上，我们弄清了变量定义的时刻，下面来看变量的作用域，也就是变量的活动空间怎么规定出来的。

变量作用域取决于其 **定义位置**。

- 定义在函数内部的变量、定义在函数声明中的形式参数，视为局部变量。
- 定义在 .py 文件内的，且函数、类之外的变量，视为全局变量。
- 定义在函数中，嵌套函数外，且被嵌套函数引用的变量，视为自由变量。
- 定义在builtin中的变量，视为内置变量。



**LEGB**规则呼之欲出：在本地空间寻找不到的变量，逐级向上级寻找。

这里的**LEGB分别指代Local，Enclose，Global和Builtin。**

![image-20231022010141104](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231022010141104.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

对于一个变量，**内部作用域先声明就会覆盖外部变量**，不声明直接使用，就会使用外部作用域的变量；

内部作用域要修改外部作用域变量的值时，全局变量要使用global关键字，嵌套作用域变量要使用
nonlocal关键字。

nonlocal是python3新增的关键字，有了这个 关键字，就能完美的实现闭包了。

```python
x =20
def xxx():
    global x
    x=10
    print("inner--{0}".format(x))

xxx()
print("outer---{0}".format(x))
```

```xml
inner--10
outer---10
```

## 7、函数类型

### （1）理解函数类型

函数的数据类型为：**function**

一个函数可以作为另一个函数的返回值使用，

也可以作为另一个函数参数使用。

有两个参数的函数和有一个参数的函数是不同的函数类型。

```python
def add(a,b):
    return a+b
def sub(a,b):
    return a-b
def cal(operation):
    if operation=='+':
        return add
    elif operation=='-':
        return sub

f1 = cal('+')
f2 = cal('-')

print(type(f1))
print('10+5={0}'.format(f1(10,5)))
print('10-5={0}'.format(f2(10,5)))
```

```xml
<class 'function'>
10+5=15
10-5=5
```

### （2）过滤函数filter( )

**filter ( function , iterable )**

- function : 过滤条件，符合条件，返回True，被保留;不符合条件，返回False，被过滤。
- iterable : 可迭代对象，会被全部遍历。

- 返回值：  不是一个列表

```python
def f(x):
    return x>5
data=[2,5,8,2,5,7,1,0]
print(filter(f,data))
print(list(filter(f,data)))
```

```xml
<filter object at 0x0000027B07F84D90>
[8, 7]
```

### （3）映射函数map( )

**map ( function , iterable )**

- funcation:提供变换规则，返回变换之后的元素。
- iterable: 可迭代对象，会被全部遍历。

```python
def f(x):
    return x*2
data=[1,2,3,4,5,6]
print(map(f,data))
print(list(map(f,data)))
```

```xml
<map object at 0x000001E8C9395090>
[2, 4, 6, 8, 10, 12]
```

## 8、lambda函数

**匿名的函数**

**lambda 参数列表 : lambda体**

- lambda体部分只能是一条语句
- 会自动计算并返回结果给lambda()函数
- 不需要return语句

```python
def cal(operation):
    if operation=='+':
        return lambda a,b:(a+b)
    elif operation=='-':
        return lambda a,b:(a-b)

f1 = cal('+')
f2 = cal('-')

print(type(f1))
print('10+5={0}'.format(f1(10,5)))
print('10-5={0}'.format(f2(10,5)))
```

```xml
<class 'function'>
10+5=15
10-5=5
```

![image-20231022094515383](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231022094515383.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

# 十、类与对象

> 本段转载于[一文入门Python面向对象编程（干货满满） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/437925568)
>
> [史上最全 Python 面向对象编程 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/61042358)
>
> [对象和类、关系、type和object的简单理解｜Python - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/159272293)
>
> [python类和对象最全详解（持续修订中）_python中什么是类?什么是对象?类中要封装哪些成员-CSDN博客](https://blog.csdn.net/q188201521/article/details/103057097)

## 1、面向对象

人类认识社会的方式更多的就是面向对象的方式。

“**物以类聚、人以群分**”，这句话好像给我们的面向对象有很好的诠释。

会飞的是鸟类，会游的是鱼类。人们总是很会捕捉生活中各种事物的特征，并进行分类。

这其实就是一种面向对象的思想。

**不同的对象总是有着不同的特征，同一类的对象总是有着相似或者相同的特征。**

有一句话叫做“一切皆对象“，这就意味着编程要进阶，面向对象是我们绕不过去的坎。

==面向过程 与 面向对象==

目的：将大象装进冰箱

- 面向过程

面向过程是一种**以事件为中心**的编程思想，编程的时候把解决问题的**步骤分析出来**，并且**按步骤实现**。

在这里面：我们的事件是把大象装进冰箱，所以我们需要把这件事情拆成各个小步骤，并且实现每个小步骤。

```python
a = "大象"
open_ice_door()  # 开冰箱门，需要自己实现开冰箱门的函数
push(a)   # 推大象进入
close_ice_door()  # 关冰箱门，需要自己实现关冰箱门的函数
```

那如果是把大象装进洗衣机呢？

```python
a = "大象"
open_washer _door()  # 开洗衣机门，需要自己实现开洗衣机门的函数
push(a)   # 推大象进入
close_washer_door()  # 关洗衣机门，需要自己实现关洗衣机门的函数
```

那如果是把大象装进铁笼呢？

```python
a = "大象"
open_hot_door()  # 开铁笼门，需要自己实现开铁笼门的函数
push(a)   # 推大象进入
close_hot_door()  # 关铁笼门，需要自己实现关铁笼门的函数
```

那我要是想，今天关冰箱、明天关洗衣机、后天关铁笼呢？我要是想关狮子、老虎呢？我要是想冰箱关大象、洗衣机关狮子、笼子关老虎呢？

我们发现，**需求会越来越复杂**，**代码量越来越多**，**重复代码也越来越多**，

而且真正复杂的场景下，我们是**没办法写出完整的面向过程的代码的**。

==这件事情本质就是：把一个动物关进一个容器里面，==

==这个容器可以开门也可以关门，开门和关门这个动作是一样的，==

==而且这个容器是可以复用的。==

- 面向对象

上面的任务中：我们需要自己创造冰箱、洗衣机、笼子，并且实现开关门方法。

于是，我们就可以把**通用的方法封装起来**

```python
class Box():
    """盒子类，实现了开门、关门方法"""

    def open_door(self):
        pass

    def close_door(self):
        pass

class IceBox(Box):
    """冰箱"""

    def ice(self):
        """制冷"""
        pass

class WaterBox(Box):
    """洗衣机"""

    def add_water(self):
        """加水"""
        pass

    def sub_water(self):
        """排水"""
        pass   

    def wash(self):
        """洗涤"""
        pass

a = "大象"
ice_box = IceBox()   # 冰箱对象
ice_box.open_door()  # 通知冰箱开门
push(a)   # 推大象进入
ice_box.close_door()  # 通知冰箱关门


# 那我想关老虎呢？
b = "老虎"
ice_box.open_door()  # 通知冰箱开门
push(b)   # 推老虎进入
ice_box.close_door()  # 通知冰箱关门
```

面向对象的思想主要是**以对象为主**，将一个问题抽象出具体的对象，并且**将抽象出来的对象和对象的属性和方法封装成一个类**。

例如上面，我们可以把冰箱、洗衣机、铁笼子抽象成一个盒子对象，这个盒子可以开门、也可以关门。

**任何脱离面向过程空谈面向对象的都是耍流氓！**

面向对象的方法，**本质上还是为面向过程服务**的，因为计算机解决问题的方法永远都是面向过程的。

面向对象只是人类的狂欢，只是为了让程序看起来更符合人的思考方式。



**面向过程编程：**

```text
1. 导入各种外部库
2. 设计各种全局变量
3. 写一个函数完成某个功能
4. 写一个函数完成某个功能
5. 写一个函数完成某个功能
6. 写一个函数完成某个功能
7. 写一个函数完成某个功能
8. ......
9. 写一个main函数作为程序入口
```

在多函数程序中，许多重要的数据被放置在全局数据区，这样它们可以被所有的函数访问。

每个函数都可以具有它们自己的局部数据，将某些功能代码封装到函数中，日后便无需重复编写，仅调用函数即可。

从代码的组织形式来看就是**根据业务逻辑从上到下垒代码** 。

**面向对象编程：**

```text
1. 导入各种外部库
2. 设计各种全局变量
3. 决定你要的类
4. 给每个类提供完整的一组操作
5. 明确地使用继承来表现不同类之间的共同点
6. 根据需要，决定是否写一个main函数作为程序入口
```

面向对象编程中，将函数和变量进一步封装成类，类才是程序的基本元素，它将数据和操作紧密地连结在一起，并保护数据不会被外界的函数意外地改变。

类和类的实例（也称对象）是面向对象的核心概念，是和面向过程编程、函数式编程的根本区别。

并不是非要用面向对象编程，要看你的程序怎么设计方便，但是就目前来说，基本上都是在使用面向对象编程。



## 2、类和对象

**类是一组相关属性和行为的集合**

**类（class）是描述具有相同属性（Arrtibute）和方法（MethoD）的对象的集合**

Python中一切皆对象（object），例如字符串、元祖、列表等都是**对象**

最常见的类是什么？人类！

人类的属性：有两个眼睛、一个鼻子、一个嘴巴、两个耳朵、一个头、两只手、两条腿

人类的行为：走、跑、跳、呼吸、吃饭

**类的实例，由类创造。**

人类是一个抽象的类。你是具体的一个人类对象。

人类是女娲娘娘画的图纸。对象是女娲娘娘根据图纸一个一个捏出来的小人。

## 3、定义一个类

*类名一般使用**大驼峰命**名*

面向对象是通过**定义class类**来定义，

这么说面向对象编程就是只使用class类，在class类中有封装，继承的功能，并且还可以构造要传入的参数，方便控制。

关键字`class`后面跟着类名，类名通常是大写字母开头的单词，紧接着是`(object)`，表示该类是从哪个类继承下来的。

通常，如果没有合适的继承类，就使用`object`类，这是所有类最终都会继承下来的类。

object类是所有类的根类，在Python中任何一个类（除object外）都直接或间接地继承了object。

```python
# 类名 Person 通常是大写字母开头的单词
# (object) 表示继承自object这个类，暂时不知道继承的可以先跳过，省略不写
class Person(object):
    pass
```

这里我们就定义了一个最基本的类。写在类中的函数，我们通常称之为（对象的）方法

==pass==

pass语句只用于维持程序结构的完整。

我们在编程时若不想马上编写某些代码，又不想有语法错误，就可以使**用pass语句占位**。

## 4、创建对象

类的实例化

person就是类的实例化对象

```python
person = Person()  # person 是 Person 类的实例对象
```

对象不再被使用时需要被销毁。

再Python中销毁对象时由**Python垃圾回收器**再后台释放对象，不需要程序员手动释放对象。



## 5、类的成员

实例变量和实例方法属于对象，通过对象调用；

类变量和类方法属于类，通过类调用。

类也遵从自下而上执行，所以如果类里面有同名的方法，**前一个方法会被后一个方法覆盖**。

然后对象初始化的时候，会调用类覆盖好的方法

- 成员变量

数据成员，保存了类或对象的数据。

有 **实例变量** 和 **类变量** 两种

 **类变量** :所有类实例共享的变量，属于类，通过 **类名.类变量**的形式访问。

- 构造方法

一种特殊的函数，**用于初始化类的成员变量**

 _ _init_ _()方法，它的第一个参数为self，之后的参数用来初始化实例变量。

在调用构造方法时不需要传入self参数。



==Python中前后用两个下划线包起来的叫做魔术方法==

```python
常用的魔术方法：
__init__：
1.用来构造初始化函数，用来给对象进行初始化属性，所以不需要返回值
2.创建对象的时候自动调用
3.自定义类如果不定义的话，默认调用父类object的，同理继承也是，子类若无，调用父类的，若有，调用自己的

class Animal:
    def __init__(self):
        print("init初始化方法，没有调用父类object")

Animal()
#结果：
init初始化方法，没有调用父类object

__new__：
1.用所给类创建一个对象，并且返回这个对象
2.因为是给类创建实例，所以至少传一个参数cls，参数cls代表代表要实例化的类，此参数在实例化时用python解释器自动提供
3.在类实例化时内部创建类实例的函数，并且返回这个实例，所以它是实例时最先被调用的方法，一般不要人为定义该方法
4.因为要创建实例返回实例，所以要有返回值。return父类__new__出来的实例，或者直接是object的__new__出来的实例

__class__

__delattr__
__dict__
__dir__
__doc__
__eq__
__format__
__ge__
__getattribute__
__gt__
__hash__
__init__
__init_subclass__
__le__
__lt__
__module__
__ne__
__new__
__reduce__
__reduce_ex__
__repr__
__setattr__
__sizeof__
__str__
__subclasshook__
__weakref__
```

- 成员方法

写在**类中的函数**，我们通常称之为（对象的）方法

有 **实例方法** 和 **类方法** 两种

定义**实例方法**时，它的第一个参数也应该时self，这会将当前实例与该方法绑定起来，这也说明该方法属于实例。

在调用方法时不需要传入self，类似于构造方法。

创建对象调用构造方法时，**省略默认值**。

访问类方法：**类名.类方法**。

注意：**类方法可以访问类变量和其他类方法，但是不能访问其他实例方法和实例变量**。

- 属性（property）

对类进行封装而提供的特殊方法

```python
class Person:
    run_speed = 0.1  # 类变量

    def __init__(self, name, age,sex='男'):  # 构造方法,可以用等号自带默认值
        # 创建和初始化实例变量
        self.name = name
        self.age = age

    def eat(self):  # 实例方法
        print('{0}在吃饭...'.format(self.name))

    def speak(self):  # 实例方法
        print('{0}在说话...'.format(self.name))

    # 类方法
    @classmethod
    def run(cls):  # 这里的cls代表这自身，可用Person代替
        return cls.run_speed


p = Person('张三', 18)  # 创建对象
print(p.name)  # 访问实例变量
p.eat()  # 调用实例方法
print(Person.run_speed)  # 访问类变量
speed = Person.run()  # 访问类方法
```

==访问限制==

如果想把某些属性给隐藏起来，不想让外界直接访问，可以在属性名前面加两个下划线。

比如帅帅不想直接让别人知道他的年龄或者修改他的年龄：

可以使用单下划线，双下划线，首尾双下划线来限制访问权限

**单下划线开头的是protected类型的成员**，只允许类本身和子类进行访问，不能使用from xxx import ccc进行导入

**双下划线只能由定义了该属性或方法的类调用**，而不能由类的对象调用，类的对象如果想调用，必须使用set/get方法

首尾双下划线是系统定义的特殊方法，一般是系统定义的名字

```python
class Person:
    def __init__(self, name,sex):
        self.name = name
        self.__age = None
        self.sex = sex

    def set(self,age):
        self.__age = age

    def get(self):
        return self.__age

    def sing(self):
        print(f"{self.name}唱的真好听")

    def dump(self):
        print(f"{self.name}跳的真不错")

    def rap(self):
        print(f"{self.name}世界第一")


shuaishuai = Person("帅帅","superman")  # 初始化
#这个时候初始化帅帅的年龄就会报错，可以使用set方法来赋值，get方法取值
shuaishuai.set(18)
print(shuaishuai.get())
```

==创建用于计算的属性==
有的时候我们需要创建对象的时候就进行给属性赋值，

但是这样的方法往往是不安全的，会直接修改我们类中的属性，这样的话安全性不高。

比如你的年龄是18岁，但是这个时候有用户进行恶作剧，直接将其修改为600岁，你是不是乐坏了？但是你感觉现实吗？

python中使用**@property**将一个方法转换为属性，从而实现用于计算的属性，

将方法转换为属性后，可以直接通过方法名来访问，而**不需要加括号**。

```python
class Person:
    def __init__(self,name,age):
        self.name = name
        self.age = age
@property
def func(self):
    if self.age < 150 and self.age > 0:
        print(self.age)
    else:
        print("想啥呢？")
shuaishuai = Person("帅帅",18)
shuaishuai.func  #func这个属性不能对其赋值，因为他本质也是一个函数
```


**@property可以将属性设置为只读属性**

==为属性添加安全保护机制==

为此，python中有了私有属性和私有方法供大家使用。

私有属性就是在属性前面加两个下划线，然后**给这个私有属性给予set和get方法**，这样对象调用的时候就只能通过set方法来进行赋值，get方法来获取值

```python
class Person:
    def __init__(self, name,sex):
        self.name = name
        self.__age = None
        self.sex = sex
def set(self,age):
    self.__age = age

def get(self):
    return self.__age
```









==拓展：==

### （1）self是什么？

首先，我们要明白self不是一个关键字，在类中，你也可以不用self，你也可以使用其他名字。

之所以将其命名为 self，只是程序员之间约定俗成的一种习惯，遵守这个约定，可以使我们编写的代码具有更好的可读性。

那self这个参数在我们的类中指的是什么呢？

**self，英文单词意思很明显，表示自己，本身。**

self在类中表示的是对象本身。在类的内部，通过这个参数访问自己内部的属性和方法。

```python
# 在这个类中，self表示一个类范围内的全局变量，在这个类中任何方法中，都能访问self绑定的变量
# 同时也能访问self绑定的函数
class Person(object):
    def __init__(self, name, gender):
        self.name = name
        self.talk()  # 访问self绑定的方法

    def talk(self):  # 参数为self，这个函数是对象的方法
        print(self.name)
```

## 6、调用类的三种方法

### **（1）实例方法**

```python
class dd:
    def __init__(self,url):
        self.url=url
    def runx(self):
        print requests.get(self.url).status_code

a = dd('http://www.baidu.com')
a.runx()
# 这种调用方法就是实例方法
```

### **（2）静态方法**

静态方法由类调用，无默认参数。将实例方法参数中的self去掉，然后在方法定义上方加上**@staticmethod**，就成为静态方法。它属于类，和实例无关。建议只使用**类名.静态方法**的调用方式。（虽然也可以使用实例名.静态方法的方式调用）

```python
class ff:
    @staticmethod
    def runx():
        print requests.get('http://www.baidu.com').status_code
ff.runx()
#这里就直接调用了类的变量，只在类中运行而不在实例中运行的方法
```

**经常有一些跟类有关系的功能但在运行时又不需要实例和类参与的情况下需要用到静态方法**. 比如更改环境变量或者修改其他类的属性等能用到静态方法. 这种情况也可以直接用函数解决, 但这样同样会扩散类内部的代码，造成维护困难。

### **（3）类方法**

类方法由类调用，采用@classmethod装饰，至少传入一个cls（代指类本身，类似self）参数。执行类方法时，自动将调用该方法的类赋值给cls。建议只使用类名.类方法的调用方式。（虽然也可以使用实例名.类方法的方式调用）

### **实际案例**

如果要构造一个类，接受一个网站和这个网站的状态码，然后打印出来。就像这样：

```text
import sys
import requests
reload(sys)
sys.setdefaultencoding('utf-8')
class gg:
    def __init__(self,url,stat):
        self.url=url
        self.stat=stat
    def outer(self):
        print self.url
        print self.stat
a = gg('langzi',200)
a.outer()
```

这样就是使用实例方法，虽然可以实现，但是有的时候传入的参数并不是(‘langzi’,200)这样的格式，而是(‘langzi-200’)这样的，那该怎么做？首先要把这个拆分，但是要使用实例方法实现起来很麻烦，这个时候就可以使用类方法。

```text
# -*- coding: utf-8 -*-
# @Time    : 2018/5/3 0003 17:27
# @Author  : Langzi
# @Blog    : www.langzi.fun
# @File    : 面向对象5.py
# @Software: PyCharm
import sys
import requests
reload(sys)
sys.setdefaultencoding('utf-8')
class gg:
    url = 0
    stat = 0
    # 因为使用classmethod后会传入新的变量，所以一开始是需要自己先定义类变量
    def __init__(self,url=0,stat=0):
    # 这里按照正常的定义构造函数
        self.url=url
        self.stat=stat
    @classmethod
    # 装饰器，立马执行下面的函数
    def split(cls,info):
        # 这个函数接受两个参数，默认的cls就是这个类的init函数，info就是外面传入进来的
        url,stat=map(str,info.split('-'))
        # 这里转换成了格式化的结构
        data = cls(url,stat)
        # 然后执行这个类第一个方法，这个类构造函数需要传入两个参数，于是就传入了两个参数
        return data
        # 这里就直接返回了函数结果
    def outer(self):
        print self.url
        print self.stat

r = gg.split(('langzi-200'))
r.outer()
# 这里是调用类方法，与调用实例方法一样
```

## 7、类与类之间的关系

一个一个的类就跟我们现实世界中的模板一样，只有把他们**全部关联起来**，才会使我们做事更加高效。

比如轮胎跟发动机组合成了车，零食跟零食袋组合成了零食一样。类和类的组合，一般分为以下三种关系：

### （1）依赖(关联)

一个动作执行的时候，需要另一个动作来帮忙。

比如打开电脑，帅帅去玩电脑或者帅帅去打王者

依赖就是我用你，你需要我。

比如帅帅玩电脑，电脑需要帅帅玩

```python
#依赖
class Person:
    def run(self):
        print("我没事干")

class Computer:
    def play(self,tool):
        tool.run()
        print("我是电脑，玩我")


class Phone:
    def play(self,tool):
        tool.run()
        print("我有王者荣耀，来玩啊")

shuaishuai = Person()
dnf = Computer()
dnf.play(shuaishuai)   #依赖是给一个类的对象的方法给另一个对象

wangzhe = Phone()
wangzhe.play(shuaishuai)
```

一个类使用某个类中的某个方法

这种情况下，类与类之间的关系是最轻的，可以随时替换。

**依赖就是一个类的对象的方法自己完不成一些功能，需要另一个对象来完成，把他加载到此方法中。**

### （2）组合(聚合)

**一个类需要某个类的具体对象去做一些事情**，这就是组合。轮胎和发动机组合成了车一样。

组合可以一对一，也可以一对多。

一个类与另一个类没有共同点，但是他们之间有关系，这就是组合

组合就是我需要什么，但是我没有这些东西，我就拿你。

将一个类的对象封装到另一个类的属性中进行一些操作

```python
class Car:
    def __init__(self,name,power = None):
        self.__name = name
        self.__power = power
    def set_power(self,power):
        self.__power = power

    def zhuang_Tread(self):
        print(f"{self.__name}装好了{self.__power.get_name()}的轮胎")

    def saiche_power(self):
        print(f"{self.__name}装好了{self.__power.get_name()}的发动机")
class Tread:
    def __init__(self,name):
        self.__name = name
    def set_name(self,name):
    	self.__name = name

	def get_name(self):
    	return self.__name
class Engine:
    def __init__(self,name):
        self.__name = name
    def set_name(self,name):
    	self.__name = name

    def get_name(self):
        return self.__name
tread = Tread("牛逼牌")
engine = Engine("赛车")
car = Car("奔驰",tread)
car.zhuang_Tread()
car.set_power(engine)
car.saiche_power()
```

## 8、面向对象的三大特性

![image-20231022155641790](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231022155641790.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### 1、封装

封装：把客观事物封装成抽象的类，隐藏属性和方法的实现细节，**仅对外公开接口**。

概念很拗口，但是思想却很简单。

封装隐藏了对象的内部细节，只保留有限的对外接口，外部调用者不用关心对象的内部细节，使得操作对象变得简单。

> 回到我们的冰箱、洗衣机，他们的共同特征是什么呢？
>
> 能装东西、能开门、能关门。
>
> 这些是他们的共性，我们就可以向上封装。
>
> 把能装东西、关门、开门封装起来。并且给他一个统称叫做：可开关盒子。
>
> 可开关盒子就是一个类。
>
> 这个类的所有对象都可以装东西、开门、关门。

封装可以把计算机中的数据跟操作这些数据的方法组装在一起，把他们封装在一个模块中，也就是一个类中。

```python
class Box():
    """盒子类，实现了开门、关门方法"""

    def open_door(self):
        pass

    def close_door(self):
        pass
```

- 私有变量

为了防止外部调用这随意存取类的内部数据（成员变量），内部数据（成员变量）会被封装为“私有变量”。

外部调用者只能通过方法调用私有变量。

在默认情况下，Python中的变量是公有的，可以在类的外部访问它们。

如果想让它们成为私有变量，则在变量前加上双下划线（__）即可。



在Python中，实例的变量名如果以双下划线开头，就变成了一个私有变量(`private`)，只有内部可以访问，外部不能访问。

==前置单下划线 `_xx`==

前置单下划线只有约定含义。程序员之间的相互约定，对Python解释器并没有特殊含义。

```python
class Person(object):
    def __init__(self, name):
        self._name = "我是一个伪私有变量"

>>> p = Person()
>>> print(p._name)
我是一个私有变量
```

我们看见，类并没有阻止我们访问变量 `_name`

> 所以：以单下划线开头的名称只是Python命名中的约定，表示供内部使用。它通常对Python解释器没有特殊含义，仅仅作为对程序员的提示。意思就是，“虽然我可以被访问，但是，请把我视为私有变量，不要随意访问”。

==前置双下划线 `__xx`==

实例的变量名如果以双下划线开头，就变成了一个私有变量(`private`)，只有内部可以访问，外部不能访问

```python
class Person(object):
    def __init__(self):
        self.__name = "我是一个私有变量"

>>> p = Person()
>>> print(p.__name)
Traceback (most recent call last):
  File "/app/util-python/python-module/obj.py", line 6, in <module>
    print(p.__name)
AttributeError: 'Person' object has no attribute '__name'
```

但我们访问 __name 的时候，报错了，阻止了我们在实例外部访问私有变量。这样就确保了外部代码不能随意修改对象内部的状态，这样通过访问限制的保护，代码更加健壮

```python
class Person(object):
    def __init__(self):
        self.__name = "我是一个私有变量"

    def __talk(self):
        print("sdsd")

p = Person()
p.__talk()
Traceback (most recent call last):
  File "/app/util-python/python-module/obj.py", line 9, in <module>
    p.__talk()
AttributeError: 'Person' object has no attribute '__talk'
```

那是真的彻底不能访问了吗？其实不是的

```python
print(p._Person__name)
我是一个私有变量
```

不能直接访问`__name`是因为Python解释器对外把`__name`变量改成了`_Person__name`，所以，仍然可以通过`_Person__name`来访问`__name`变量：

但是，最好不要这样做，Python的访问限制其实并不严格，主要靠自觉。

```python
class obj:
    def __init__(self,name):
        self.name=name
    def pri(self):
        print self.name
    __age = 18
    # 加上双下划线的就是私有变量，只能在类的内部访问，外部无法访问
a = obj('zhao')
a.pri()
```

运行结果：

```text
zhao
```

如果要在类中调用这个私有成员，可以这么用

```python
class obj:
    def __init__(self,name):
        self.name=name
    def prin(self):
        print self.name
    __age = 18
    # 加上双下划线的就是私有变量，只能在类的内部访问，外部无法访问
    @classmethod
    # 如果要在类中调用，首先调用类方法
    def pri(cls):
        print cls.__age
        # 然后在使用
a = obj('zhao')
a.prin()
obj.pri()
# 通过这样直接调用类中的私有变量
```

运行结果：

```text
zhao
18
```

- 私有方法

私有方法与私有变量的封装是类似的，在方法前加上双下划线（__）就是私有方法了。

- 使用属性

为了实现对象的封装，在一个类中不应该有公共的成员变量，这些成员变量应该被设计为私有的，然后通过公有的set和get方法进行访问。

**使用get-set-del方法操作私有成员**

```python
class obj:
    def __init__(self,name):
        self.name=name
    def prin(self):
        print self.name
    __age = 18
    # 加上双下划线的就是私有变量，只能在类的内部访问，外部无法访问
    @classmethod
    # 如果要在类中调用，首先调用类方法
    def pri(cls):
        print cls.__age
        # 然后在使用
    @classmethod
    def set_age(cls,value):
        cls.__age = value
        return cls.__age
        # 这个用法就是改变__age的值
    @classmethod
    def get_age(cls):
        return cls.__age
        # 这个用法就是直接返回__age的值
    @classmethod
    def del_age(cls):
        del cls.__age
        # 这个用法就是直接删除__age的值

print obj.get_age()
# 这里是直接调用出__age的值  返回值18
print obj.set_age(20)
# 这里是直接改变__age的值  返回值20
obj.del_age()
# 这里是直接删除__age的值
```

**Propety装饰器**

把类的方法**伪装成属性调用**的方式，就是把类里面的一个函数，变成一个属性一样的东西~

一开始调用类的方法要使用圆括号，现在变成了属性进行读取设置存储。

举个例子来说明：

**常用的调用方法**

```python
class obj:
    def __init__(self,name,age):
        self.__name=name
        self.__age=age
        # 讲这些设置成私有变量
    def get_age(self):
        return self.__age
    def set_age(self,value):
        if isinstance(value,int):
            self.__age=value
        else:
            raise ValueError('非整数类型')
    def del_age(self):
        print 'delete over'
a = obj('langzi',18)
print a.get_age()
a.set_age(20)
print a.get_age()
```

**使用装饰器**

在方法前加上装饰器使得方法成为属性。

属性使用起来类似于公有变量

```python
class obj:
    def __init__(self,name,age):
        self.__name=name
        self.__age=age
        # 把这些设置成私有变量
    @property
    def age(self):
        return self.__age
    @age.setter  # 定义age属性的set()方法，使用@age.setter装饰器进行修饰，age是属性名
    def age(self,value):
        if isinstance(value,int):
            self.__age=value
        else:
            raise ValueError('非整数类型')
    @age.deleter
    def age(self):
        print 'delete over'
a = obj('langzi',18)
# 使用这些装饰器，可以使用类与对象的方法直接调用
print a.age
# 这里就是直接调用返回age的值
a.age=20
# 这里就是直接使用setter把值转换
print a.age
del a.age
# 删除age
```

当然这种调用方法有些麻烦，每次都是一个一个去实例类与对象，有个更加简单直观的方法。

**更加减半的使用property()函数**

除了使用装饰器的方式将一个方法伪装成属性外，Python内置的**builtins模块中的property()函数**，为我们提供了第二种设置类属性的手段。

```python
class People:

    def __init__(self, name, age):
        self.__name = name
        self.__age = age

    def get_age(self):
        return self.__age

    def set_age(self, age):
        if isinstance(age, int):
            self.__age = age
        else:
            raise ValueError

    def del_age(self):
        print("删除年龄数据！")

    # 核心在这句
    age = property(get_age, set_age, del_age, "年龄")    


obj = People("jack", 18)
print(obj.age)
obj.age = 19
print("obj.age:  ", obj.age)
del obj.ag
```

通过语句age = property(get_age, set_age, del_age, “年龄”)将一个方法伪装成为属性。其效果和装饰器的方法是一样的。

property()函数的参数：

- 第一个参数是方法名，调用 **实例.属性** 时自动执行的方法 

- 第二个参数是方法名，调用 **实例.属性 ＝ XXX**时自动执行的方法 
- 第三个参数是方法名，调用 **del 实例.属性** 时自动执行的方法 
- 第四个参数是字符串，调用 **实例.属性.doc**时的描述信息。

==拓展==

**内置装饰器**

- @property

通过 @property 装饰器，可以直接通过方法名来访问方法，不需要在方法名后添加一对“（）”小括号。

> 修饰方法，使方法可以像属性一样访问。

**未加装饰器：**

```python
class Person(object):
    def __init__(self, name, age):
        self._name = name
        self._age = age

    def name(self):
        return self._name

p = Person("baozi", 26)
print(p.name)
# <bound method Person.name of <__main__.Person object at 0x7fb728643dd8>>

print(p.name())  # 没加装饰器，必须调用函数
# baozi
```

**加装饰器：**

```python
class Person(object):
    def __init__(self, name, age):
        self._name = name
        self._age = age

    @property
    def name(self):
        return self._name

p = Person("baozi", 26)
print(p.name)  # 加了装饰器，像访问属性一样，直接访问方法，不用再加()调用
# baozi
```

通过这个装饰器，我们可以像访问属性一样，直接访问方法。

那么，这个装饰器有什么用处呢？那我直接 `p.name()`不行吗？也能实现我的需求啊

确实是这样的。但是从代码可读性而言，我们想访问对象的属性，使用`p.name()`肯定是没有 `p.name`这么直观的。

> 他的使用场景是：我们想访问对象属性，又不想属性被修改的时候，就可以使用这个装饰器。

拓展一下：如果，我想改年龄，并且年龄需要一些限制条件该怎么办呢？

```python
class Person(object):
    def __init__(self, name, age):
        self._name = name
        self._age = age

    def set_age(self, age):
        if age <= 0:
            raise ValueError('age must be greater than zero')
        self._age = age

    def get_age(self):
        return self._age
```

有问题吗？没有问题，那我能不能通过刚才那个装饰器来玩呢？也可以

```python
class Person(object):
    def __init__(self, name, age):
        self._name = name
        self._age = age

    @property
    def age(self):
        return self._age

    @age.setter
    def age(self, age):
        if age <= 0:
            raise ValueError('age must be greater than zero')
        self._age = age
```

看到这里，小伙伴可能会有点疑惑了？`@age.setter`这又是何方神圣？怎么蹦出来的？它也是一个装饰器。这个装饰器在属性赋值的时候会被调用。

> `@*.setter` 装饰器必须在`@property`的后面，且两个被修饰的属性（函数）名称必须保持一致。`*`即为函数名

使用这两个装饰器，我们就可以做很多事情了。比如：实现密码的密文存储和明文输出、修改属性前判断是否满足条件等等。

为两个同名函数打上@*.setter装饰器和@property装饰器后：

1. 当把类方法作为属性**赋值**时会触发@*.setter对应的函数

2. 当把类方法作为属性**读取**时会触发@property对应的函数



- @staticmethod

将类中的方法装饰为静态方法，即**类不需要创建实例的情况下，可以通过类名直接引用**。

```python
class Person(object):
    def __init__(self, name, age):
        self._name = name
        self._age = age

    # 此方法只能是类的实例调用
    def talk(self):
        print(f"name is {self._name} age is {self._age}")

    # 此方法没有就像普通的函数一样，直接通过 Person.talk()就可以直接调用
    @staticmethod
    def static_talk(name, age): # 这里无需再传递self，函数不用再访问类
        print(f"name is {name} age is {age}")
p = Person("baozi", 26) # 正常

p.static_talk("baozi", 26)  # 报错，该方法是个静态方法，不能通过实例访问
# Traceback (most recent call last):
# File "/app/util-python/python-module/obj.py", line 14, in <module>
#    p.static_talk("baozi", 60)
#TypeError: static_talk() takes 2 positional arguments but 3 were given


Person.static_talk("baozi", 60) # 正常

Person.talk() # 报错，这个方法没有被修饰，只能被实例访问，不能被类访问
# Traceback (most recent call last):
# File "/app/util-python/python-module/obj.py", line 15, in <module>
#  Person.talk()
# TypeError: talk() missing 1 required positional argument: 'self'
```

- @classmethod

这个装饰器修饰的方法是**类方法**，而不是实例方法。这句话是什么意思呢？我们常规定义的方法，都属于实例方法，必须要先创建实例以后，才能调用。但是类方法，无需实例化就可以访问。

类方法的第一个参数是类本身，而不是实例

```python
class Person(object):
    def __init__(self, name, age):
        self._name = name
        self._age = age

    @classmethod
    def static_talk(cls, name, age):
        print(f"name is {name} age is {age}")

Person.static_talk("baozi", 60)
```

怎么看起来跟我们的 @staticmethod 功能一样呢？其实注意细节的同学已经发现了。

我们 @classmethod修饰的函数，多了一个参数 cls，这个参数跟我们的self可不一样，**self指的是当前实例**，而我们的**cls指的是当前的类**。

1. @classmethod修饰的方法需要**通过cls参数传递当前类对象**，它可以访问类属性，不能访问实例属性

2. @staticmethod修饰的方法定义与普通函数是一样的，它不可以访问类属性，也不能访问实例属性

那这个装饰器又有什么用呢？

网上说的最多的就是用来做**实现多构造器**。什么叫多构造器呢？

```python
class Person(object):
    def __init__(self, age):
        self._age = age

    @classmethod
    def init_18_age_person_instance(cls):  # 这是一个类方法。这个方法只创建年龄为18岁的的对象。
        age = 18
        return cls(age)

    @classmethod
    def init_30_age_person_instance(cls):  # 这是一个类方法。这个方法只创建年龄为30岁的的对象。
        age = 30
        return cls(age)

p = Person(18) # 创建了一个实例，属性age = 18

p_18 = Person.init_18_age_person_instance() # 这里也创建了一个实例，属性age = 18

p_30 = Person.init_30_age_person_instance() # 这里也创建了一个实例，属性age = 30
```

当然我这里场景使用得不是很恰当，只是为了简单说明它的功能。通过这个函数，可以模拟出多构造器。具体的业务场景需要你们多多去挖掘。

### 2、继承

> 本段转载于[Python类的继承关系及super的用法 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/285244974)

继承：子类可以使用父类的所有功能，并且对这些功能进行扩展。继承的过程，就是从**一般到特殊**的过程。

> 继承的思想也很简单。
>
> 你有没有想过一个问题，你为什么长得像人，而不像猪？
>
> 首先，你爸是人，你妈也是人，你爸妈都有人的模样，你继承他们，就会继承他们的所有这些属性。
>
> 你一出生就会有人类共有的这些属性。
>
> 并且你可以对这些属性进行拓展，比如，你爸只会说中文，但是你会说中文、你拓展了这个方法，你还会说英文。

继承简单地说就是一种层次模型，这种层次模型能够被重用。

层次结构的**上层具有通用性**，但是**下层结构则具有特殊性**。

在继承的过程中类则可以从最顶层的部分继承一些方法和变量。

类除了可以继承以外同时还能够进行修改或者添加。通过这样的方式能够有效提高工作效率

```python
class Father:

    def talk(self):
        print("我会讲话")

    def breathe(self):
        print("我能呼吸")

class Me(Father):
    pass


me = Me()  # 我们的 Me 类，并没有实现下面两个方法，而是继承了 Father 类的方法
me.talk()
me.breathe()
我会讲话
我能呼吸
```

**组合继承：**

```python
class P1():
    def talk(self):
        print("我是p1")

class P2():
    def talk(self):
        print("我是p2")

class Person(P1, P2): # P1排在第一位，调用P1的talk()
    pass

p = Person()
p.talk()
# 我是p1
class P1():
    def talk(self):
        print("我是p1")

class P2():
    def talk(self):
        print("我是p2")

class Person(P2, P1): # P2排在第一位，调用P2的talk()
    pass

p = Person()
p.talk()
# 我是p2
```

这里注意一个小细节，当我继承自多个父类，多个父类都有相同的方法。那我调用的时候会调用谁的呢？

其实，是**按照继承参数的顺序**来的，**谁排在第一个就调用谁的方法**

### （1）不使用super的继承

**1.Python单继承**

```python3
class Goat(object):
    def __init__(self):
        self.name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class My_favor(Goat):
    pass
M = My_favor()
M.god()
>>> 乔丹将篮球推向了全世界
    乔丹是历史上最伟大的篮球运动员，篮球之神
```

**分析： My_favor继承了goat这个类，所以就拥有goat类的所有属性和方法。**

**2 Python多继承**

```python3
class Goat(object):
    def __init__(self):
        self.name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class Mamba(object):
    def __init__(self):
        self.name = "科比"
        print(f"{self.name}最具职业精神的伟大篮球运动员")
    def god(self):
        print(f"{self.name}是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我")

# class My_favor(Goat,Mamba):
class My_favor(Mamba,Goat):
    pass
M = My_favor()
M.god()
>>> 科比最具职业精神的伟大篮球运动员
    科比是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我
```

**分析：如果一个类继承多个父类的时候，优先继承的是第一个类的属性和方法，也即若想优先继承哪个类，就把哪个类放在最前面即可。**

```python3
class Goat(object):
    def __init__(self):
        self.name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class Mamba(object):
    def __init__(self):
        self.name = "科比"
        print(f"{self.name}最具职业精神的伟大篮球运动员")
    def god(self):
        print(f"{self.name}是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我")

# class My_favor(Goat,Mamba):
class king_james(Mamba,Goat):
    def __init__(self):
        self.name = "詹姆斯"
        print(f"{self.name}最全能的伟大的篮球运动员")
    def god(self):
        print(f"{self.name}是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员")
M = king_james()
M.god()
>>> 詹姆斯最全能的伟大的篮球运动员
    詹姆斯是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员
```

**分析：如果子类和父类拥有同名属性和方法，子类创建对象调用属性和方法的时候，调用到的是==子类里面==的同名属性和方法。**

```python3
print(king_james.__mro__)

>>> (<class '__main__.king_james'>, <class '__main__.Mamba'>, <class '__main__.Goat'>, <class 'object'>)
```

**分析：当代码比较复杂时，可通过_ _mro_ _方法来查看具体某个类的继承关系。**

```python3
class Goat(object):
    def __init__(self):
        self.name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class Mamba(object):
    def __init__(self):
        self.name = "科比"
        print(f"{self.name}最具职业精神的伟大篮球运动员")
    def god(self):
        print(f"{self.name}是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我")

# class My_favor(Goat,Mamba):
class king_james(Mamba,Goat):
    def __init__(self):
        self.name = "詹姆斯"
        # print(f"{self.name}最全能的伟大的篮球运动员")
    def god(self):
        print(f"{self.name}是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员")
    def god_goat(self):
        Goat.__init__(self)
        Goat.god(self)
    def god_mamba(self):
        Mamba.__init__(self)
        Mamba.god(self)
#print(king_james.__mro__)
M = king_james()
M.god_mamba()

>>> 科比最具职业精神的伟大篮球运动员
    科比是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我
```

**分析：如果在子类中想调用父类的同名属性和方法，则需要在子类中重新定义函数（再次封装），且进行初始化。**

子类的方法会重写（Override）父类的同名方法

**3 多层继承**

```python
class Goat(object):
    def __init__(self):
        self.name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class Mamba(object):
    def __init__(self):
        self.name = "科比"
        print(f"{self.name}最具职业精神的伟大篮球运动员")
    def god(self):
        print(f"{self.name}是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我")

# class My_favor(Goat,Mamba):
class king_james(Mamba,Goat):
    def __init__(self):
        self.name = "詹姆斯"
        print(f"{self.name}最全能的伟大的篮球运动员")
    def god(self):
        print(f"{self.name}是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员")
    def god_goat(self):
        Goat.__init__(self)
        Goat.god(self)
    def god_mamba(self):
        Mamba.__init__(self)
        Mamba.god(self)
class fat_tiger(king_james):
    pass
# print(king_james.__mro__)
fat = fat_tiger()
fat.god()
fat.god_goat()
fat.god_mamba()
>>> 詹姆斯最全能的伟大的篮球运动员
    詹姆斯是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员
    乔丹将篮球推向了全世界
    乔丹是历史上最伟大的篮球运动员,篮球之神
    科比最具职业精神的伟大篮球运动员
    科比是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我
```

**分析：如上所示，多层继承也完全可以实现调用父类函数及属性。**

### （2）使用super的继承

上述方法在继承父类的属性和方法时，若父类的类名修改的话，子类在继承的时候也要相应的进行修改，同时代码量大，复杂。接下里介绍super方法继承。

**1. 继承一个类**

```python3
class Goat(object):
    def __init__(self):
        self.name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class Mamba(object):
    def __init__(self):
        self.name = "科比"
        print(f"{self.name}最具职业精神的伟大篮球运动员")
    def god_mamba(self):
        print(f"{self.name}是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我")

# class My_favor(Goat,Mamba):
class king_james(Mamba):
    def __init__(self):
        self.name = "詹姆斯"
        print(f"{self.name}最全能的伟大的篮球运动员")
    def god(self):
        print(f"{self.name}是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员")
        super().__init__()
        super().god_mamba()

# print(king_james.__mro__)
M = king_james()
M.god()

>>> 詹姆斯最全能的伟大的篮球运动员
    詹姆斯是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员
    科比最具职业精神的伟大篮球运动员
    科比是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我
```

**分析：使用super来继承Mamba这个类。**

**2. 继承多个类**

```python
class Goat(object):
    def __init__(self):
        self.name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god_goat(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class Mamba(Goat):
    def __init__(self):
        self.name = "科比"
        print(f"{self.name}最具职业精神的伟大篮球运动员")
        super().__init__()
        super().god_goat()
    def god_mamba(self):
        print(f"{self.name}是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我")

# class My_favor(Goat,Mamba):
class king_james(Mamba):
    def __init__(self):
        self.name = "詹姆斯"
        print(f"{self.name}最全能的伟大的篮球运动员")
    def god(self):
        print(f"{self.name}是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员")
        super().__init__()
        super().god_mamba()

# print(king_james.__mro__)
M = king_james()
M.god()

>>> 詹姆斯最全能的伟大的篮球运动员
    詹姆斯是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员
    科比最具职业精神的伟大篮球运动员
    乔丹将篮球推向了全世界
    乔丹是历史上最伟大的篮球运动员,篮球之神
    乔丹是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我
```

**分析：同时调用多级类。**

**3. 定义私有属性和方法**

```python3
class Goat(object):
    def __init__(self):
        self.__name = "乔丹"
        print(f"{self.name}将篮球推向了全世界")
    def god_goat(self):
        print(f"{self.name}是历史上最伟大的篮球运动员,篮球之神")

class Mamba(Goat):
    def __init__(self):
        self.name = "科比"
        print(f"{self.name}最具职业精神的伟大篮球运动员")
        super().__init__()
        super().god_goat()
    def god_mamba(self):
        print(f"{self.name}是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我")

# class My_favor(Goat,Mamba):
class king_james(Mamba):
    def __init__(self):
        self.name = "詹姆斯"
        print(f"{self.name}最全能的伟大的篮球运动员")
    def god(self):
        print(f"{self.name}是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员")
        super().__init__()
        super().god_mamba()

# print(king_james.__mro__)
M = king_james()
M.god()

>>> 詹姆斯最全能的伟大的篮球运动员
    詹姆斯是历史上唯一一个为三个城市带来总冠军且获得FMVP的球员
    科比最具职业精神的伟大篮球运动员
    科比将篮球推向了全世界
    科比是历史上最伟大的篮球运动员,篮球之神
    科比是我最喜欢的篮球运动员，他的曼巴精神深深鼓励了我
```

**分析：设置私有属性或者函数，在属性或者函数前加”__“即可。由于上面中self.__name = "乔丹"，设置了私有属性，所以只能用Mamba的初始化来进行执行。**

### 3、多态

> 本段转载于[python中对多态的理解 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/88402677)
>
> [Python中的多态如何理解？_python多态的理解-CSDN博客](https://blog.csdn.net/weixin_44695969/article/details/92175840)

### （1）初识多态

多态指的是一类事物有多种形态，（一个抽象类有多个子类，因而多态的概念依赖于继承）

**子类所创建的对象采用不同的方式实现父类方法**

> 你爸有一个talk()方法，也就是说话，你继承了你爸的talk()方法，
>
> 对于同样的talk()方法，你爸讲中文，你讲英语，你弟弟讲俄语、你妹妹讲韩语，这就是多态

```python
# 爸爸类
class Father:
    def talk(self):
        print("我会讲话，我讲的是中文")

# 继承自爸爸类
class Me(Father):
    def talk(self):
        print("我是哥哥，我讲英语：hello，world")

# 继承自爸爸类
class Son(Father):
    def talk(self):
        print("我是弟弟，我讲俄语：Всем привет")

# 继承自爸爸类
class Sister(Father):
    def talk(self):
        print("我是妹妹，我讲韩语：전 세계 여러분 안녕하세요")

me = Me()
son = Son()
sister = Sister()

me.talk()
son.talk()
sister.talk()
我是哥哥，我讲英语：hello，world
我是弟弟，我讲俄语：Всем привет
我是妹妹，我讲韩语：전 세계 여러분 안녕하세요
```

> 多态存在的三个必要条件

1. 要有继承
2. 要有重写；
3. 父类引用指向子类对象。

### （2）多态性

**注意**：多态与多态性是两种概念

多态性是指具有**不同功能的函数可以使用相同的函数名**，这样就可以用一个函数名调用不同内容的函数。

在面向对象方法中一般是这样表述多态性：向不同的对象发送同一条消息，不同的对象在接收时会产生不同的行为（即方法）。

也就是说，每个对象可以用自己的方式去响应共同的消息。

所谓消息，就是调用函数，不同的行为就是指不同的实现，即执行不同的函数。

```python
import abc
class Animal(metaclass=abc.ABCMeta): #同一类事物:动物
    @abc.abstractmethod
    def talk(self):
        pass

class Cat(Animal): #动物的形态之一:猫
    def talk(self):
        print('say miaomiao')

class Dog(Animal): #动物的形态之二:狗
    def talk(self):
        print('say wangwang')

class Pig(Animal): #动物的形态之三:猪
    def talk(self):
        print('say aoao')

c = Cat()
d = Dog()
p = Pig()

def func(obj):
    obj.talk()

func(c)
func(d)
func(p)

------------------------------

>>> say miaomiao
>>> say wangwang
>>> say aoao
```

综上可以说，多态性是 : **一个接口,多种实现**

**多态性的好处:**

- 增加了程序的灵活性,以不变应万变，不论对象千变万化，使用者都是同一种形式去调用，如func(obj)
- 增加了程序额可扩展性,通过继承animal类创建了一个新的类，使用者无需更改自己的代码，还是用func(obj)去调用

### （3）鸭子类型

调用不同的子类将会产生不同的行为，而无须明确知道这个子类实际上是什么，这是多态的重要应用场景。

而在python中，因为鸭子类型(duck typing)使得其多态不是那么酷。

鸭子类型是动态类型的一种风格。

在这种风格中，一个对象有效的语义，不是由继承自特定的类或实现特定的接口，而是由"**当前方法和属性的集合**"决定。

这个概念的名字来源于由James Whitcomb Riley提出的鸭子测试，

“鸭子测试”可以这样表述：“**当看到一只鸟走起来像鸭子、游泳起来像鸭子、叫起来也像鸭子，那么这只鸟就可以被称为鸭子**。”

在鸭子类型中，关注的不是对象的类型本身，而是它是如何使用的。

例如，在不使用鸭子类型的语言中，我们可以编写一个函数，它接受一个类型为"鸭子"的对象，并调用它的"走"和"叫"方法。

在使用鸭子类型的语言中，这样的一个函数可以接受一个任意类型的对象，并调用它的"走"和"叫"方法。如果这些需要被调用的方法不存在，那么将引发一个运行时错误。

任何拥有这样的正确的"走"和"叫"方法的对象都可被函数接受的这种行为引出了以上表述，这种决定类型的方式因此得名。

鸭子类型通常得益于不测试方法和函数中参数的类型，而是依赖文档、清晰的代码和测试来确保正确使用。

**Duck typing** 这个概念来源于美国印第安纳州的诗人詹姆斯·惠特科姆·莱利（James Whitcomb Riley,1849- 1916）的诗句：”When I see a bird that walks like a duck and swims like a duck and quacks like a duck, I call that bird a duck.”

先上代码，也是来源于网上很经典的案例：

```python
class Duck():
    def walk(self):
         print('I walk like a duck')
    def swim(self):
         print('i swim like a duck')

class Person():
    def walk(self):
     　　print('this one walk like a duck') 
    def swim(self):
     　　print('this man swim like a duck')
```

可以很明显的看出，Person类拥有跟Duck类一样的方法，当有一个函数调用Duck类，并利用到了两个方法walk()和swim()。我们传入Person类也一样可以运行，函数并不会检查对象的类型是不是Duck，只要他拥有walk()和swim()方法，就可以正确的被调用。

再举例，如果一个对象实现了**getitem**方法，那Python的解释器就会把它当做一个collection，就可以在这个对象上使用切片，获取子项等方法；如果一个对象实现了**iter**和next方法，Python就会认为它是一个iterator，就可以在这个对象上通过循环来获取各个子项。

==拓展==：

Java中多态性的表现： 多态性，可以理解为一个事物的多种形态。

同样中也支持多态，但是是有限的的支持多态性，主要是因为Python中变量的使用不用声明，所以**不存在父类引用指向子类对象的多态体现**，同时**Python不支持重载**。

在Python中 多态的使用不如Java中那么明显，所以Python中刻意谈到多态的意义不是特别大。

Java中多态的体现：

- 方法的重载(overload)和重写(overwrite)。
- 对象的多态性（将子类的对象赋给父类的引用）——可以直接应用在抽象类和接口上

广义上：①方法的重载、重写 ②子类对象的多态性

狭义上：子类对象的多态性（在Java中,子类的对象可以替代父类的对象使用）

## 9. 尝试理解一下一切皆对象

通过我们上面介绍的一些内置方法以后，我们或许对**一切皆对象**有了更进一步的认识。

此时我们发现，我们的str、int、dict、list、tuple这些其实本质上都是一个对象。针对不同的数据结构，它们自己重写了自己的一套内置方法来实现不同的功能。

比如字典 dict["key"] 的取值方式就是实现了我们之前介绍的：`__setitem__`、`__getitem__`....

比如我们的字符串"hello,world"，它不是一个静态的字符串，他也是一个对象，他也有很多内置方法，我们能看到"hello,world"，是因为它实现了`__str__()`

==拓展==

魔法方法

![image-20231023003342633](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231023003342633.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

# 十一、异常处理

>  本段转载于[深入理解Python异常处理：从基础到高级-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/2330624)
>
> [基础 | 彻底搞懂Python异常处理：try-except-else-finally - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/360807803)

## 1、初识异常

在编程中，异常是程序运行过程中的错误或异常情况的表示。当发生异常时，程序不会按照正常流程继续执行，而是跳转到异常处理代码。

**异常**：程序正常执行过程中出现的不正常的情况，该情况影响了程序的正常执行。

**异常程序**：是指程序执行的非法指令，比如常见的非法操作码，地址越界，算术溢出等，异常程序的出现一般有两种情况：

- 程序设计时的编程错误或程序运行时的硬件错误
- 精心设计地入侵系统程序（病毒）

 ==异常的种类==

Python中有许多内置的异常类，每个异常类用于表示不同类型的错误。常见的异常包括：

- `SyntaxError`：语法错误
- `IndentationError`：缩进错误
- `NameError`：变量名未定义
- `TypeError`：类型不匹配
- `ValueError`：值错误
- `ZeroDivisionError`：除零错误
- `FileNotFoundError`：文件未找到

==拓展==

程序运行出错时会有**Traceback**信息。

**Traceback信息**是“异常堆栈信息”，描述了程序运行的过程以及引发异常的信息。

包括：

- 哪个.py 文件出现了异常
- 第几行出现了异常
- 发生异常的表达式（语句）
- 发生了什么异常，异常信息表达式

在Python中，异常类命名的主要后缀有 **Exception**、**Error**、**Warning**。

## 2、捕获并处理异常

### （1）try-except语句

**可以嵌套使用**

异常处理通过`try`和`except`语句实现。`try`块包含可能引发异常的代码，而`except`块包含处理异常的代码。

在except语句中可以指定具体的异常类型。

如果不指定：except语句可以捕获在try中发生的额所有异常；

如果指定（推荐）：except语句只能捕获在try中发生的指定类型的异常。

```python
try:
    # 可能引发异常的代码
    result = 10 / 0
except ZeroDivisionError as e:  # 其中e是异常对象，是一个变量
    # 处理异常的代码
    print("除零错误发生")
```

### （2）多个except代码块

一个`try`块可以包含多个`except`块，用于处理不同类型的异常。

多条语句可能引发多种不同的异常，对每一种异常都会采用不同的处理方式。

```python
try:
    result = int("abc")
except ValueError:
    print("值错误")
except ZeroDivisionError:
    print("除零错误")
except:  # 范围最广，捕获上面没有匹配的异常类
    print("其他异常")
```

### （3）多重异常捕获

如果多个except代码块的异常处理过程类似，可以合并处理。

```python
try:
    result = int("abc")
except (ValueError, ZeroDivisionError) as e:
    print("异常发生:{}".format(e))
```

### （4）else 和 finally

- **try**：正常情况下，程序计划执行的语句。
- **except**：程序异常是执行的语句。
- **else**：程序无异常即try段代码正常执行后会执行该语句。
- **finally**：不管有没有异常，都会执行的语句。

`else`块在`try`块中没有引发异常时执行，而`finally`块始终执行，无论是否引发异常。

通常情况下，在try-except语句中会占用一些资源，例如：打开的文件、网络 连接、打开的数据库以及数据结果集等都会占用计算机资源，需要程序员释放这些资源。

为了确保这些资源能够被释放，可以使用finally代码块。

```python
try:
    result = 10 / 2
except ZeroDivisionError:
    print("除零错误")
else:
    print("计算结果：", result)
finally:
    print("无论如何都会执行的代码")
```

## 3、异常对象

### （1）异常信息

`except`块可以访问异常对象，它包含有关异常的详细信息，如异常类型和描述。

```python
try:
    result = int("abc")
except ValueError as e:
    print("异常类型：", type(e))
    print("异常描述：", e)
```

### （2）抛出异常

使用`raise`语句可以手动引发异常。

```python
def divide(x, y):
    if y == 0:
        raise ZeroDivisionError("除零错误")
    return x / y

try:
    result = divide(10, 0)
except ZeroDivisionError as e:
    print("异常类型：", type(e))
    print("异常描述：", e)
```

## 4、自定义异常类

你也可以创建自定义异常类，以便更好地组织和处理特定类型的错误。

实现自定义异常类，需要继承Exception类或其子类。

ZeroDivisionError 和 ValueError 异常都属于 Exception 的子类。

```python
class MyError(Exception):
    def __init__(self, message):  # 构造方法,message是异常描述信息
        super().__init__(message)  # 调用父类构造方法，并把参数message传给父类构造方法

try:
    raise MyError("自定义异常发生")
except MyError as e:
    print("异常类型：", type(e))
    print("异常描述：", e)
```

## 5、return的处理

![image-20231023081329974](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231023081329974.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- try-except-finally（存在异常）

优先finally中的return，其次在except中的return

- try-else-finally（不存在异常且try中无return）

优先finally中的return，其次在else中的return

- try-finally（不存在异常且try中有return）

由于try中有return，else不执行

优先finally中的return，其次在try中的return

## 6、异常的使用建议

- 适度使用异常

异常应该用于处理意外的错误情况，而不应该用于控制流程。不要过度使用异常来替代条件语句。

- 具体而不是泛化

捕获特定类型的异常，而不是使用通用的`except`块。这样可以更精确地处理错误情况。

- 清理资源

在`finally`块中清理资源，如关闭文件或释放网络连接。确保在退出`try`块时始终执行。

- 记录异常信息

在处理异常时，建议记录异常信息，以便更容易调试和修复问题。

```python
import logging

try:
    result = 10 / 0
except ZeroDivisionError as e:
    logging.error("除零错误：%s", e)
```

- 异常处理链

在异常处理中可以使用多个`except`块，形成异常处理链，以处理不同类型的异常。

```python
try:
    result = int("abc")
except ValueError:
    print("值错误")
except TypeError:
    print("类型错误")
```

# 十二、常用的内置模块

> 本段转载于[python 常用的内置模块_python内置模块-CSDN博客](https://blog.csdn.net/ruanxingzi123/article/details/82787852)
>
> [Python常用的模块 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/101407848)

## 1、模块和包

### 1.模块介绍

- 模块定义:一系列功能的集合体
- 模块使用: import导入模块 或者 from ... import... 导入模块
- 模块分类:内置模块 自定义模块 第三方模块
- 模块加载顺序: 内存>内置>sys.path(环境变量中的路径时逐一加载的)
- 模块起别名: import 模块名 as 别名
- 模块两种被执行方式:

```python
1.一个py文件作为自执行文件，__name__变量的值为 '__main__'
if __name__ == '__main__':
    # 自执行的逻辑 => 因为在文件作为模块使用时 __name__为文件名，不满足条件
    pass
2.一个py文件作为模块被导入执行，__name__变量的值为 '文件(模块)名' 
此时被其他使用
```

### 2. 包的介绍

- 包的定义:

一系列模块的集合体,用文件件来管理一系列有联系的功能的模块,该文件夹称之为包,文件夹名就是包名

- 包与普通文件夹的区别:

包的文件夹中一定存在一个__init__.py文件文件

- __init__.py文件的作用

```python
1   产生一个全局名称空间提供给包使用 此名称空间就是包的名称空间
2   管理包     包可以直接点出来模块使用
```

- 导包完成的三件事

```python
# 导包完成的三件事
# 1）编译形成包中__init__.py文件的pyc文件
# 2）执行__init__.py文件，形成一个全局名称空间，将__init__.py文件中所有名字存放其中，该名称空间就代表包的名称空间
# 3）在导包的文件中，产生一个与包名相同的名字，指向包的名称空间(__init__.py文件的全局名称空间)
```

- 包的管理

```python
# 在包中采用相对导入管理模块或模块中的名字


# 在包的__init__.py文件或是包中任意一个模块中
# . 代表当前文件所在目录
# .. 代表当前文件所在目录的上一级目录
# 注：.语法不能出包，因为包外的文件都能自执行，但拥有.开头导入的文件不能自执行
```

## 2、数学计算模块（math）

> 本段转载于[Python math 模块 | 菜鸟教程 (runoob.com)](https://www.runoob.com/python3/python-math.html)

**import math**

- math模块常量

![image-20231024111200788](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024111200788.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- math模块方法

![image-20231024111239813](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024111239813.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231024111303724](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024111303724.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231024111321912](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024111321912.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231024111343975](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024111343975.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

![image-20231024111405399](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024111405399.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



## 3、日期时间模块（datatime）

参考：[Python3 日期和时间 | 菜鸟教程 (runoob.com)](https://www.runoob.com/python3/python3-date-time.html)

**提示**：在将日期时间与字符串相互转换的时候，提供的字符串应该可以表示一个有效的日期时间，否则会发生ValueError异常。

## 4、正则表达式模块（re）

> 本段转载于[Python内置模块之re库，一文搞定正则表达式的初阶用法 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/364210633)
>
> [python——正则表达式(re模块)详解_python re正则表达式-CSDN博客](https://blog.csdn.net/guo_qingxia/article/details/113979135)

就其本质而言，正则表达式（或 RE）是一种**小型的、高度专业化的**编程语言，（在Python中）它内嵌在Python中，并通过 re 模块实现。

正则表达式模式被编译成一系列的字节码，然后由用 **C 编写**的匹配引擎执行。

正则表达式指预定义好一个“**字符串模板**”，通过这个“**字符串模板**”可以匹配、查找和替换那些匹配“**字符串模板**”的字符串。

正则表达式实现的字符串查找替换操作效率更高、功能更强大。

难点在于 **编写字符串模板**。

几乎所有编程语言的正则表达式都是==通用的==。

re 库是 Python 中处理正则表达式的标准库

正则表达式是一个特殊的字符序列，它能帮助你方便的检查一个字符串是否与某种模式匹配。

Python 自1.5版本起增加了re 模块，它提供 Perl 风格的正则表达式模式。

re 模块使 Python 语言拥有全部的正则表达式功能。

compile 函数根据一个模式字符串和可选的标志参数生成一个正则表达式对象。该对象拥有一系列方法用于正则表达式匹配和替换。

re 模块也提供了与这些方法功能完全一致的函数，这些函数使用一个模式字符串做为它们的第一个参数。

**什么是原生字符？**

在正式学习之前，先了解一下原生字符串。

在 Python 中，**表示原生字符串，需要在字符串前面加上 r**。

例如 my_str = 'i'am xiangpica' 在程序中会直接报错，如果希望字符串中 ' 可以正常运行，需要加上转移字符 \，修改为 my_str = 'i \ 'am xiangpica'。

但这样结合上文正则表达式中的操作符，就会出现问题，因为 **\ 在正则表达式中是有真实含义的**，如果你使用 re 库去匹配字符串中的 \，那需要使用 4 个反斜杠，为了避免这种情况出现，引入了原生字符串概念。

```python
# 不使用原生字符串的正则表达式  "\\\\"
# 使用原生字符串的正则表达式 r"\\"
```

在后文会有实际的应用。

接下来在学习一个案例，例如下述代码：

```python
my_str='C:\number'
print(my_str)
C:
umber
```

本段代码的输出效果如下，\n 被解析成了换行，如果想要屏蔽这种现象，使用 r 即可：

```python
my_str=r'C:\number'
print(my_str)
```

输出 C:\number。

![image-20231024143701162](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024143701162.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**匹配分组**

![image-20231024151821076](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024151821076.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （1）字符串匹配

该函数用于在目标字符串开始位置去匹配正则表达式，返回 match 对象，未匹配成功返回 None，函数原型如下：

```python
re.match(pattern,string,flags=0)
```

一定要注意是目标字符串**开始位置**。

案例：匹配邮箱信息

```python
import re

pattern = r'\w+@sina\.cn'
email = '15879624465@sina.cn'
match = re.match(pattern, email)
print(match)
print(type(match))
email2 = '15879624465@qq.cn'
match2 = re.match(pattern,email2)
print(match2)
print(type(match2))
```

```xml
<re.Match object; span=(0, 19), match='15879624465@sina.cn'>
<class 're.Match'>
None
<class 'NoneType'>
```

span 指字符串跨度，（0，19）表示找到的字符串位置，0指开始位置索引，19指结束位置索引。

### （2）字符串查找

常用于数据分析、网络爬虫等数据处理中。

#### search(p,text)

该函数用于，在字符串中搜索正则表达式匹配到的**第一个位置**的值，返回 match 对象。

函数原型如下：

```python
re.search(pattern,string,flags=0)
```

search 函数的第三个参数 flags 表示正则表达式使用时的控制标记。

- re.I，re.IGNORECASE：忽略正则表达式的大小写；
- re.M，re.MULTILINE：正则表达式中的 ^ 操作符能够将给定字符串的每行当做匹配的开始；
- re.S，re.DOTALL：正则表达式中的 . 操作符能够匹配所有字符

```python
import re

pattern = r'world'
str = 'world hello world'
match = re.search(pattern, str)
print(match)
print(type(match))
```

```xml
<re.Match object; span=(0, 5), match='world'>
<class 're.Match'>
```

#### findall(p,text)

该函数用于搜索字符串，以列表格式返回**全部匹配**到的字符串，函数原型如下：

```python
re.findall(pattern,string,flags=0)
```

```python
import re

pattern = r'world'
str = 'world hello world'
match = re.findall(pattern, str)
print(match)
print(type(match))
```

```xml
['world', 'world']
<class 'list'>
```

### （3）字符串替换

####  re.sub 函数

在一个字符串中替换被正则表达式匹配到的字符串，**返回替换后的字符串**，函数原型如下：

```python
re.sub(pattern,repl,string,count=0,flags=0)
```

其中 repl 参数是替换匹配字符串的**新字符串**；count 参数是匹配的最大替换次数，默认为0（表示不限制替换数量）；string是即将被替换的旧字符串。

```python
import re

pattern = r'\d+'
str = 'AB123CD34EF5678  '
match = re.sub(pattern, ' ', str,count=2)
print(match)
print(type(match))
```

```xml
AB CD EF5678  
<class 'str'>
```

### （4）字符串分割

#### re.split 函数

该函数将一个字符串按照正则表达式匹配结果进行分割，返回一个列表。

函数原型如下：

```python
re.split(pattern, string, maxsplit=0, flags=0)
```

re.split 函数进行分割的时候，如果正则表达式匹配到的字符恰好在字符串开头或者结尾，

返回分割后的字符串列表**首尾都多了空格，需要手动去除**

```python
import re
my_str = '1梦想橡皮擦1good1good1'
pattern = r'\d'
ret = re.split(pattern, my_str)
print(ret)
```

运行结果：

```xml
['', '梦想橡皮擦', 'good', 'good', '']
```

切换为中间的内容，则能正确的分割字符串。

```python
import re
my_str = '1梦想橡皮擦1good1good1'
pattern = r'good'
ret = re.split(pattern, my_str)
print(ret)
```

如果在 **pattern 中捕获到括号**，那**括号中匹配到的结果也会在返回的列表**中。

```python
import re
my_str = '1梦想橡皮擦1good1good1'
pattern = r'(good)'
ret = re.split(pattern, my_str)
print(ret)
```

运行结果，你可以对比带括号和不带括号的区别进行学习：

**不带括号**

```xml
['1梦想橡皮擦1', '1', '1']
```

**带括号**

```xml
['1梦想橡皮擦1', 'good', '1', 'good', '1']
```

**maxsplit 参数表示最多进行分割次数， 剩下的字符全部返回到列表的最后一个元素**，例如设置匹配 1 次，得到的结果是 ['1梦想橡皮擦1', '1good1']。

```text
13.2.5 re.finditer 函数
```

搜索字符串，并返回一个匹配结果的迭代器，每个迭代元素都是 match 对象。函数原型如下：

```python
re.finditer(pattern,string,flags=0)
```

测试代码如下：

```python
import re
my_str = '1梦想橡皮擦1good1good1'
pattern = r'good'
# ret = re.split(pattern, my_str,maxsplit=1)
ret =re.finditer(pattern, my_str)
print(ret)
```

## 5、拓展阅读

[Python 常用内置模块详解 - lyshark - 博客园 (cnblogs.com)](https://www.cnblogs.com/LyShark/p/11297586.html)

[python 常用的内置模块_python内置模块-CSDN博客](https://blog.csdn.net/ruanxingzi123/article/details/82787852)

==group==

group方法返回一个或者多个匹配的子组。

如果只有一个参数，结果就是一个字符串，如果有多个参数，结果就是一个元组（每个参数对应一个项），如果没有参数，整个匹配都被返回。 

如果一个参数值为 0，即是group(0)，相应的返回值就是整个匹配字符串；如果它是一个范围 [1..99]，结果就是相应的括号组字符串。

如果一个组号是负数，或者大于样式中定义的组数，一个 **IndexError** 索引错误就 `raise`。

如果一个组包含在样式的一部分，并被匹配多次，就返回最后一个匹配。

“Python核心编程第三版”定义如下：

当处理正则表达式时，除了正则表达式对象之外，还有另一个对象类型：**匹配对象**。

匹配对象有两个主要的方法：group()和groups()。

group()要么返回整个匹配对象，要么根据要求返回特定子组。

groups()则仅返回一个包含唯一或者全部子组的元组。

如果没有子组的要求，那么当group()仍然返回整个匹配时，groups()返回一个空元组。

```shell
>>> re.match('aa','aabcdefg').group()#匹配aa group()返回匹配对象
'aa'
>>> type(re.match('aa','aabcdefg').group())#group()返回类型为字符串
<class 'str'>
>>> re.match('aa','aabcdefg').groups()#匹配aa groups()返回匹配对象为元祖，如果无子组，返回空元祖
()
>>> type(re.match('aa','aabcdefg').groups())#groups()返回类型元祖
<class 'tuple'>
>>> re.match('(aa)','aabcdefg').group()#匹配aa group()返回匹配对象 用一个()代表有一个子组
'aa'
>>> re.match('(aa)','aabcdefg').groups()#groups()返回匹配对象 所有子组（这里只有1个子组）
('aa',)
>>> re.match('(aa)\w+(cd)\w+(fg)','aabcdefg').group()#group()返回匹配对象 有3个子组
'aabcdefg'
>>> re.match('(aa)\w+(cd)\w+(fg)','aabcdefg').groups()#groups()返回匹配对象 有3个子组
('aa', 'cd', 'fg')
>>> re.match('(aa)\w+(cd)\w+(fg)','aabcdefg').group(1)#group(1)返回第1个()匹配的对象，类型为字符串
'aa'
>>> re.match('(aa)\w+(cd)\w+(fg)','aabcdefg').group(2)#group(2)返回第2个()匹配的对象
'cd'
>>> re.match('(aa)\w+(cd)\w+(fg)','aabcdefg').group(3)#group(3)返回第3个()匹配的对象
'fg'
```

# 十三、文件读写

> 本段转载于[一文搞懂Python文件读写 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/78330811)
>
> [最好懂的python文件读写(详解)-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1905786)
>
> [文本文件与二进制文件 - GGBeng - 博客园 (cnblogs.com)](https://www.cnblogs.com/xzxl/p/7508003.html)
>
> [Python——文件打开模式_python对文件的打开模式_Mood Crows的博客-CSDN博客](https://blog.csdn.net/qq_42659468/article/details/118883499)

## 1、文本文件与二进制文件

在**文本文件**的内部一字符形式存储数据，字符是有编码的，例如：GBK（简体中文）、UTF-8等；

在**二进制文件**的内部以字节形式存储数据，没有编码的概念，例如：Windows中的exe、图片（jpg、png等），以及Word、Excel和PPT等文件。

计算机文件分为两类：文本文件和二进制文件。

特别的是，**文本文件**是指以ASCII码方式(也称文本方式)存储的文件，更确切地说，英文、数字等字符存储的是ASCII码，而汉字存储的是机内码。

**文本文件**中除了存储文件有效字符信息（包括能用ASCII码字符表示的回车、换行等信息）外，不能存储其他任何信息。

文本文件是一种由若干行字符构成的[计算机文件](http://baike.baidu.com/view/6552064.htm)。文本文件存在于计算机文件系统中。通常，通过在文本文件**最后一行后放置文件结束标志来指明文件的结束**。

文本文件是指一种容器，而纯文本是指一种内容。文本文件可以包含纯文本。

大家都知道计算机的存储在物理上是二进制的，所以**文本文件与二进制文件的区别并不是物理上的，而是逻辑上的**。

这两者只是在编码层次上有差异。简单来说，文本文件是基于字符编码的文件，常见的编码有ASCII编码，UNICODE编码等等。二进制文件是基于值编码的文件，你可以根据具体应用，指定某个值是什么意思（这样一个过程，可以看作是自定义编码。

从上面可以看出文本文件基本上是定长编码的(也有非定长的编码如UTF-8)。而二进制文件可看成是变长编码的，因为是值编码嘛，多少个比特代表一个值，完全由你决定。

大家可能对BMP文件比较熟悉，就拿它举例子吧，其头部是较为固定长度的文件头信息，前2字节用来记录文件为BMP格式，接下来的8个字节用来记录文件长度，再接下来的4字节用来记录bmp文件头的长度。

 **两者的区别**

要弄明白二者的区别，需要知道**文件的读写过程**。

读文件：实际上是“磁盘→文件缓冲区→应用程序内存空间”这两个转化过程！

我们说“**文本文件和二进制文件没有区别**”，实际上针对的是第一个过程；既然没有区别，那么打开方式不同，为何显示内容就不同呢？这个区别实际上是第二个过程造成的。

文件实际上包括两部分，控制信息和内容信息。纯文本文件仅仅是没有控制格式信息罢了；实际上也是一种特殊的二进制文件。所以，我们**很难区分二者的不同，因为他们的概念上不是完全互斥的**。

我们说文本文件是特殊的二进制文件，是因为文本文件实际上的解释格式已经确定了：ASCII或者unicode编码。文本文件的一个缺点是，它的熵往往较低，也就是说，其实本可以用更小的存储空间记录这些信息。比如，文本文件中的一个数字65536，需要用5个字节来存储；但是用二进制格式，采用int存储，仅仅需要2个字节。而**二进制文件elf和bmp等，都往往有一个head，告诉你文件信息和解释方式**。

至于“文本文件可以按行操作，即一行一行的操作，而二进制就只能按字节块了”，这个说法则是完全错误的。

文本文件和二进制文件**在存储时**的区别

1. 二进制文件是把内存中的数据按其在内存中的存储形式原样输出到磁盘上存放，也就是说存放的是数据的原形式。
2. 文本文件是把数据的终端形式的二进制数据输出到磁盘上存放，也就是说存放的是数据的终端形式。

　　我们有必要把需要存储的数据分为字符数据和非字符数据两类。当你有数据要存储的时候．首先要考虑的问题并不是你要选择用二进制文件还是文本文件来进行存储，而是首先得考虑你要存储的数据是字符数据还是非字符数据．在此基础上再讨论应该选择用什么文件进行存储为好。

（1）如果要存储字符数据，无论是放在文本文件还是放在二进制文件中都和内存中的数据形式是没有区别的．同样也和终端形式没有区别。那么在存储和显示的特性上也没有任何区别，不浪费存储空间也不浪费转换时间。所以如果一个文件只存放字符数据，那么讨论该文件是用文本文件或是二进制文件是没有任何意义的。

（2）如果要存储非字符数据，则情况要复杂一些。

1. 如果您需要频繁地保存和访问数据．那么应该采用二进制文件进行存放，这样可以节省存储空间和转换时间。
2. 如果您需要频繁地向终端显示数据或从终端读人数据，那么应该采用文本文件进行存放，这样可以节省转换时间。

（3）如果要存储的数据中既有字符数据又有非字符数据那么要怎么办呢?那就要综合上述两点进行权衡以找到最佳平衡点了

==总结==：字符数据本身在内存中就经过了编码，所以无论是二进制还是文本形式都是一样的，而对于非字符数据来说，例如inti=10；如果用二进制来进行存储的话为1010，但是如果需要用文本形式来进行存储的话就必须进行格式化编码（对1和0分别编码，即形式为‘1’和‘0’分别对应的码值）。



## 2、打开文件

如果你想用python读取文件（如txt、csv等），第一步要用open函数打开文件。

open()是python的内置函数，它会**返回一个文件对象**，这个文件对象拥有read、readline、write、close等方法。

open函数有两个参数：

```python
open('file','mode',encoding=None,errors=None)
```

> 参数解释
>
> **file：**需要打开的文件路径，可以是字符串或整数；如果是字符串，则表示文件名（文件名既可以是当前目录的相对路径，也可以是绝对路径）；如果是整数，则表示一个已经打开的文件。
>
> **mode（可选）：**打开文件的模式，如只读、追加、写入等
>
> **encoding（可选）：**用来指定打开文件时的文件编码，默认是UTF-8编码，
>
> **errors（可选）：**用来指定在文本文件发生编码错误时如何处理。推荐errors参数的取值为‘ignore’，表示在遇到编码错误时忽略该错误，程序会继续执行，不会退出。

**mode常用的模式：**

- r：表示文件只能读取
- w：表示文件只能写入
- a：表示打开文件，在原有内容的基础上追加内容，在末尾写入
- w+:表示可以对文件进行读写双重操作

mode参数可以省略不填，默认为r模式

mode参数还可以指定以什么样的编码方式读写文本，默认情况下open是以文本形式打开文件的，比如上面的四种mode模式。

当你需要以字节（二进制）形式读写文件时，只需要在mode参数中追加'b'即可：

- rb：以二进制格式打开一个文件，用于只读
- wb：以二进制格式打开一个文件，用于只写
- ab：以二进制格式打开一个文件，用于追加
- wb+:以二进制格式打开一个文件，用于读写

![image-20231024221044871](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024221044871.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**常用**

![image-20231024221114055](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231024221114055.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

当我们读取某个文件，**向文件中写入某些内容(覆盖写)**，向文件中追加写入某写内容时，

最好的方式就是分别使用**r、w、a**这三种模式。

对于这三种模式，要么读，要么写，读模式就不能写，写模式就不能读。   对于r+、w+、a+这三种模式，如果你不是特别清楚python文件读写的原理，就不要轻易使用，因为会出现很多问题

- ##### r+模式：可读可写

对于这种模式，不管是读取文件中的内容，还是朝文件中写入内容。前提条件：文件存在。

**只读取文件中的内容**

使用r+模式，当只读文件的时候，可以读取到其中的内容。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'r+',encoding='utf-8')
print(f.read())
f.close()
```

```xml
天安门上太阳升
```

**朝文件中写入内容后，立即读取，会出现啥问题？**

当写入内容后，立即读取文件内容，发现什么也读取不到。这是由于当你写入内容后，文件句柄会放在写入内容的最后面，因此当你立即读取的时候，句柄会从上次内容最后的位置，朝后面读，因此读取为空。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'r+',encoding='utf-8')
f.write('新中国站起来了')
print(f.read())
f.close()
```

```xml

```

**朝文件中写入内容后，调整句柄位置后，再读取，会出现啥问题？**

当朝文件中写入内容后，调整句柄位置后，再读取文件中的内容，发现就有了内容。

这是由于我们使用了f.seek(0)方法，将句柄由内容末尾调整到了内容开头，因此就又有了内容。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'r+',encoding='utf-8')
f.write('新中国站起来了')
f.seek(0)
print(f.read())
f.close()
```

```xml
新中国站起来了
```

此时文件的内容

![image-20231025120225158](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025120225158.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- ##### w+：可读可写

**直接往文件中写入内容，之后再直接读取上述文件，看看会发生啥问题？**

使用w+模式，当我们直接朝文件中写入，毋庸置疑，肯定是可以的。

接着，我们直接读取这个文件中的内容，奇怪的现象发生了，什么都读取不到。

这是因为w+模式，在进行文件读取的时候，默认是先写再读。

但是我们确实没有写入任何东西呀？

这是由于系统默认帮我们写入了一个空值，因此把原有内容覆盖了。

所以再当我们读取文件中的内容的时候，发现读取为空。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'w+',encoding='utf-8')
f.write('新中国站起来了')
f.close()

f2 = open(f_path,'w+',encoding='utf-8')
print(f2.read())
f2.close()
```

```xml
```

**朝文件中写入内容后，立即读取，又会发生什么？**

再接着，我们朝文件中，写入内容后再立即读取，这下仍然读取不到任何内容，这又是为什么呢？

这是由于我们第一次写入“哈哈哈哈哈哈”的时候，句柄移动到了内容最后。

当我们立即读取的时候，句柄从内容最后的位置，继续朝后面读，因此啥也没有。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'w+',encoding='utf-8')
f.write('新中国站起来了')
print(f.read())
f.close()
```

```xml
```

**朝文件中写入内容后，调整句柄位置后，再读取，会发生什么？**

 最后，当朝文件中写入内容后，调整句柄位置后，再读取文件中的内容，发现就有了内容。

这是由于我们使用了f.seek(0)方法，将句柄由内容末尾调整到了内容开头，因此就又有了内容。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'w+',encoding='utf-8')
f.write('新中国站起来了')
f.seek(0)
print(f.read())
f.close()
```

```xml
新中国站起来了
```

- ##### a+：可读可写

**直接朝文件中写入内容**

使用a+模式，朝文件中写入内容，毋庸置疑，肯定是没问题的。

```python
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'a+',encoding='utf-8')
f.write('新中国站起来了')
f.close()
```

```xml
```

**直接读取文件中的内容**

接着，当我们读取上述文件中的内容，会发现什么也读取不到。

这是由于，使用r+模式打开文件，文件句柄默认放在内容的最后面，因此你直接读取其中的内容，什么也没有。

```python
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'a+',encoding='utf-8')
print(f.read())
f.close()
```

```xml
```

**调整句柄位置后，再读取文件中的内容**

最后，在读取文件中内容之前，我们使用了f.seek(0)方法，

将句柄由内容末尾调整到了内容开头，再次读取文件中的内容，发现就有了内容。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'a+',encoding='utf-8')
f.seek(0)
print(f.read())
f.close()
```

```xml
新中国站起来了
```

## 3、关闭文件

打开文件并处理完毕后，需要关闭文件，这里用到close方法。

f.close() 用来关闭文件并立即释放它使用的所有系统资源。如果你没有显式地关闭文件，Python的垃圾回收器最终将销毁该对象并为你关闭打开的文件，但这个文件可能会保持打开状态一段时间。

对文件的操作往往会抛出异常，为了保证对文件的操作无论是正常结束还是异常结束，都能关闭文件，我们应该将对close（）方法的调用放在异常处理的finally代码块中。

应该要养成使用close()的习惯。

使用方法很简单：

```python
f = open(file) # 打开文件
f.close() # 关闭文件
```



==拓展==

**在with as 代码块中关闭文件**

作用：

- 当子句体结束后文件会正确关闭，即使在某个时刻引发了异常

- 帮助自动释放资源，包括关闭文件的操作
- 可以替代finally代码块
- 优化代码结构，提高其可读性

```python
f_name = 'text.txt'
with open(f_name) as f:
    content = f.read()
    print(content)
```



## 4、读写文件

读写文本文件与读写二进制文件的主要区别：

- 在读写文本文件时，需要指定encoding，而二进制文件则不需要；
- 在调用读写方法时，文本文件操作的是字符串，而二进制文件操作的是字节。

### （1）读文件

**read()**会读取一些数据并将其作为字符串（在文本模式下）或字节对象（在二进制模式下）返回。

read方法有一个参数：

```python3
f.read(size) # f为文件对象
```

> 参数size（可选）为数字，表示从已打开文件中读取的字节计数，默认情况下为读取全部；
>
> 当size=-1时，说明对读取的字符数没有限制。

假设有一个文件sample1.txt，内容如下：

```text
This is python big data analysis!
```

现在读取该文件：

```python
with  open('sample1.txt') as f:
content = f.read()
    print(content)
    f.close()
```

输出：

![image-20231025100209094](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025100209094.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**readline方法**从文件中读取整行，包括换行符'\n'。

换行符（\n）留在字符串的末尾，如果文件不以换行符结尾，则在文件的最后一行省略，这使得返回值明确无误。

如果 f.readline() 返回一个空的字符串，则表示已经到达了文件末尾，而空行使用 '\n' 表示，该字符串只包含一个换行符。

f.readline()有一个参数：

```python3
f.readline(size)
```

参数size表示从文件读取的字节数。



假设有一个文件sample2.txt，共三行，内容如下：

```text
hello,my friends!
This is python big data analysis,
let's study.
```

我要用readline函数读取该文件：

```python3
with  open('a.txt') as f:
    print(f.readline())
    print(f.readline(5))
    f.close()
```

readline方法会记住上一个readline函数读取的位置，接着读取下一行。

所以当你需要遍历文件每一行的时候，不妨使用readline方法吧！

输出：

![image-20231025100504031](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025100504031.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**readlines方法**和readline方法长得像，但功能不一样，前面说过readline方法只读取一行，readlines方法则是读取所有行，返回的是所有行组成的列表。

readlines方法没有参数，使用更加简单。依旧以sample2.txt为例：

```python3
with  open('a.txt') as f:
    print(f.readlines())
    f.close()
```

输出：

![image-20231025100623862](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025100623862.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

#### read、readline、readlines的区别

![image-20231025143137239](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025143137239.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- read()

返回类型是 **str**

```python
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'r',encoding='utf-8')
content = f.read()
print(type(content))
print(content)
f.close()
```

```xml
<class 'str'>
关关雎鸠，在河之洲。窈窕淑女，君子好逑。
参差荇菜，左右流之。窈窕淑女，寤寐求之。
求之不得，寤寐思服。悠哉悠哉，辗转反侧。
参差荇菜，左右采之。窈窕淑女，琴瑟友之。
参差荇菜，左右芼之。窈窕淑女，钟鼓乐之。
```

- readline()

返回类型同样是 **str** 

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'r',encoding='utf-8')
for i in range(4):
    content = f.readline().strip()
    print(content)
f.close()
```

```xml
关关雎鸠，在河之洲。窈窕淑女，君子好逑。
参差荇菜，左右流之。窈窕淑女，寤寐求之。
求之不得，寤寐思服。悠哉悠哉，辗转反侧。
参差荇菜，左右采之。窈窕淑女，琴瑟友之。
```

- readlines()

返回类型是 **list**

```python
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'r',encoding='utf-8')
content = f.readlines()
print(type(content))
print(content)
f.close()
```

```xml
<class 'list'>
['关关雎鸠，在河之洲。窈窕淑女，君子好逑。\n', '参差荇菜，左右流之。窈窕淑女，寤寐求之。\n', '求之不得，寤寐思服。悠哉悠哉，辗转反侧。\n', '参差荇菜，左右采之。窈窕淑女，琴瑟友之。\n', '参差荇菜，左右芼之。窈窕淑女，钟鼓乐之。\n']
```

### （2）写文件

**write（s）方法**顾名思义，就是将字符串写入到文件里。

它只有一个参数：

```python3
f.write([str]) # f为文件对象
```

参数[str]代表要写入的字符串

使用起来也很简单，比如将下面字符串（注意里面的转行符'\n'）

```xml
'hello,my friends!\nthis is python big data analysis'
```

写入到文件sample3.txt里。

```python
with  open('sample3.txt','w') as f:
    f.write('hello,my friends!\nthis is python big data analysis')
    f.close()
```

输出：

![image-20231025100901711](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025100901711.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

****

**writelines(lines)**方法：

向文件中写入一个字符串列表，不添加分隔符，因此通常为每一行末尾都提供行分隔符。

### （3）刷新写缓冲区

**flush（）**

刷新写缓冲区，在文件没有关闭的情况下，将数据写入文件中。



## 5、文件读写流程

### （1）类比windows中手动操作txt文档，说明python中如何操作txt文件？

① windows中手动操作txt文件的步骤

- 找到word文档
- 打开word文档
- 查看(或操作)word文档中的内容
- 关闭word文档

② python操作txt文件的步骤

- 获取被打开的文件的内存对象，该内存对象又叫做“文件句柄”。
- 通过这个内存对象(文件句柄)，来对文件进行操作(读取，写入等操作)。
- 关闭文件

### （2）什么是文件的内存对象(文件句柄)？

使用python读取一个txt文件的时候，相当于把这个文件从硬盘上，读取到了内存中。

我们如果想要操作这个文件，是不是**先要获取这个文件对象**？

只有获取这个文件对象后，才能够真正的去操作这个文件，不管是读取文件中的内容，还是向文件中写入内容。 

这个“**文件句柄**”包含了文件的文件名、文件的字符集、文件的大小、文件在硬盘上的起始位置。

### （3）演示怎么读取文件

```python
f = open(r"G:\6Tipdm\file_read_write\yesterday.txt","r",encoding="utf-8")
data  = f.read()
print(data[:245])
f.close()
```

![image-20231025104935593](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025104935593.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**但是如果我们进行两次读取**

```python
f = open(r"G:\6Tipdm\file_read_write\yesterday.txt","r",encoding="utf-8")
data  = f.read()
data1 = f.read()
print(data[:245])
print("-------------------------------------")
print(data1[:245])
f.close()
```

![image-20231025105032229](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025105032229.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**问题**：我们读取了2遍内容，为什么只显示了一次读取的结果呢？

**原因**：

![image-20231025105131765](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025105131765.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

 通过上图我们可以发现，

当我们操作这个“文件句柄”的read()方法去读取文件的时候，这个句柄会从文件的开头位置1，移动到文件的结束位置2。

**如果不做任何操作，读取完毕之后，句柄就会停止在2这个位置。**

因此当我们再次读取文件的时候，该句柄是从2这个位置，往后面读取内容。

由于后面没有任何内容，因此第二次读取为空。

那么，如果我们想要第二次同样能够读取到文件中的内容，应该怎么办呢？

**解决方法**：

使用**seek（）**函数调整句柄位置。

例如：f.seek(0)，将句柄调整到文本的开头位置。

### （4）演示怎么写入文件

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'

f = open(f_path,'w',encoding='utf-8')
f.write('我爱北京天安门')
f.close()
```

![image-20231025110304440](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025110304440.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'

f = open(f_path, 'w', encoding='utf-8')
f.write('五星红旗飘啊飘')
f.write('天安门上太阳升')
f.close()
```

![image-20231025110857820](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025110857820.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



意外发生。当我们再次写入新的内容的时候，发现之前写的内容不见了，这是为啥呢？

这就是我们下面要讲述的“**文件读写的几种常见模式**”。

![image-20231025111040010](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025111040010.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 6、对于一个10G的大文件，怎么高效的查看文件中的内容呢？

当我们读取文件中的内容，相当于是把写在硬盘上的东西，读取到内存中。

不管你是使用read()或者readlines()一次性读取到到内存中，还是使用readline()一行行的将整个内容读取到内存中，如果文件很大，都将会耗用很大的内存。

同时，从硬盘读取文件内容到内存中，也会很慢。

因此，有没有一种高效的方式？

既让我们看到了文件中的内容，又不会占用内存呢？下面我们将进行说明。

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f = open(f_path,'r',encoding='utf-8')
for line in f:
    print(line.strip())
f.close()
```

```xml
关关雎鸠，在河之洲。窈窕淑女，君子好逑。
参差荇菜，左右流之。窈窕淑女，寤寐求之。
求之不得，寤寐思服。悠哉悠哉，辗转反侧。
参差荇菜，左右采之。窈窕淑女，琴瑟友之。
参差荇菜，左右芼之。窈窕淑女，钟鼓乐之。
```

 **结果说明**：

上述方式中，f相当于一个迭代器，我们使用for循环迭代f中元素。

每循环一次，就相当于读取一行到内存中，并记住这一次读取到的位置。

当进行下次迭代的时候，上一次读取到内存中的内容，就会被销毁了，当前内存中读取的就是第二行的内容。

当进行第三次循环的时候，内存中第二行的内容也会被销毁，此时内存中只会保存第三行的内容，这样依次进行下去。

直到最后一次循环，读取最后一行的内容，此时，内存中保留的也只是最后一行的内容。

迭代器有一个特性：**每次进行迭代的时候，就会记住当前读取的位置**。

**当进行下一次迭代的时候，前面的内容会被销毁掉，在内存中只会保留当前循环得到的内容**。

## 7、复制文件

### （1）复制文本文件

```python3
f_path = r'C:\Users\15879\Desktop\IO\hello.txt'
f_path2 = r'C:\Users\15879\Desktop\IO\hello2.txt'

with open(f_path,'r',encoding='utf-8') as f:
    lines = f.readlines()
    with open(f_path2,'w',encoding='utf-8') as f2:
        f2.writelines(lines)
        print('文件复制成功'
```

![image-20231025151903163](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025151903163.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （2）复制二进制文件

```python3
f_path = r'C:\Users\15879\Desktop\IO\dog.png'
f_path2 = r'C:\Users\15879\Desktop\IO\dog2.png'

with open(f_path,'rb') as f:
    b = f.read()
    with open(f_path2,'wb') as f2:
        f2.write(b)
        print('文件复制成功')
```

![image-20231025152223164](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231025152223164.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



# 十四、图形用户界面

> 本段转载于[Python大佬手把手教你利用wxPython模块编写界面程序 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/259787153)

## 1、Python中的图形用户界面开发库

> 本段转载于[python gui 中三大框架tkinter，wxpython, pyqt如何选择_python gui哪个好-CSDN博客](https://blog.csdn.net/python1212/article/details/101421435)
>
> [Tkinter vs wxPython - Python图形用户界面库的比较 - 掘金 (juejin.cn)](https://juejin.cn/post/7120087497727541262)

### Tkinter

Tkinter 模块(Tk 接口)是 **Python 的标准 Tk GUI 工具包的接口** 。

Tk 和 Tkinter 可以在大多数的 Unix 平台下使用，同样可以应用在 Windows 和 Macintosh 系统里。

Tk8.0 的后续版本可以实现本地窗口风格，并良好地运行在绝大多数平台中。

**优点**

Tkinter是最古老的GUI库之一，这使得它积累了大量的用户群，最终导致它被添加到标准Python库中。这使得它不需要任何额外的安装或下载包的好处。它也是一个非常成熟和稳定的库，所以你不可能遇到任何问题。

Tkinter的主要优点可以用一句话来概括。它**简单、快速、易学**。这三点是Tkinter受欢迎的主要原因，尽管有一些缺点，我们后面会讲到。

其他一些不太被提及的优点，但也很重要，那就是Tkinter的（事件）绑定系统和它的布局管理。绑定系统非常灵活且易于集成，允许你做一些事情，比如在鼠标悬停或按键时触发功能。

同样地，Tkinter的布局系统也非常直观，并且很容易使用三个布局管理器之一进行设置，即pack()、place()或[grid()](https://link.juejin.cn/?target=https%3A%2F%2Fcoderslegacy.com%2Fpython%2Ftkinter-grid-layout%2F)。你可能会发现Tkinter的布局和绑定系统比wxPython更加强大和容易使用。

**缺点**

如果你想要构建一个GUI界面布局，你就必须自己写代码，因为Tkinter没有提供一个图形界面设计器，我估计这也是很多人没有选择它来做软件的一个最主要原因。

毋庸置疑，它有一个非常 "经典 "的外观，在合适的人手中可以用来创建专业的应用程序。然而，它的开箱即用的外观几乎被其他所有的GUI库比下去了，如ax wxPython和PyQt。

Tkinter的另一个缺点是它的小工具。虽然它们很简单，使用起来也很直观，但它们的外观明显过时了。此外，其他库如PyQt和wxPython有更强大和先进的部件，如[PyQt的视频播放器](https://link.juejin.cn/?target=https%3A%2F%2Fcoderslegacy.com%2Fpython%2Fpyqt5-video-player-with-qmediaplayer%2F)。(Tkinter在基本部件方面与之匹配得很好，但在高级部件方面就不行了)

![image-20231026182027420](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026182027420.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

如果没有ttk子模块，Tkinter的缺点可能会说服许多人转而使用另一个GUI库。然而，ttk 通过引入主题和新的样式选项，以及许多部件的更新外观，帮助缓解了这一问题。

下面是一些默认的tkinter部件的外观。

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/TkinterDefaultLook.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

下面是同样的东西，但用ttk版本的小工具代替。

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/TkinterVistaTheme.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

正如你所看到的，较低的那个看起来更整洁，更现代。还有一些特殊的效果，比如当你把鼠标悬停在按钮上时（会给它一个蓝色的亮点），这在默认的Tkinter中是不存在的。

另外，请注意，ttk是 ***不是***一个单独的库或包，需要单独下载。它包含在tkinter库中，可以很容易地被导入。你可以在这个ttk教程系列中[了解更多关于ttk和它的部件的](https://link.juejin.cn/?target=https%3A%2F%2Fcoderslegacy.com%2Fpython%2Ftkinter-ttk-widgets-tutorial%2F)信息

### PyQt

pyqt5是一套Python绑定Digia QT5应用的框架。

它可用于Python 2和3。Qt库是最强大的GUI库之一。

Qt强大之处在于网上有很多pyqt的资源，而且qt技术已经相当成熟，pyqt是采用基本和qt一致的api，因此之前使用过qt的人，转移到pyqt很容易，这也是我们学习编程的始终强调的一点，一通百通，当你一门语言学习扎实了，学透了，那么转移到其它语言是非常容易的。

pyqt5作为Python的一个模块，它有620多个类和6000个函数和方法。这是一个跨平台的工具包，它可以运行在所有主要的操作系统，包括UNIX，Windows，Mac OS。pyqt5是双重许可。开发者可以在GPL和商业许可之间进行选择。

QT可能是最强大的，但也许它也是最复杂的。如果你要推销自己的软件，那么你需要确保你有正确理解QT许可证或准备支付一笔不小的费用。

QT给我们带来最方便的好处，就是它有一个QT Desiginer，这个设计器可以方便我们进行页面的布局，可以说在Tkinter里面需要一坨坨的代码完成的页面布局，在QT里面只要拖一拖控件就搞定了。

![image-20231026182209283](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026182209283.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### wxPython

wxPython 是一款开源软件，是 Python 语言的一套优秀的 GUI 图形库，

允许 Python 程序员很方便的创建完整的、功能健全的 GUI 用户界面。

wxPython可以说是上面两者之间的一个很好的妥协。

它是**免费的**，**源代码是开放的**，允许其应用在商业产品上，你可以免费使用它和共享它。

同时，它也提供类似QT Designer的设计器wxFormbuilder。

可以说他就是个压缩版的QT，但是该有的功能却完全不缺失。

对于wxPython，它是wxWidgets库的一个Python扩展

**优势**

wxPython的主要优势和卖点在于它有大量功能丰富的widgets，以及良好的设计和外观。这些也是它相对于Tkinter库的主要优势，Tkinter库看起来有点过时。另一个优点是，wxPython开箱即用，在所有平台上看起来都很好，而且不需要任何定制的修补。

它的学习曲线可能比Tkinter更陡峭，但一旦你掌握了它的工作原理，你就可以获得比Tkinter更多的特性和功能。

那些对更原生的windows外观感兴趣的人将会喜欢wxPython，因为它类似于原生的Windows GUI。

![wxPython vs Tkinter - Menus](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/wxPythonCheckItemsMenu.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

用Python创建强大的菜单

[菜单部件](https://link.juejin.cn/?target=https%3A%2F%2Fcoderslegacy.com%2Fwxpython-tutorial%2Fmenu-and-menubar-widget%2F)是一个很好的例子，wxPython内置了对菜单图标、键盘快捷键和方便的菜单项部件的支持，比如你在上图中看到的check-button-menu。

**劣势**

首先，我想说的是，wxPython需要单独下载（幸运的是，使用pip的过程很简单）。当你把你的应用程序分发给其他用户时，这一点可能很重要。否则，如果只是个人问题，这几乎是一个可以忽略不计的问题。

wxPython的另一个 "缺点 "是它比Tkinter慢一些，尽管这在最初加载窗口显示的时候有点难以衡量。

另一个小问题是，wxPython仍在积极开发中，不过这在某种意义上也对它有利。它还没有达到像Tkinter那样的稳定性和成熟度，但是它的积极开发有可能带来一些新的功能，这些功能可以使wxPython的天平倾向于后者。

我们已经在Tkinter部分讨论了一些Tkinter胜过wxPython的地方，所以我们不要再提这个了。然而，如果我们从中立的角度来看待wxPython，其实并没有什么明显的缺点（除了速度问题）。



### 比较Tkinter和wxPython的代码

这只是一个简单的例子，我们创建了一个链接到函数的单一按钮。

这些例子应该向你展示了在wxPython/Tkinter中设置一个窗口和一个简单的widget所需要的基本代码。

首先，我们有Tkinter。

```python3
import tkinter as tk

class Window:
    def __init__(self, master):
        self.master = master
        frame = tk.Frame(self.master)
        
        button = tk.Button(frame, text = "Close Window", command = self.quit)
        button.pack(pady = 30)

        frame.pack()

    def quit(self):
        self.master.destroy()

root = tk.Tk()
root.geometry('200x150')
window = Window(root)
root.mainloop()
```

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/Tkinter_CloseWindow.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

------

这里是wxPython的版本。

```python3
import wx
 
class Window(wx.Frame):
    def __init__(self, title):
        super().__init__(parent = None, title = title)
        panel = wx.Panel(self)
 
        closeButton = wx.Button(panel, label = "Close", pos = (50,50), size = (100,30))
        closeButton.Bind(wx.EVT_BUTTON, self.closeWindow)
 
        self.Centre() 
        self.Show()
 
    def closeWindow(self, e):
        wx.CallAfter(self.Close)
         
         
app = wx.App()
window = Window("WxPython Button Tutorial")
app.MainLoop()
```

![wxPython vs Tkinter - Code Comparision](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/wxPython_CloseWindow.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

(默认的wxPython窗口尺寸相当大，因此看起来是这样的，不要惊慌)



### 题外话

看到这里，似乎有人可能已经决定使用wxPython了，但是我想告诉你的是，存在即合理这个道理。既然这三种框架都存在，并且都依然在维护，就说明这三个框架都有人在使用，并且都有自己的受众人群，也都有自己存在的意义。

Tkinter的设计更好，更容易使用，但wxPython的功能更丰富，更强大，看起来也更漂亮。

很多人都在纠结到底应该选择哪一个，我觉得，先选择一个并深入研究下去，你才会知道哪个更适合自己，毕竟，萝卜白菜，各有所爱，他人满意的，并不一定适合你。

***只要记住，两者都是伟大的库，都是用来制作强大的GUI应用程序的。最后，更重要的是你自己在利用库的功能方面的技能。***

## 2、安装wxPython

**pip install wxPython**

pip是Python提供的包（库）管理工具，可以对第三方库进行安装、卸载等操作。

成功操作，出现如下界面：

![image-20231026191602144](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026191602144.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 3、第一个wxPython程序

用户界面的组成：窗口、窗口中的控件。

编写wxPython程序其实主要是创建窗口和添加控件的过程。

至少需要一个应用（wx.App）对象和一个窗口（wx.Frame）对象。

```python3
import wx

app = wx.App()
frm = wx.Frame(None,title='Hello World!',size=(400,300),pos=(100,100))
# None表示所在的父窗口
# size表示窗口的大小
# pos表示窗口的位置
frm.Show() # 窗口默认隐藏,需要调用Show()方法才能显示
app.MainLoop() # 让应用程序进入主事件循环中
```

![image-20231026211039153](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026211039153.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**事件循环**

事件循环是一种事件或消息分发处理**机制**，

大部分图形用户界面在界面中的显示及响应用户事件的处理都是通过**主事件循环**实现的。

**libpng**

一款用C语言编写的比较底层的读写PNG文件的库，跨平台。

在运行Python文件时会输出“libpng warning:iCCP:konwn incorrent sRGB profile”信息，

这是因为wxPython加载图片时使用了libpng工具，

如果png图片的格式比较老，

libpng工具就会发出这个警告。

## 4、自定义窗口类并添加组件

**面板放到窗口中**

**静态文本对象被放到面板中**

```python3
import wx


class MyFrame(wx.Frame):
    def __init__(self):
        super().__init__(None, title="Hello World!", size=(400, 300), pos=(100, 100))
        # 自定义窗口中的控件
        panel = wx.Panel(parent=self)
        statictext = wx.StaticText(parent=panel, label='Hello World!', pos=(10, 10))


app = wx.App()
frm = MyFrame()
frm.Show()
app.MainLoop()
```

![image-20231026211128523](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026211128523.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**使用建议：**

先将所有控件放到面板中，再将面板放到窗口中。

## 5、事件处理

**图形界面的控件要响应用户的操作，就必须添加事件处理机制**

### （1）事件源

事件发生的场所，就是各个控件，例如：按钮事件的事件源是按钮。

### （2）事件

wxPython中的事件被封装为事件类wx.Event及其子类，例如：按钮事件类是wx.CommandEvent，鼠标按钮事件类是wx.MoveEvent。

### （3）事件处理

一个响应用户事件的方法。

```python3
import wx


class MyFrame(wx.Frame):
    def __init__(self):
        super().__init__(None, title="事件处理", size=(300, 180), pos=(100, 100))
        # 自定义窗口中的控件
        panel = wx.Panel(parent=self)
        self.statictext = wx.StaticText(parent=panel, label='请点击OK按钮', pos=(110, 20))
        button = wx.Button(parent=panel,label= 'OK', pos=(100, 50))
        self.Bind(wx.EVT_BUTTON, self.on_click, button)

    def on_click(self, event):
        self.statictext.SetLabelText('Hello World!')


app = wx.App()
frm = MyFrame()
frm.Show()
app.MainLoop()
```

![image-20231026214253595](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026214253595.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**self.Bind(wx.EVT_BUTTON, self.on_click, button)**

- wx.EVT_BUTTON

事件类型，就是按钮点击事件

- self.on_click

事件处理程序，可以是自定义的函数

- button

事件源，就是按钮对象

## 6、布局管理

> 本段转载于[第6天 | 25天学会wxPython，箱子布局 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/405394448)
>
> [wxPython学习（5.布局管理）_horizontal.add-CSDN博客](https://blog.csdn.net/qq_35634418/article/details/89396733)

### （1）绝对布局

**不推荐使用**

当然，在wxPython中，大多数组件可用x、y轴坐标进行定位摆放，只是那样要费时费力，还会遇到调整窗口大小时，组件的尺寸和位置不会随之改变的问题，会遇到不同系统上，应用界面不一致的问题。

控件的位置和大小都使用了绝对数值，这些控件不会随父窗口的移动或大小变化而变化。

（1）组件的尺寸和位置不随窗口的改变而改变；

（2）不同平台上应用程序可能显示不同；

（3）字体的改变可能破坏布局；

（4）如果想改变布局，必须将之前的全部推翻。

### （2）布局管理器sizer

wxPython提供了8个布局管理器类

![image-20231026234532802](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026234532802.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

#### 1）盒子布局管理器

**wx.BoxSizer**

**box = wx.BoxSizer(orient=wx.HORIZONTAL)**：可支持横向布局和纵向布局

- orient

orient值为wx.HORIZONTAL(默认)时，水平排列，为wx.VERTICAL时，垂直排列

**box.Add(window=wx.Window, proportion=0, flag=0, border=0, userData=None)**：添加子窗口（或控件）到父窗口

- window

继承于wx.Window的组件，如Button、StaticText等

- proportion

**排列比例**，一个布局中所包含的组件的尺寸由其比例所决定，

比例为0表示在窗口尺寸变化时保持尺寸不变，

其他比例系数表示组件在该布局管理器中的尺寸占比；

可以用wx.EXPAND旗标来使得组件占据管理器分配给它的所有空间；

- flag

**对齐方式**。

可以设定wx.LEFT(左端对齐)、wx.RIGHT(右端对齐)、wx.TOP(顶部对齐)、wx.BOTTOM(底部对齐)、中心对齐(wx.ALIGN_CENTRE)等多种对齐方式，

不同方向之间可以通过竖线符号|组合；

wx.EXPAND|wx.ALL 会随着窗口变大而变化

**对齐标志**

![image-20231026220543322](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026220543322.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**边框标志**

![image-20231026220609758](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026220609758.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**调整尺寸标志**

![image-20231026220726645](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026220726645.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- border

边界，调整组件的边框的宽度(上下左右)，一般和flag参数配合使用

##### 重构事件处理

```python3
import wx


class MyFrame(wx.Frame):
    def __init__(self):
        super().__init__(None, title='事件处理', size=(300, 180))
        panel = wx.Panel(parent=self)
        self.statictext = wx.StaticText(parent=panel, label='请点击OK按钮')
        button = wx.Button(parent=panel, label='OK')
        self.Bind(wx.EVT_BUTTON, self.on_click, button)

        vbox = wx.BoxSizer(wx.VERTICAL)
        vbox.Add(self.statictext, proportion=1, flag=wx.ALIGN_CENTER_HORIZONTAL | wx.FIXED_MINSIZE | wx.TOP, border=30)
        vbox.Add(button, proportion=1, flag=wx.EXPAND | wx.BOTTOM, border=10)
        panel.SetSizer(vbox)

    def on_click(self, event):
        self.statictext.SetLabelText('Hello World!')


app = wx.App()
frame = MyFrame()
frame.Show()
app.MainLoop()
```

![image-20231026225155579](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026225155579.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

##### 盒子布局管理器嵌套

```python3
import wx


class MyFrame(wx.Frame):
    def __init__(self):
        super().__init__(None, title='布局管理嵌套', size=(300, 120))

        # 组件
        panel = wx.Panel(parent=self)
        self.statictext = wx.StaticText(parent=panel, label='请单击按钮')
        button1 = wx.Button(parent=panel, id=10, label='Button1')
        button2 = wx.Button(parent=panel, id=11, label='Button2')

        # 小盒子
        hbox = wx.BoxSizer(wx.HORIZONTAL)
        hbox.Add(button1, proportion=1, flag=wx.EXPAND | wx.ALL, border=10)
        hbox.Add(button2, proportion=1, flag=wx.EXPAND | wx.ALL, border=10)

        # 最外层大盒子
        vbox = wx.BoxSizer(wx.VERTICAL)
        vbox.Add(self.statictext, proportion=1, flag=wx.CENTER | wx.FIXED_MINSIZE | wx.TOP, border=10)
        vbox.Add(hbox, proportion=1, flag=wx.CENTER)

        # 设置面板的布局
        panel.SetSizer(vbox)

        # 绑定事件
        self.Bind(wx.EVT_BUTTON, self.on_click, id=10, id2=20)

    # 处理点击操作
    def on_click(self, event):
        id = event.GetId()
        if id == 10:
            self.statictext.SetLabelText('Button1被单击了')
        if id == 11:
            self.statictext.SetLabelText('Button2被单击了')


app = wx.App()
frame = MyFrame()
frame.Show()
app.MainLoop()
```



![image-20231026233353228](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231026233353228.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 7、控件

wxPython的所有控件都继承自wx.Control

### （1）基础控件

基础按钮Button；

图形按钮BitmapButton；

切换按钮ToggleButton（有两种状态可以切换：按下和未按下）；

静态文本框StaticText（展示一行或多行只读文本）；

文本输入框TextCtrl；

富文本输入框RichTextCtrl可以加入图像、文字色彩等效果；

带格式文本输入框StyledTextCtrl；

超链接HyperLinkCtrl；

静态位图：StaticBitmap；

静态分割线StaticLine（可垂直可水平）；

静态框StaticBox（为了装饰用，将多个组件组合在一起显示）；

下拉列表框ComboBox；

可编辑的下拉列表框Choice；

复选框CheckBox（有两个状态：勾选或未勾选）；

单选按钮RadioButton（单选按钮是从一组选项中只能选择一个，将多个单选按钮组合成一个选项组时，只需设定第一个单选按钮style为wx.RB_GROUP，后面跟着的那些单选按钮就自动跟它一组，如果想另开一组，只需再将另一组的第一个单选按钮的style设置为wx.RB_GROUP）；

进度条Gauge；

滑动条Slider；

整数数值调节钮SpinCtrl；

浮点数数值调节钮SpinCtrlDouble；

滚动条ScrollBar。

### （2）高级组件

列表框ListBox：是对一组选项的展示和交互，它有两个主要的事件，一个是wx.EVT_COMMAND_LISTBOX_SELECTED，即鼠标单击某一项时产生；另一个是wx.EVT_COMMAND_LISTBOX_DOUBLE_CLICKED，即鼠标双击某一项时产生。

列表视图ListCtrl：也是用来展示一组选项，与ListBox不同的是，ListBox仅能展示一列，而ListCtrl能展示多列。ListCtrl有三种视图模式：list、report和icon。向ListCtrl中插入数据需要使用两种方法：首先使用InsertItem()方法获得行号，然后再在当前行中使用SetItem()方法在列中插入数据。

Mixins：Mixins增强了ListCtrl的功能，它们都在wx.lib.mixins.listctrl这个模块中，一共有六种Mixins：

（1）wx.ColumnSorterMixin：使得在report视图中对列进行排序；

（2）wx.ListCtrlAutoWidthMixin：自动调整最后一列的宽度来占据剩余的空间；

（3）wx.ListCtrlSelectionManagerMix：定义了与系统无关的选择策略；

（4）wx.TextEditMixin：使得可以编辑文本；

（5）wx.CheckListCtrlMixin：给每一行增加了一个复选框；

（6）wx.ListRowHighlighter：候选行自动背景高亮。

wx.html.HtmlWindow：用来展示HTML页面。

wx.SplitterWindow：包含两个子窗口（如果使用wxFormBuilder，注意手动添加上两个panel）

另外还有比如：

树状结构TreeCtrl；

表格Grid；

搜索框SearchCtrl；

调色板ColourPickerCtrl；

字体设置器FontPickerCtrl；

文件选择器FilePickerCtrl；

文件目录选择器DirPickerCtrl；

文件树选择器GenericDirCtrl；

日期选择器DatePickerCtrl；

日历CalenderCtrl。

### （3）综合实例

> 本段参考[wxpython缩放图片 - 远洪 - 博客园 (cnblogs.com)](https://www.cnblogs.com/liyuanhong/p/12129698.html)

```python3
import wx


class MyFrame(wx.Frame):
    def __init__(self):
        super().__init__(None, title='组件综合示例', size=(600, 660), pos=(300, 50))

        self.panel = wx.Panel(parent=self)

        # 文本输入控件
        tc1 = wx.TextCtrl(self.panel)
        tc1.SetValue('haobingo')
        tc2 = wx.TextCtrl(self.panel, style=wx.TE_PASSWORD)
        tc3 = wx.TextCtrl(self.panel, style=wx.TE_MULTILINE)

        userid = wx.StaticText(self.panel, label="用户ID:")
        pwd = wx.StaticText(self.panel, label='密码:')
        content = wx.StaticText(self.panel, label='多行文本:')

        id_hbox1 = wx.BoxSizer(wx.HORIZONTAL)
        id_hbox2 = wx.BoxSizer(wx.HORIZONTAL)
        id_hbox3 = wx.BoxSizer(wx.HORIZONTAL)

        id_hbox1.Add(userid, proportion=1, flag=wx.LEFT | wx.EXPAND, border=10)
        id_hbox1.Add(tc1, proportion=4)

        id_hbox2.Add(pwd, proportion=1, flag=wx.LEFT | wx.EXPAND, border=10)
        id_hbox2.Add(tc2, proportion=4)

        id_hbox3.Add(content, proportion=1, flag=wx.LEFT | wx.EXPAND, border=10)
        id_hbox3.Add(tc3, proportion=4)

        text_vbox = wx.BoxSizer(wx.VERTICAL)
        text_vbox.Add(id_hbox1, flag=wx.EXPAND | wx.ALL, border=10)
        text_vbox.Add(id_hbox2, flag=wx.EXPAND | wx.ALL, border=10)
        text_vbox.Add(id_hbox3, flag=wx.EXPAND | wx.ALL, border=10)

        # 复选框和单选按钮
        st1 = wx.StaticText(self.panel, label='请选择你喜欢的编程语言:')
        cb1 = wx.CheckBox(self.panel, id=1, label='Python')
        cb1.SetValue(True)
        cb2 = wx.CheckBox(self.panel, id=2, label='Java')
        cb3 = wx.CheckBox(self.panel, id=3, label='C++')

        st2 = wx.StaticText(self.panel, label='选择性别:')
        r1 = wx.RadioButton(self.panel, id=4, label='男', style=wx.RB_GROUP)
        r2 = wx.RadioButton(self.panel, id=5, label='女')

        st1_hbox = wx.BoxSizer(wx.HORIZONTAL)
        st1_hbox.Add(st1, flag=wx.LEFT | wx.RIGHT, border=5)
        st1_hbox.Add(cb1)
        st1_hbox.Add(cb2)
        st1_hbox.Add(cb3)

        st2_hbox = wx.BoxSizer(wx.HORIZONTAL)
        st2_hbox.Add(st2, flag=wx.LEFT | wx.RIGHT, border=5)
        st2_hbox.Add(r1)
        st2_hbox.Add(r2)

        check_box = wx.BoxSizer(wx.VERTICAL)
        check_box.Add(st1_hbox, flag=wx.ALL, border=10)
        check_box.Add(st2_hbox, flag=wx.ALL, border=10)

        # 列表
        s1 = wx.StaticText(self.panel, label='选择你喜欢的编程语言:')
        list1 = ['Python', 'Java', 'C++']
        lb1 = wx.ListBox(self.panel, choices=list1, style=wx.LB_SINGLE)

        s2 = wx.StaticText(self.panel, label='选择你喜欢的水果:')
        list2 = ['苹果', '橘子', '香蕉']
        lb2 = wx.ListBox(self.panel, choices=list2, style=wx.LB_EXTENDED)

        s1_hbox = wx.BoxSizer(wx.HORIZONTAL)
        s1_hbox.Add(s1, proportion=1, flag=wx.LEFT | wx.RIGHT, border=5)
        s1_hbox.Add(lb1, proportion=1)

        s2_hbox = wx.BoxSizer(wx.HORIZONTAL)
        s2_hbox.Add(s2, proportion=1, flag=wx.LEFT | wx.RIGHT, border=5)
        s2_hbox.Add(lb2, proportion=1)

        list_box = wx.BoxSizer(wx.VERTICAL)
        list_box.Add(s1_hbox, flag=wx.ALL | wx.EXPAND, border=5)
        list_box.Add(s2_hbox, flag=wx.ALL | wx.EXPAND, border=5)

        # 静态图片控件
        p1 = wx.Image('./images/p1.jpg').Scale(300, 300)
        p2 = wx.Image('./images/p2.jpg').Scale(300, 300)
        p3 = wx.Image('./images/p3.png').Scale(300, 300)

        self.bmps = [wx.Bitmap(p1, wx.BITMAP_SCREEN_DEPTH),
                     wx.Bitmap(p2, wx.BITMAP_SCREEN_DEPTH),
                     wx.Bitmap(p3, wx.BITMAP_SCREEN_DEPTH)]

        b1 = wx.Button(self.panel, id=8, label='切换p1')
        b2 = wx.Button(self.panel, id=9, label='切换p2')
        b3 = wx.Button(self.panel, id=10, label='切换p3')
        self.Bind(wx.EVT_BUTTON, self.on_pic_click, id=8, id2=10)
        self.image = wx.StaticBitmap(self.panel, bitmap=self.bmps[0])

        button_vbox = wx.BoxSizer(wx.VERTICAL)
        button_vbox.Add(b1, proportion=1, flag=wx.EXPAND)
        button_vbox.Add(b2, proportion=1, flag=wx.EXPAND)
        button_vbox.Add(b3, proportion=1, flag=wx.EXPAND)

        pic_hbox = wx.BoxSizer(wx.HORIZONTAL)
        pic_hbox.Add(button_vbox, proportion=1, flag=wx.ALIGN_CENTER)
        pic_hbox.Add(self.image, proportion=3, flag=wx.EXPAND)

        # 最外层大盒子
        vbox = wx.BoxSizer(wx.VERTICAL)
        vbox.Add(text_vbox, flag=wx.CENTER)
        vbox.Add(check_box, flag=wx.CENTER)
        vbox.Add(list_box, flag=wx.CENTER)
        vbox.Add(pic_hbox, flag=wx.CENTER)

        # 面板的布局
        self.panel.SetSizer(vbox)

    # 处理绑定事件
    def on_pic_click(self, event):
        id = event.GetId()
        if id == 8:
            self.image.SetBitmap(self.bmps[0])
        if id == 9:
            self.image.SetBitmap(self.bmps[1])
        if id == 10:
            self.image.SetBitmap(self.bmps[2])
        self.panel.Layout()


# 初始化
app = wx.App()
frame = MyFrame()
frame.Show()
app.MainLoop()
```

![image-20231027204249773](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231027204249773.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



# 十五、网络通信

## 1、基本的网络知识

### （1）TCP/IP

> 参考文章
>
> [太棒了！TCP/IP协议 （图解+秒懂+史上最全）_图解tcpip_退休的汤姆的博客-CSDN博客](https://blog.csdn.net/stone_tmp/article/details/118386484)
>
> [TCP/IP协议详解 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/33889997)

### （2）IP地址

> 参考文章
>
> [一文详解IP地址：含义、作用、格式、分类等 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/498255136)
>
> [IP 基础知识全家桶，45 张图一套带走 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/138235610)

### （3）端口

> 参考文章
>
> [深入理解什么是端口(port) - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/225777212)
>
> [计算机端口的安全知识大全，整的明明白白！-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1406267)

### （4）HTTP/HTTPS

> 参考文章
>
> [十分钟搞懂HTTP和HTTPS协议？ (zhihu.com)](https://www.zhihu.com/tardis/zm/art/72616216?source_id=1005)
>
> [HTTP/HTTPS详解（最全） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/616202212)



## 2、Python爬虫

> 本段参考于[urllib库的使用（一篇就够了）-CSDN博客](https://blog.csdn.net/m0_43404934/article/details/122330996)
>
> [浅谈Python两大爬虫库——urllib库和requests库区别-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1826626)
>
> [urllib.request详细介绍-CSDN博客](https://blog.csdn.net/qq_43546676/article/details/88777227)
>
> [Python爬虫入门：urllib.request.Request详解-CSDN博客](https://blog.csdn.net/qq_36365528/article/details/96751748)

### （1）urllib库

通常爬取网页，在构造http请求的时候，都需要加上一些额外信息，什么Useragent，cookie等之类的信息，或者添加代理[服务器](https://cloud.tencent.com/act/pro/promotion-cvm?from_column=20065&from=20065)。往往这些都是一些必要的反爬机制。

urllib库的response对象是先创建http，request对象，装载到reques.urlopen里完成http请求。

返回的是http，response对象，实际上是html属性。使用.read().decode()解码后转化成了str字符串类型，decode解码后中文字符能够显示出来。

Python2中，有urllib和urllib2两个库来实现请求的发送，而在Python3中，统一为了urllib，其官方文档链接为：https://docs.python.org/3/library/urllib.html。urllib是Python内置的HTTP请求库，它包含4个模块。

#### 1）request模块

最基本的HTTP请求模块，可以用来**模拟发送请求**。

urllib的request模块提供了最基本的构造HTTP请求的方法，

使用它可以方便地实现请求的发送并得到响应，

同时它还带有处理授权验证（authentication）、重定向（redirection）、浏览器Cookies以及其他内容。

- **urlopen( )**

使用urlopen( )函数可以**发送一个请求**，urlopen( )函数的完整参数列表如下：

```python3
urllib.request.urlopen(url,data=None,[timeout,]*,cafile=None,capath=None,cadefault=False,context=None)
```

用法可参考官方文档https://docs.python.org/3/library/urllib.request.html。

1）使用urlopen( )方法爬取网页源代码，url参数用于指定要请求的URL路径（未指定data参数时，**默认使用GET请求方法**）

```python
#导入request模块
import urllib.request
#发出请求并返回响应
response = urllib.request.urlopen("https://www.python.org")
#打印响应返回的内容
print(response.read())
```

 **urlopen( )函数返回的是一个HTTPResponse对象**，

它包含了read( )、readinto( )、getheader(name)、getheaders( )、fileno( )等方法， 

以及msg、version、status、reason、debuglevel、closed等属性。

```python
#导入request模块
import urllib.request
#发出请求并得到响应
response = urllib.request.urlopen("https://www.python.org")
#查看响应的类型
print(type(response))
#打印响应状态码
print(response.status)
#打印请求头
print(response.getheaders())
#打印请求头中Server属性的值（表示服务端使用Web服务器是什么软件，如Tomcat、Nginx等）
print(response.getheader("Server"))
```

```python3
<class 'http.client.HTTPResponse'>
200
[('Connection', 'close'), ('Content-Length', '50392'), ('Report-To', '{"group":"heroku-nel","max_age":3600,"endpoints":[{"url":"https://nel.heroku.com/reports?ts=1698459881&sid=67ff5de4-ad2b-4112-9289-cf96be89efed&s=jTW9gdoO1mL2zidTLIDqBY57vPLljYtSErUeVI6iMt0%3D"}]}'), ('Reporting-Endpoints', 'heroku-nel=https://nel.heroku.com/reports?ts=1698459881&sid=67ff5de4-ad2b-4112-9289-cf96be89efed&s=jTW9gdoO1mL2zidTLIDqBY57vPLljYtSErUeVI6iMt0%3D'), ('Nel', '{"report_to":"heroku-nel","max_age":3600,"success_fraction":0.005,"failure_fraction":0.05,"response_headers":["Via"]}'), ('Server', 'nginx'), ('Content-Type', 'text/html; charset=utf-8'), ('X-Frame-Options', 'SAMEORIGIN'), ('Via', '1.1 vegur, 1.1 varnish, 1.1 varnish'), ('Accept-Ranges', 'bytes'), ('Date', 'Sat, 28 Oct 2023 03:15:25 GMT'), ('Age', '2725'), ('X-Served-By', 'cache-iad-kiad7000025-IAD, cache-cgh11149-CGH'), ('X-Cache', 'HIT, HIT'), ('X-Cache-Hits', '123, 2'), ('X-Timer', 'S1698462926.635599,VS0,VE0'), ('Vary', 'Cookie'), ('Strict-Transport-Security', 'max-age=63072000; includeSubDomains; preload')]
nginx
```

2）data参数可以设置请求要传递的参数，使用时需要使用bytes( )方法将**参数转化为字节流编码格式**的内容，即bytes类型；并且如果**使用了data参数**，则请求方法就不再是GET方法了，而是**POST方法**。

```python
import urllib.parse
import urllib.request
data = bytes(urllib.parse.urlencode({'word':'hello'}),encoding='utf-8')
response = urllib.request.urlopen('http://httpbin.org/post',data=data)
print(response.read())
```

 这里传递了一个参数word，值是hello。它需要被转码成bytes（字节流）类型。其中转字节流采用了bytes( )方法，该方法的第一个参 数是字符串类型，**需要用urllib.parse模块里的urlencode( )方法将字典参数转换为字符串**，bytes( )方法第二个参数指定编码格式。执行后， 通过观察返回的响应头里的Content-Type字段的值可以知道使用的是POST请求方法。

4）timeout参数可以设置超时时间，单位为秒，如果请求超过了设置的超时时间还没有得到响应，就会抛出异常。如果不指定timeout参 数，就会使用全局默认时间。它支持HTTP、HTTPS、FTP请求。

```python
import urllib.request
#向百度发出请求，如果5秒内还没有得到响应，则抛出异常
response = urllib.request.urlopen('https://www.baidu.com',timeout=5)
print(response.read())
```

 可以通过设置这个超时时间来控制一个网页在长时间未响应时，就跳过它的抓取。这可以利用try except语句实现，如下：

```python
import socket
import urllib.request
import urllib.error
try:
	response = urllib.request.urlopen('http://www.baidu.com',timeout=0.01)
except urllib.error.URLError as e:
	print(e.reason)
	print(socket.timeout)
	if isinstance(e.reason,socket.timeout):
		print('Time Out')
```

5）除了url、data、timeout这些参数外，还有context参数，它必须是ssl.SSLContext类型，用来制定SSL设置。此外，cafile和capath这两 个参数分别指定CA证书的和它的路径，这个在请求HTTPS链接时会有用，cadefault参数已经启用了，其默认值为false。

-  **Request**

使用urlopen( )方法可以**实现最基本请求的发起**，但不足以构建一个完整的请求。如果请求中需要加Headers等信息，则需要使用Request类来构建。它的构造方法如下：

```python3
class urllib.request.Request(url,data=None,headers{},origin_req_host=None,unverifiable=False,method=None)
```

**url是必选参数**，其余都是可选参数。

- url：请求的URL。。

- data：请求的参数。必须传bytes（字节流）类型的，如果是字典，可以先用urllib.parse模块里的urlencode( )编码。

- headers：请求头。它是一个字典类型的数据。可以在构造Request对象时通过headers参数直接构造，也可以由Request对象调用add_header( )方法添加。添加请求头最常用的就是通过修改User-Agent来伪装浏览器，默认的User-Agent是Python-urllib，比如伪装火狐浏览器，可以将请求头中的User-Agent字段值设置为：

  Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:95.0) Gecko/20100101 Firefox/95.0

  可以去某个浏览器发送请求然后查看请求中的User-Agent字段的值。

- origin_req_host：请求方的host名称或者IP地址。

- unverifiable：该请求是否是无法验证的，默认为False，意思是说用户没有足够权限来选择接收这个请求的结果。例如，请求一个HTML文档中的图片，但是没有自动抓取图像的权限，这时unverifiable的值就是True。

- method：请求使用的方法，类型是一个字符串，比如GET、POST。

通过Request类，一方面我们可以**将请求独立成一个对象**，另一方面可以更加丰富和灵活地配置参数。

1）基本使用

```python
import urllib.request
#调用Request()方法返回一个Request类型对象
request = urllib.request.Request('https://python.org')
#使用urlopen发送请求时将Request类型对象传进去
response = urllib.request.urlopen(request)
print(response.read().decode('utf-8'))
123456
```

 它依旧是使用urlopen( )方法发送请求，只不过这次该方法的参数**不再是URL**，而是**一个Request类型的对象。**

```python3
Open the URL url, which can be either a string or a Request object.
```

2）设置请求头、请求参数。

```python
from urllib import request,parse
url = 'http://httpbin.org/post'
#请求头
headers = {
	'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:95.0) Gecko/20100101 Firefox/95.0',
	'Host':'httpbin.org'
}
param = {
	'name':'Germey'
}
data = bytes(parse.urlencode(param),encoding='utf-8')
req = request.Request(url=url,data=data,headers=headers,method='POST')
'''
也可以通过add_header()方法逐个添加请求头
req.add_header('User-Agent','Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:95.0) Gecko/20100101 Firefox/95.0')
'''
response = request.urlopen(req)
print(response.read().decode('utf-8'))
```

```json
{
  "args": {}, 
  "data": "", 
  "files": {}, 
  "form": {
    "name": "Germey"
  }, 
  "headers": {
    "Accept-Encoding": "identity", 
    "Content-Length": "11", 
    "Content-Type": "application/x-www-form-urlencoded", 
    "Host": "httpbin.org", 
    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:95.0) Gecko/20100101 Firefox/95.0", 
    "X-Amzn-Trace-Id": "Root=1-653cade1-07d4a5225ccda80110169b6b"
  }, 
  "json": null, 
  "origin": "38.60.209.41", 
  "url": "http://httpbin.org/post"
}
```

- **Handler、Opener**

实现验证、代理设置、Cookies处理等功能需要使用Handler和Opener。

可以将Handler理解为各种处理器，有专门处理登录验证的，有处理Cookie的，有处理代理设置的，利用它们，几乎可以做到HTTP请求中所有的事情。

urllib.request模块里的BaseHandler类，是其他所有Handler的父类，提供了最基本的方法，例如default_open( )、protocol_request( )等。

它的常用子类有：

- HTTPDefaultErrorHandler：用于处理HTTP响应错误，错误都会抛出HTTPError类型的异常。
- HTTPRedirectHandler：用于处理重定向。
- HTTPCookieProcessor：用于处理Cookies。
- ProxyHandler：用于设置代理，默认代理为空。
- HTTPPasswordMgr：用于管理密码，它维护了用户名和密码的表。
- HTTPBasicAuthHandler：用于管理认证，如果一个链接打开时需要认证，那么可以用它来解决认证问题。

更多的Handler类可参考官方文档：https://docs.python.org/3/library/urllib.request.html#urllib.request.BaseHandler。

Handler需要和Opener（Opener对应的类为OpenerDirector）组合使用，

通过Handler对象可以构建Opener对象，Opener对象可以调用open( )方法，open( )方法的返回类型和urlopen( )是一样的。

1）**验证**。有些网站在打开时就会弹出提示框，直接提示你输入用户名和密码，验证成功后才能查看页面，比如Tomcat管理页：

![image-20231028144915421](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231028144915421.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

请求这样带有验证的页面时，可以借助HTTPBasicAuthhandler完成，代码如下：

```python
from urllib.request import HTTPPasswordMgrWithDefaultRealm,HTTPBasicAuthHandler,build_opener
from urllib.error import URLError
username = 'admin'
password = '123456'
#tomcat服务器管理页
url = 'http://localhost:8080/manager/html'
p = HTTPPasswordMgrWithDefaultRealm();
p.add_password(None,url,username,password)
auth_handler = HTTPBasicAuthHandler(p)
opener = build_opener(auth_handler)
try:
	result = opener.open(url)
	html = result.read().decode('utf-8')
	print(html)
except URLError as e:
	print(e.reason)
```

 该案例中，如果验证成功，则打印tomcat管理页的源代码。

2）**实现代理**。在做爬虫的时候，免不了要使用代理，如果要添加代理，可以使用ProxyHandler，其参数是一个字典，字典中键名协议类 型（比如HTTP或者HTTPS等），键值是代理连接，可以添加多个代理。

```python
from urllib.error import URLError
from urllib.request import ProxyHandler,build_opener
#为了方便测试，在本地搭建了一个代理，运行在9743端口上
proxy_handler = ProxyHandler({
	'http':'http://127.0.0.1:9743',
	'http':'https://127.0.0.1:9743'
})
opener = build_opener(proxy_handler)
try:
	response = opener.open('https://www.baidu.com')
	print(response.read().decode('utf-8'))
except URLError as e:
	print(e.reason)
```

3）**获取网站的Cookie**。首先，必须声明一个CookieJar对象，然后利用HTTPCookieProcessor来构建一个Handler，最后利用 build_opener( )方法构建Opener，执行open( )方法即可。

```python
import urllib.request,http.cookiejar

cookie = http.cookiejar.CookieJar()
handler = urllib.request.HTTPCookieProcessor(cookie)
opener = urllib.request.build_opener(handler)
response = opener.open('http://www.baidu.com')
#遍历cookies
for item in cookie:
	print(item.name+"="+item.value)
```

4）**获取网站的Cookie并保存为文件**。

```python
import urllib.request,http.cookiejar

filename = 'cookies.txt'
cookie = http.cookiejar.MozillaCookieJar(filename)
handler = urllib.request.HTTPCookieProcessor(cookie)
opener = urllib.request.build_opener(handler)
response = opener.open('http://www.baidu.com')
cookie.save(ignore_discard=True,ignore_expires=True)
```

 这里将CookieJar换成了MozillaCookieJar，它在生成文件时会用到，是CookieJar的子类，可以用来处理Cookies和文件相关的事件， 比如读取和保存Cookies，本例中将Cookies保存成了Mozilla型浏览器的Cookies格式，运行之后当前目录下生成了一个cookies.txt文 件，内容如下：

![image-20231028145357257](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231028145357257.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

另外，LWPCookieJar也可以读取和保存Cookies，但是保存的格式和MozillaCookieJar不一样，它会保存为libwww-perl（LWP）格式 的Cookies文件。要保存成LWP格式的Cookie文件，可以在声明时使用LWPCookieJar

```python
cookie = http.cookiejar.LWPCookieJar(filename)
```

 此时生成的Cookies文件中的格式如下：

```python
#LWP-Cookies-2.0
Set-Cookie3: BAIDUID="9627B6EED697A23FD61384D21DE5EEAD:FG=1"; path="/"; domain=".baidu.com"; path_spec; domain_dot; expires="2024-10-27 06:54:41Z"; comment=bd; version=0
Set-Cookie3: BIDUPSID=9627B6EED697A23F3918AFE5BA7E48B7; path="/"; domain=".baidu.com"; path_spec; domain_dot; expires="2091-11-15 10:08:48Z"; version=0
Set-Cookie3: PSTM=1698476080; path="/"; domain=".baidu.com"; path_spec; domain_dot; expires="2091-11-15 10:08:48Z"; version=0
```

5）生成Cookies文件后，后续过程中会读取Cookies文件并进行利用。以LWPCookieJar格式的Cookie文件为例

```python
import urllib.request,http.cookiejar

cookie = http.cookiejar.LWPCookieJar()
#加载Cookies文件
cookie.load('cookies.txt',ignore_discard=True,ignore_expires=True)
handler = urllib.request.HTTPCookieProcessor(cookie)
opener = urllib.request.build_opener(handler)
response = opener.open('http://www.baidu.com')
#运行正常的话，会输出百度网页的源代码
print(response.read().decode('utf-8'))
```

以上是urllib库中request模块的基本用法，想实现更多的功能，可以参考官方文档：https://docs.python.org/3/library/urllib.request.html

#### 2）error模块

异常处理模块，如果出现请求错误，可以捕获异常，然后进行重试或其他操作。

urllib库中的error模块定义了由request模块产生的异常，使用request模块发送请求时，如果出现错误，便会抛出error模块中定义的异常。

#### 3）parse模块

工具模块，提供了许多URL处理方法，如拆分、解析、合并等。

#### 4）robotparser模块

主要用于识别网站的rebots.txt文件，然后判断哪些网站可以爬，哪些网站不可以爬。

#### ==拓展阅读==

一、**使用urllib**

在Python2版本中，有urllib和urlib2两个库可以用来实现request的发送。

而在Python3中，已经不存在urllib2这个库了，统一为urllib。Python3 urllib库官方链接：https://docs.python.org/3/library/urllib.html

urllib中包括了四个模块，包括：`urllib.request`, `urllib.error`, `urllib.parse`, `urllib.robotparser`

urllib.request可以用来发送request和获取request的结果

urllib.error包含了urllib.request产生的异常

urllib.parse用来解析和处理URL

urllib.robotparse用来解析页面的robots.txt文件

可见其中模拟请求使用的最主要的库便是urllib.request，异常处理用urllib.error库。

下面会对它们一一进行详细的介绍

二、**使用urllib.request发送请求**

urllib.request.urlopen()基本使用

urllib.request 模块提供了最基本的构造 HTTP 请求的方法，利用它可以模拟浏览器的一个请求发起过程，同时它还带有处理 authenticaton （授权验证）， redirections （重定向)， cookies (浏览器Cookies）以及其它内容。

好，那么首先我们来感受一下它的强大之处，我们百度为例，我们来把这个网页抓下来。

```python
import urllib.request
 
response = urllib.request.urlopen("https://www.baidu.com")
print(response.read().decode("utf-8"))
```

真正的代码只有两行，我们便完成了百度的抓取，输出了网页的源代码，得到了源代码之后呢？你想要的链接、图片地址、文本信息不就都可以提取出来了吗？接下来我们看下它返回的到底是什么，利用 type 函数输出 response 的类型。

```python
import urllib.request
response = urllib.request.urlopen("https://www.baidu.com")
print(type(response))
```

> 输出：`<class 'http.client.HTTPResponse'>`

通过输出结果可以发现它是一个 HTTPResposne 类型的对象，它主要包含的方法有 read() 、 readinto() 、getheader(name) 、 getheaders() 、 fileno() 等函数和 msg 、 version 、 status 、 reason 、 debuglevel 、 closed 等属性。 

得到这个对象之后，赋值为 response ，然后就可以用 response 调用这些方法和属性，得到返回结果的一系列信息。

例如 response.read() 就可以得到返回的网页内容， response.status 就可以得到返回结果的状态码，如200代表请求成功，404代表网页未找到等。

下面再来一个实例感受一下：

```python
>>> import urllib.request
>>> response = urllib.request.urlopen("https://www.baidu.com")
>>> print(response.status)
200
>>> print(response.getheaders())
[('Accept-Ranges', 'bytes'), ('Cache-Control', 'no-cache'), ('Content-Length', '227'), ('Content-Type', 'text/html'), ('Date', 'Tue, 25 Jul 2017 06:36:40 GMT'), ('Last-Modified', 'Wed, 28 Jun 2017 02:16:00 GMT'), ('P3p', 'CP=" OTI DSP COR IVA OUR IND COM "'), ('Pragma', 'no-cache'), ('Server', 'BWS/1.1'), ('Set-Cookie', 'BD_NOT_HTTPS=1; path=/; Max-Age=300'), ('Set-Cookie', 'BIDUPSID=BEF13521D9F33BE4108EA36C07303743; expires=Thu, 31-Dec-37 23:55:55 GMT; max-age=2147483647; path=/; domain=.baidu.com'), ('Set-Cookie', 'PSTM=1500964600; expires=Thu, 31-Dec-37 23:55:55 GMT; max-age=2147483647; path=/; domain=.baidu.com'), ('Strict-Transport-Security', 'max-age=0'), ('X-Ua-Compatible', 'IE=Edge,chrome=1'), ('Connection', 'close')]
>>> print(response.getheader("Server"))
BWS/1.1
```

可见，三个输出分别输出了响应的状态码，响应的头信息，以及通过传递一个参数获取了 Server 的类型。

三、**urllib.request.urlopen()详解**

利用以上最基本的 urlopen() 方法，我们可以完成最基本的简单网页的 GET 请求抓取。
如果我们想给链接传递一些参数该怎么实现呢？我们首先看一下 urlopen() 函数的API。

```python
urllib.request.urlopen(url, data=None, [timeout, ]*, cafile=None, capath=None, cadefault=False, context=None)
1
```

可以发现除了第一个参数可以传递URL之外，我们还可以传递其它的内容，比如 data （附加参数）， timeout （超时时间）等等。

data 参数是可选的，如果要添加 data ，它要是字节流编码格式的内容，即 bytes 类型，通过 bytes() 函数可以进行转化，另外如果你传递了这个 data 参数，它的请求方式就不再是 GET 方式请求，而是 POST 。

```python
# coding=utf-8
import urllib.parse
import urllib.request
data = bytes(urllib.parse.urlencode({'word': 'hello'}), encoding=
'utf8')
response = urllib.request.urlopen('http://httpbin.org/post', dat
a=data)
print(response.read())
```

在这里我们传递了一个参数 word ，值是 hello 。它需要被转码成 bytes （字节流）类型。其中转字节流采用了 bytes() 方法，第一个参数需要是 str (字符串)类型，需要用 urllib.parse.urlencode() 方法来将参数字典转化为字符串。第二个参数指定编码格式，在这里指定为 utf8 。

提交的网址是 httpbin.org ，它可以提供 HTTP 请求测试。 http://httpbin.org/post 这个地址可以用来测试 POST 请求，它可以输出请求和响应信息，其中就包含我们传递的 data 参数。
运行结果如下：

```python
{
"args": {},
"data": "",
"files": {},
"form": {
"word": "hello"
},
"headers": {
"Accept-Encoding": "identity",
"Content-Length": "10",
"Content-Type": "application/x-www-form-urlencoded",
"Host": "httpbin.org",
"User-Agent": "Python-urllib/3.5"
},
"json": null,
"origin": "123.124.23.253",
"url": "http://httpbin.org/post"
}
```

我们传递的参数出现在了 form 中，这表明是模拟了表单提交的方式，以 POST 方式传输数据。

timeout参数

imeout 参数可以设置超时时间，单位为秒，意思就是如果请求超出了设置的这个时间还没有得到响应，就会抛出异常，如果不指定，就会使用全局默认时间。它支持 HTTP 、 HTTPS 、 FTP 请求。
下面来用一个实例感受一下：

```python
>>> import urllib.request
>>> response = urllib.request.urlopen("http://httpbin.org/get",timeout=1)
>>> print(response.read())
```

结果如下：

```python
During handling of the above exception, another exception occurr
ed:
Traceback (most recent call last): File "/var/py/python/urllibte
st.py", line 4, in <module> response = urllib.request.urlopen('h
ttp://httpbin.org/get', timeout=1)
...
urllib.error.URLError: <urlopen error timed out>
```

在这里我们设置了超时时间是1秒，程序1秒过后服务器依然没有响应，于是抛出了 urllib.error.URLError 异常，错误原因是 timed out 。

因此我们可以通过设置这个超时时间来控制一个网页如果长时间未响应就跳过它的抓取，利用 try,except 语句就可以实现这样的操作。

```python
import urllib.request
import  socket
import urllib.error
try:
    response = urllib.request.urlopen('http://httpbin.org/get',timeout=0.1)
except urllib.error.URLError as e:
    if  isinstance(e.reason, socket.timeout):
            print("Time out!")
```

在这里我们请求了 http://httpbin.org/get 这个测试链接，设置了超时时间是0.1秒，然后捕获了 urllib.error.URLError 这个异常，然后判断异常原因是超时异常，就得出它确实是因为超时而报错，打印输出了 TIME OUT ，当然你也可以在这里做其他的处理。

运行结果如下：

```python
Time out!
```

常理来说，0.1秒内基本不可能得到服务器响应，因此输出了 TIME OUT 的提示。这样，我们可以通过设置 timeout 这个参数来实现超时处理，有时还是很有用的。

其他参数

还有 context 参数，它必须是 ssl.SSLContext 类型，用来指定 SSL 设置。cafile 和 capath 两个参数是指定CA证书和它的路径，这个在请求 HTTPS 链接时会有用。

cadefault 参数现在已经弃用了，默认为 False 。

以上讲解了 url.request.urlopen() 方法的用法，通过这个最基本的函数可以完成简单的请求和网页抓取，如需详细了解，可以参见官方文档。https://docs.python.org/3/library/urllib.request.html

四、**urllib.request.Request的使用**

由上我们知道利用 urlopen() 方法可以实现最基本的请求发起，但这几个简单的参数并不足以构建一个完整的请求，如果请求中需要加入 headers 等信息，我们就可以利用更强大的 Request 类来构建一个请求。

首先我们用一个实例来感受一下 Request 的用法:

```python
import urllib.request
 
request =urllib.request.Request("https://www.baidu.com")
response = urllib.request.urlopen(request)
print(response.read().decode("utf-8"))
```

可以发现，我们依然是用 urlopen() 方法来发送这个请求，只不过这次 urlopen() 方法的参数不再是一个URL，而是一个 Request ，通过构造这个这个数据结构，一方面我们可以将请求独立成一个对象，另一方面可配置参数更加
丰富和灵活。

下面我们看一下 Request 都可以通过怎样的参数来构造，它的构造方法如下。

```python
class urllib.request.Request(url, data=None, headers={}, origin_req_host=None, unverifiable=False, method=None)
```

第一个参数是请求链接，这个是必传参数，其他的都是可选参数。

data 参数如果要传必须传 bytes （字节流）类型的，如果是一个字典，可以先用 urllib.parse.urlencode() 编码。

headers 参数是一个字典，你可以在构造 Request 时通过 headers 参数传递，也可以通过调用 Request 对象的 add_header() 方法来添加请求头。请求头最常用的用法就是通过修改 User-Agent 来伪装浏览器，默认的 User-
Agent 是 Python-urllib ，你可以通过修改它来伪装浏览器，比如要伪装火狐浏览器，你可以把它设置为 Mozilla/5.0 (X11; U; Linux i686)Gecko/20071127 Firefox/2.0.0.11

origin_req_host 指的是请求方的 host 名称或者 IP 地址。

unverifiable 指的是这个请求是否是无法验证的，默认是 False 。意思就是说用户没有足够权限来选择接收这个请求的结果。例如我们请求一个HTML文档中的图片，但是我们没有自动抓取图像的权限，这时 unverifiable 的值就是 True 。

method 是一个字符串，它用来指示请求使用的方法，比如 GET ， POST ， PUT 等等。
下面我们传入多个参数构建一个 Request 来感受一下：

```python
from urllib import request,parse
url = "http://httpbin.org/post"
headers = {
    #伪装一个火狐浏览器
    "User-Agent":'Mozilla/4.0 (compatible; MSIE 5.5; Windows NT)',
    "host":'httpbin.org'
}
dict = {
    "name":"Germey"
}
data = bytes(parse.urlencode(dict),encoding="utf8")
req = request.Request(url=url,data=data,headers=headers,method="POST")
response = request.urlopen(req)
print(response.read().decode("utf-8"))
```

在这里我们通过四个参数构造了一个 Request ， url 即请求链接，在 headers 中指定了 User-Agent 和 Host ，传递的参数 data 用了 urlencode() 和 bytes() 方法来转成字节流，另外指定了请求方式为 POST 。

运行结果如下：

```python
{
  "args": {}, 
  "data": "", 
  "files": {}, 
  "form": {
    "name": "Germey"
  }, 
  "headers": {
    "Accept-Encoding": "identity", 
    "Connection": "close", 
    "Content-Length": "11", 
    "Content-Type": "application/x-www-form-urlencoded", 
    "Host": "httpbin.org", 
    "User-Agent": "Mozilla/4.0 (compatible; MSIE 5.5; Windows NT)"
  }, 
  "json": null, 
  "origin": "1.85.221.5", 
  "url": "http://httpbin.org/post"
}
```

通过观察结果可以发现，我们成功设置了 data ， headers 以及 method 。

另外 headers 也可以用 add_header() 方法来添加。

req = request.Request(url=url, data=data, method=‘POST’)
req.add_header(‘User-Agent’, ‘Mozilla/4.0 (compatible; MSIE 5.5;Windows NT)’)

如此一来，我们就可以更加方便地构造一个 Request ，实现请求的发送。

五、**urllib.request高级特性**

大家有没有发现，在上面的过程中，我们虽然可以构造 Request ，但是一些更高级的操作，比如 Cookies 处理，代理该怎样来设置？
接下来就需要更强大的工具 Handler 登场了。

简而言之你可以把它理解为各种处理器，有专门处理登录验证的，有处理 Cookies 的，有处理代理设置的，利用它们我们几乎可以做到任何 HTTP 请求中所有的事情。

首先介绍下 urllib.request.BaseHandler ，它是所有其他 Handler 的父类，它提供了最基本的 Handler 的方法，例
如 default_open() 、 protocol_request() 等。
接下来就有各种 Handler 类继承这个 BaseHandler ，列举如下：

- HTTPDefaultErrorHandler 用于处理HTTP响应错误，错误都会抛出 HTTPError 类型的异常。
- HTTPRedirectHandler 用于处理重定向。
- HTTPCookieProcessor 用于处理 Cookie 。
- ProxyHandler 用于设置代理，默认代理为空。
- HTTPPasswordMgr 用于管理密码，它维护了用户名密码的表。
- HTTPBasicAuthHandler 用于管理认证，如果一个链接打开时需要认证，那么可以用它来解决认证问题。 另外还有其他的 Handler ，可以参考官方文档。https://docs.python.org/3/library/urllib.request.html#urllib.request.BaseHandler

它们怎么来使用，不用着急，下面会有实例为你演示。

另外一个比较重要的就是 OpenerDirector ，我们可以称之为 Opener ，我们之前用过 urllib.request.urlopen() 这个方法，实际上它就是一个 Opener 。

那么为什么要引入 Opener 呢？因为我们需要实现更高级的功能，之前我们使用的 Request 、 urlopen() 相当于类库为你封装好了极其常用的请求方法，利用它们两个我们就可以完成基本的请求，但是现在不一样了，我们需要实现更高级的功能，所以我们需要深入一层，使用更上层的实例来完成我们的操作。所以，在这里我们就用到了比调用 urlopen() 的对象的更普遍的对象，也就是 Opener 。

Opener 可以使用 open() 方法，返回的类型和 urlopen() 如出一辙。那么它和 Handler 有什么关系？简而言之，就是利用 Handler 来构建 Opener 。
认证
我们先用一个实例来感受一下：

```python
import urllib.request
auth_handler = urllib.request.HTTPBasicAuthHandler()
auth_handler.add_password(realm='PDQ Application',
                          uri='https://mahler:8092/site-updates.py',
                          user='klem',
                          passwd='kadidd!ehopper')
opener = urllib.request.build_opener(auth_handler)
urllib.request.install_opener(opener)
urllib.request.urlopen('http://www.example.com/login.html')
```

此处代码为实例代码，用于说明 Handler 和 Opener 的使用方法。在这里，首先实例化了一个 HTTPBasicAuthHandler 对象，然后利用 add_password() 添加进去用户名和密码，相当于建立了一个处理认证的处理器。
接下来利用 urllib.request.build_opener() 方法来利用这个处理器构建一个 Opener ，那么这个 Opener 在发送请求的时候就具备了认证功能了。接下来利用 Opener 的 open() 方法打开链接，就可以完成认证了。
代理

如果添加代理，可以这样做：

```python
import urllib.request
proxy_handler = urllib.request.ProxyHandler({
'http': 'http://218.202.111.10:80',
'https': 'https://180.250.163.34:8888'
})
opener = urllib.request.build_opener(proxy_handler)
response = opener.open('https://www.baidu.com')
print(response.read())
```

此处代码为实例代码，用于说明代理的设置方法，代理可能已经失效。

在这里使用了 ProxyHandler ， ProxyHandler 的参数是一个字典，key是协议类型，比如 http 还是 https 等，value是代理链接，可以添加多个代理。
然后利用 build_opener() 方法利用这个 Handler 构造一个 Opener ，然后发送请求即可。

六、**Cookie设置**

我们先用一个实例来感受一下怎样将网站的 Cookie 获取下来。

```python
import http.cookiejar, urllib.request
cookie = http.cookiejar.CookieJar()
handler = urllib.request.HTTPCookieProcessor(cookie)
opener = urllib.request.build_opener(handler)
response = opener.open('http://www.baidu.com')
for item in cookie:
   print(item.name+"="+item.value)
```

首先我们必须声明一个 CookieJar 对象，接下来我们就需要利用 HTTPCookieProcessor 来构建一个 handler ，最后利用 build_opener 方法构建出 opener ，执行 open() 即可。

运行结果如下：

```python
BAIDUID=2E65A683F8A8BA3DF521469DF8EFF1E1:FG=1
BIDUPSID=2E65A683F8A8BA3DF521469DF8EFF1E1
H_PS_PSSID=20987_1421_18282_17949_21122_17001_21227_21189_21161_20927
PSTM=1474900615
BDSVRTM=0
BD_HOME=0
```

可以看到输出了每一条 Cookie 的名称还有值。

不过既然能输出，那可不可以输出成文件格式呢？我们知道很多 Cookie 实际也是以文本形式保存的。

答案当然是肯定的，我们用下面的实例来感受一下：

```python
filename = 'cookie.txt'
cookie = http.cookiejar.MozillaCookieJar(filename)
handler = urllib.request.HTTPCookieProcessor(cookie)
opener = urllib.request.build_opener(handler)
response = opener.open('http://www.baidu.com')
cookie.save(ignore_discard=True, ignore_expires=True)
```

这时的 CookieJar 就需要换成 MozillaCookieJar ，生成文件时需要用到它，它是 CookieJar 的子类，可以用来处理 Cookie 和文件相关的事件，读取和保存 Cookie ，它可以将 Cookie 保存成 Mozilla 型的格式。
运行之后可以发现生成了一个 cookie.txt 文件。

内容如下：

```python
# Netscape HTTP Cookie File
# http://curl.haxx.se/rfc/cookie_spec.html
# This is a generated file! Do not edit.
.baidu.com TRUE / FALSE 3622386254 BAIDUID 05A
E39B5F56C1DEC474325CDA522D44F:FG=1
.baidu.com TRUE / FALSE 3622386254 BIDUPSID 05
AE39B5F56C1DEC474325CDA522D44F
.baidu.com TRUE / FALSE H_PS_PSSID 19638_1453
_17710_18240_21091_18560_17001_21191_21161
.baidu.com TRUE / FALSE 3622386254 PSTM 147490
2606
www.baidu.com FALSE / FALSE BDSVRTM 0
www.baidu.com FALSE / FALSE BD_HOME 0
```

另外还有一个 LWPCookieJar ，同样可以读取和保存 Cookie ，但是保存的格式和 MozillaCookieJar 的不一样，它会保存成与libwww-perl的Set-Cookie3文件格式的 Cookie 。
那么在声明时就改为

cookie = http.cookiejar.LWPCookieJar(filename)

```python
#LWP-Cookies-2.0
Set-Cookie3: BAIDUID="0CE9C56F598E69DB375B7C294AE5C591:FG=1"; path="/"; domain=".baidu.com"; path_spec; domain_dot; expires="208
4-10-14 18:25:19Z"; version=0
Set-Cookie3: BIDUPSID=0CE9C56F598E69DB375B7C294AE5C591; path="/"; domain=".baidu.com"; path_spec; domain_dot; expires="2084-10-1
4 18:25:19Z"; version=0
Set-Cookie3: H_PS_PSSID=20048_1448_18240_17944_21089_21192_21161_20929; path="/"; domain=".baidu.com"; path_spec; domain_dot; di
scard; version=0
Set-Cookie3: PSTM=1474902671; path="/"; domain=".baidu.com"; path_spec; domain_dot; expires="2084-10-14 18:25:19Z"; version=0
Set-Cookie3: BDSVRTM=0; path="/"; domain="www.baidu.com"; path_spec; discard; version=0
Set-Cookie3: BD_HOME=0; path="/"; domain="www.baidu.com"; path_spec; discard; version=0
```

生成的内容如下：由此看来生成的格式还是有比较大的差异的。
那么生成了 Cookie 文件，怎样从文件读取并利用呢？
下面我们以 LWPCookieJar 格式为例来感受一下：

```python
cookie = http.cookiejar.LWPCookieJar()
cookie.load('cookie.txt', ignore_discard=True, ignore_expires=True)
handler = urllib.request.HTTPCookieProcessor(cookie)
opener = urllib.request.build_opener(handler)
response = opener.open('http://www.baidu.com')
print(response.read().decode('utf-8'))
```

前提是我们首先利用上面的方式生成了 LWPCookieJar 格式的 Cookie ，然后利用 load() 方法，传入文件名称，后面同样的方法构建 handler 和 opener 即可。
运行结果正常输出百度网页的源代码。

好，通过如上用法，我们可以实现绝大多数请求功能的设置了。

### （2）requests库

requests库调用是requests.get方法传入url和参数，返回的对象是Response对象，打印出来是显示响应状态码。

通过.text 方法可以返回是unicode 型的数据，一般是在网页的header中定义的编码形式，而content返回的是bytes，二级制型的数据，还有 .json方法也可以返回json字符串。

如果想要提取文本就用text，但是如果你想要提取图片、文件等二进制文件，就要用content，当然decode之后，中文字符也会正常显示。

**requests的优势：**

Python爬虫时，更建议用requests库。因为requests比urllib更为便捷，requests可以直接构造get，post请求并发起，而urllib.request只能先构造get，post请求，再发起。

**对比使用urllib和使用requests**

1. 在使用urllib内的request模块时，返回体获取有效信息和请求体的拼接需要decode和encode后再进行装载。进行http请求时需先构造get或者post请求再进行调用，header等头文件也需先进行构造。
2. requests是对urllib的进一步封装，因此在使用上显得更加的便捷，建议在实际应用当中尽量使用requests。

- 使用urllib

```python3
from urllib import request
#请求头
headers = {
    "User-Agent": 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/64.0.3282.186 Safari/537.36'
}
wd = {"wd": "中国"}
url = "http://www.baidu.com/s?"
req = request.Request(url, headers=headers)
response = request.urlopen(req)
print(type(response))
print(response)
res = response.read().decode()
print(type(res))
print(res)
```

- 使用requests

```python3
import requests

headers = {
    "User-Agent": "Mozilla/5.0 (Linux; U; Android 8.1.0; zh-cn; BLA-AL00 Build/HUAWEIBLA-AL00) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/57.0.2987.132 MQQBrowser/8.9 Mobile Safari/537.36"
}
wd = {"wd": "中国"}
url = "http://www.baidu.com/s?"
response = requests.get(url, params=wd, headers=headers)
data = response.text
data2 = response.content
print(response)
print(type(response))
print(data)
print(type(data))
print(data2)
print(type(data2))
print(data2.decode())
print(type(data2.decode()))
```



# 十六、PyMySql操作Mysql

> 本段参考于[Python操作Mysql,这一篇就够了 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/397765212)

由于Mysql服务器以独立的进程运行，并通过网络对外服务。

所以我们需要支持Python的Mysql驱动来连接Mysql服务器。

在Python中支持Mysql的数据库模块有很多，我们选择使用PyMySql。

## 1、导入PyMySql

- 项目引入

```python3
import pymysql
```

- 命令行安装

```shell
pip install pymysql
```

## 2、连接数据库

使用数据库的第一步就是连接数据库，接下来我们看看如何使用PyMysql连接数据库。

1：连接数据库

2：创建游标对象

3：对数据库进行增删改查

4：关闭游标

5：关闭连接

```python3
import pymysql

# 打开数据库连接
try:
    db = pymysql.connect(host='localhost', user='root', passwd='123456', port=3306)
    print('连接成功！')
except:
    print('something wrong!')

# 使用 cursor() 方法创建一个游标对象 cursor
cursor = db.cursor()

# 使用 execute()  方法执行 SQL 查询
cursor.execute("SELECT VERSION()")

# 使用 fetchone() 方法获取单条数据.
data = cursor.fetchone()

print("Database version : %s " % data)

# 关闭数据库连接
db.close()
```

```python
连接成功！
Database version : 5.7.19 
```

## 3、创建数据库表

如果数据库连接存在我们可以使用execute()方法来为数据库创建表，如下所示创建表EMPLOYEE：

```python3
import pymysql

# 打开数据库连接
try:
    db = pymysql.connect(host='localhost', user='root', passwd='123456', port=3306, db='test')
    print('连接成功！')
except:
    print('something wrong!')

# 使用 cursor() 方法创建一个游标对象 cursor
cursor = db.cursor()

# 使用 execute() 方法执行 SQL，如果表存在则删除
cursor.execute("DROP TABLE IF EXISTS EMPLOYEE")

# 使用预处理语句创建表
sql = """CREATE TABLE EMPLOYEE (
         FIRST_NAME  CHAR(20) NOT NULL,
         LAST_NAME  CHAR(20),
         AGE INT,  
         SEX CHAR(1),
         INCOME FLOAT )"""

cursor.execute(sql)
print('建表成功！')

# 关闭数据库连接
db.close()
```

```xml
连接成功！
建表成功！
```

可以打开Navicat发现在我们名称为test的数据库下多了一个employee的Table。如下图：

![image-20231028164752597](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231028164752597.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 4、插入数据

我们来看看如何使用INSERT语句向表 EMPLOYEE 插入数据。

```python3
import pymysql

# 打开数据库连接
try:
    db = pymysql.connect(host='localhost', user='root', passwd='123456', port=3306, db='test')
    print('连接成功！')
except:
    print('something wrong!')

# 使用 cursor() 方法创建一个游标对象 cursor
cursor = db.cursor()

# SQL 插入语句
sql = """INSERT INTO EMPLOYEE(FIRST_NAME,
         LAST_NAME, AGE, SEX, INCOME)
         VALUES ('Mac', 'Mohan', 20, 'M', 2000)"""
try:
    # 执行sql语句
    cursor.execute(sql)
    # 提交到数据库执行
    db.commit()
    print('数据插入成功！')
except:
    # 如果发生错误则回滚
    db.rollback()
    print('数据插入错误！')

# 关闭数据库连接
db.close()

'''
连接成功！
数据插入成功！
'''
```

![image-20231028165713086](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231028165713086.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 5、数据库查询操作

Python查询Mysql使用 fetchone() 方法获取单条数据, 使用fetchall() 方法获取多条数据。

- fetchone(): 该方法获取下一个查询结果集。结果集是一个对象
- fetchall(): 接收全部的返回结果行.
- rowcount: 这是一个只读属性，并返回执行execute()方法后影响的行数。

查询EMPLOYEE表中salary（工资）字段大于1000的所有数据：

```python3
import pymysql

# 打开数据库连接
try:
    db = pymysql.connect(host='localhost', user='root', passwd='123456', port=3306, db='test')
    print('连接成功！')
except:
    print('something wrong!')

# 使用 cursor() 方法创建一个游标对象 cursor
cursor = db.cursor()

# SQL 查询语句
sql = "SELECT * FROM EMPLOYEE \
       WHERE INCOME > %s" % (1000)
try:
    # 执行SQL语句
    cursor.execute(sql)
    # 获取所有记录列表
    results = cursor.fetchall()
    for row in results:
        fname = row[0]
        lname = row[1]
        age = row[2]
        sex = row[3]
        income = row[4]
        # 打印结果
        print('数据查询成功！')
        print("fname=%s,lname=%s,age=%s,sex=%s,income=%s" % \
              (fname, lname, age, sex, income))
except:
    print("Error: unable to fetch data")

# 关闭数据库连接
db.close()
'''
连接成功！
数据查询成功！
fname=Mac,lname=Mohan,age=20,sex=M,income=2000.0
'''
```

```xml
连接成功！
数据查询成功！
fname=Mac,lname=Mohan,age=20,sex=M,income=2000.0
```

## 6、数据库更新操作

更新操作用于更新数据表的的数据，以下实例将 TESTDB 表中 SEX 为 'M' 的 AGE 字段递增 1：

```python3
import pymysql

# 打开数据库连接
try:
    db = pymysql.connect(host='localhost', user='root', passwd='123456', port=3306, db='test')
    print('连接成功！')
except:
    print('something wrong!')

# 使用 cursor() 方法创建一个游标对象 cursor
cursor = db.cursor()

# SQL 更新语句
sql = "UPDATE EMPLOYEE SET AGE = AGE + 1 WHERE SEX = '%c'" % ('M')
try:
    # 执行SQL语句
    cursor.execute(sql)
    # 提交到数据库执行
    db.commit()
    print('数据更新成功！')
except:
    # 发生错误时回滚
    db.rollback()

# 关闭数据库连接
db.close()
```

```xml
连接成功！
数据更新成功！
```

![image-20231028180741501](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231028180741501.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 7、删除操作

删除操作用于删除数据表中的数据，以下实例演示了删除数据表 EMPLOYEE 中 AGE 大于 20 的所有数据：

```python3
import pymysql

# 打开数据库连接
try:
    db = pymysql.connect(host='localhost', user='root', passwd='123456', port=3306, db='test')
    print('连接成功！')
except:
    print('something wrong!')

# 使用 cursor() 方法创建一个游标对象 cursor
cursor = db.cursor()

# SQL 删除语句
sql = "DELETE FROM EMPLOYEE WHERE AGE > %s" % (20)
try:
    # 执行SQL语句
    cursor.execute(sql)
    # 提交修改
    db.commit()
    print('数据删除成功')
except:
    # 发生错误时回滚
    db.rollback()

# 关闭连接
db.close()
```

```xml
连接成功！
数据删除成功
```

![image-20231028180954681](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231028180954681.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 8、执行事务

什么是事务？

转账是生活中常见的操作,比如从A账户转账100元到B账号。

站在用户角度而言,这是一个逻辑上的单一操作,然而在数据库系统中,至少会分成两个步骤来完成:

- 1.将A账户的金额减少100元
- 2.将B账户的金额增加100元。

![image-20231028181258432](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/image-20231028181258432.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



在这个过程中可能会出现以下问题:

- 1.转账操作的第一步执行成功,A账户上的钱减少了100元,但是第二步执行失败或者未执行便发生系统崩溃,导致B账户并没有相应增加100元。
- 2.转账操作刚完成就发生系统崩溃,系统重启恢复时丢失了崩溃前的转账记录。
- 3.同时又另一个用户转账给B账户,由于同时对B账户进行操作,导致B账户金额出现异常。

为了便于解决这些问题,需要引入数据库事务的概念。

事务应该具有4个属性：原子性、一致性、隔离性、持久性。这四个属性通常称为ACID特性。

**原子性**(Atomicity):事务中的所有操作作为一个整体像原子一样不可分割，要么全部成功,要么全部失败。

**一致性**(Consistency):事务的执行结果必须使数据库从一个一致性状态到另一个一致性状态。一致性状态是指:1.系统的状态满足数据的完整性约束(主码,参照完整性,check约束等) 2.系统的状态反应数据库本应描述的现实世界的真实状态,比如转账前后两个账户的金额总和应该保持不变。

**隔离性**(Isolation):并发执行的事务不会相互影响,其对数据库的影响和它们串行执行时一样。比如多个用户同时往一个账户转账,最后账户的结果应该和他们按先后次序转账的结果一样。

**持久性**(Durability):事务一旦提交,其对数据库的更新就是持久的。任何事务或系统故障都不会导致数据丢失。

在事务的ACID特性中,C即一致性是事务的根本追求,而对数据一致性的破坏主要来自两个方面

```python3
# SQL删除记录语句
sql = "DELETE FROM EMPLOYEE WHERE AGE > %s" % (20)
try:
   # 执行SQL语句
   cursor.execute(sql)
   # 向数据库提交
   db.commit()
except:
   # 发生错误时回滚
   db.rollback()
```

对于支持事务的数据库， 在Python数据库编程中，当游标建立之时，就自动开始了一个隐形的数据库事务。

commit()方法游标的所有更新操作，rollback()方法回滚当前游标的所有操作。每一个方法都开始了一个新的事务。



## 9、防SQL注入

> 本段转载于[Python使用MySQL数据库方法及防SQL注入_皛心的博客-CSDN博客](https://blog.csdn.net/m0_47670683/article/details/114002909)

**SQL注入攻击**：指在传递实参时，使用特殊字符或SQL关键字，在拼接成SQL后，这条SQL语句就有一定的攻击性，在一定程度上可以修改代码。

关于防SQL语句注入要先看案例再来说明：

假设有一个应用，登录时需要用户提供用户名和密码。

Python程序收到用户输入的用户名和密码后再提交到MySQL数据库进行比对，若用户名和密码正确则允许登录，错误则拒绝登录。

- 一、创建测试用的库和表：

  ```sql
  create database test_login;
  use test_login;
  create table login(name char(12),password char(12));
  insert into login values('张三','123456');
  ```

- 二、未防范[SQL注入](https://so.csdn.net/so/search?q=SQL注入&spm=1001.2101.3001.7020)的错误代码案例：

  ```python
  import pymysql
  
  with pymysql.connect(host='127.0.0.1', user='你的账户', password='你的密码', database='test_login') \
          as conn, conn.cursor() as cur:
      usr = input('请输入用户名：')
      pwd = input('请输入密码：')
      condition = f'select * from login where name="{usr}" and password="{pwd}"'
      print(condition)
      cur.execute(condition)
      if cur.rowcount:
          print('登录成功')
      else:
          print('登录失败')
  ```

- 三、测试SQL注入，在输用户名时输入 1" or 1=1; #，请看下图：

  ![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210223205829995.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

  请认真看上面打印的sql语句内容：

  ```sql
  select * from login where name="1" or 1=1; #" and password="1"
  ```

  请注意sql语句中#表示注释后面的全部内容，所以MySQL服务端真正执行的语句如下：

  ```sql
  select * from login where name="1" or 1=1;
  ```

  看到这相信大家都能明白为啥无论密码输入什么都能登录成功，以上就是**著名的SQL注入**。

  上面的案例仅仅是示范如何绕过安全验证，实际上通过SQL注入甚至可以删库、删表造成整个系统崩溃。

  所以我们写代码时必须要防范SQL注入！

- 四、防范SQL注入的正确代码：

**使用占位符**

  ```python
import pymysql

with pymysql.connect(host='127.0.0.1',  user='你的账户', password='你的密码', database='test_login') \
        as conn, conn.cursor() as cur:
    usr = input('请输入用户名：')
    pwd = input('请输入密码：')
    condition = 'select * from login where name="%s" and password="%s"'
    print(condition)
    cur.execute(condition, (usr, pwd))  # execute方法有2个参数，第一个是SQL语句，第二个是元组(元组的成员是多个参数)
    if cur.rowcount:
        print('登录成功')
    else:
        print('登录失败')
  ```

- 五、测试SQL注入

  ![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-ScwmOz06-1614085050023)(/home/windf/图片/sqlzr2.jpg)]](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210223205745214.jpg?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

  此时可以看到SQL注入不会生效，请牢记execute防范SQL注入的正确方法！！！

  写代码务必不要出现可以SQL注入的巨大漏洞！！！
  补充一条：可以在用户输入用户名和密码时进行检测，不允许用户名和密码中出现**;和#**这2个符号。

  这样也可以有效地防范SQL注入！

# 十七、多线程

> 本段转载于[探索Python的多线程编程：原理与实践-腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/2301975?areaId=106005)
>
> [Python多线程编程（详细：适合小白入门）_手可摘星辰不去高声语的博客-CSDN博客](https://blog.csdn.net/weixin_44917390/article/details/119610760)
>
> [Python中的多线程（史上最简单易懂版）_python 多线程-CSDN博客](https://blog.csdn.net/Elon15/article/details/125350491)
>
> [python多线程详解（超详细）-CSDN博客](https://blog.csdn.net/weixin_40481076/article/details/101594705)

在计算机科学领域，多线程编程是一种重要的技术，用于实现并发执行和提高程序性能。

Python作为一门广泛使用的编程语言，在多线程编程方面也有着强大的支持。

多线程简单理解就是：一个CPU，也就是单核，将时间切成一片一片的，

CPU轮转着去处理一件一件的事情，到了规定的[时间片](https://so.csdn.net/so/search?q=时间片&spm=1001.2101.3001.7020)就处理下一件事情。

## 1、多任务

**进程是分配资源的最小单位，一旦创建一个进程就会分配一定的资源（打开两个QQ）**

**线程是程序执行的最小单元，**实际上进程只负责分配资源，而利用这些资源执行程序的是线程，

也就是说**进程是线程的容器，一个进程中最少有一个线程来负责执行程序**。

线程（Thread）是操作系统能够进行运算调度的最小单位。

一个进程可以包含多个线程，每个线程独立执行特定的任务，共享进程的资源。与单线程相比，多线程可以实现并发执行，提高程序的执行效率。

多线程编程具有以下优势和适用场景：

- 加速程序执行：多线程可以同时执行多个任务，提高程序的处理能力和响应速度。
- 并发处理：多线程可以同时处理多个并发请求，适用于[服务器](https://cloud.tencent.com/act/pro/promotion-cvm?from_column=20065&from=20065)端程序和网络编程。
- 可以充分利用多核处理器的优势，提高系统性能。

然而，多线程编程也存在一些挑战和注意事项，如线程安全、资源竞争等问题。

线程自己不拥有系统资源，但可与同属一个进程的其他线程**共享进程所拥有的全部资源（一个QQ打开两个chat窗口）**

**--- > 进程：**

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811165755207.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**--- >** **线程：**

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811201819239.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

**什么是线程？**  

线程也叫轻量级进程，是操作系统能够进行运算调度的最小单位，它被包涵在进程之中，是进程中的实际运作单位。

线程自己不拥有系统资源，只拥有一点儿在运行中必不可少的资源，但它可与同属一个进程的其他线程共享进程所拥有的全部资源。

一个线程可以创建和撤销另一个线程，同一个进程中的多个线程之间可以并发执行。

**为什么要使用多线程？**

线程在程序中是独立的、并发的执行流。

与分隔的进程相比，进程中线程之间的隔离程度要小，它们共享内存、文件句柄和其他进程应有的状态。

 因为线程的划分尺度小于进程，使得多线程程序的并发性高。

进程在执行过程之中拥有独立的内存单元，而多个线程共享    内存，从而极大的提升了程序的运行效率。

 线程比进程具有更高的性能，这是由于同一个进程中的线程都有共性，多个线程共享一个进程的虚拟空间。

线程的共享环境包括进程代码段、进程的共有数据等，利用这些共享的数据，线程之间很容易实现通信。    

操作系统在创建进程时，必须为改进程分配独立的内存空间，并分配大量的相关资源，但创建线程则简单得多。

因此，使用多线程来实现并发比使用多进程的性能高得要多。

总结起来，使用多线程编程具有**如下几个优点**：    

进程之间不能共享内存，但线程之间共享内存非常容易。    

操作系统在创建进程时，需要为该进程重新分配系统资源，但创建线程的代价则小得多。因此使用多线程来实现多任务并发执行比使用多进程的效率高。   

python语言内置了多线程功能支持，而不是单纯地作为底层操作系统的调度方式，从而简化了python的多线程编程。



## 2.多线程完成多任务

### （1）线程的创建步骤

```python
①导入线程模块
import threading
②通过线程类创建进程对象
线程对象 = threading.Thread(target = 任务名)
③启动线程执行任务
线程对象.start()
```

```python3
print("当前活跃线程的数量", threading.active_count())
print("将当前所有线程的具体信息展示出来", threading.enumerate())
print("当前的线程的信息展示", threading.current_thread())
```

### （2）通过线程类创建线程对象

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811202405767.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （3）线程创建与启动代码

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811202447261.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



```python
import threading
import time
def sing():
	for i in range(3):
	print("i am sing ooo~")
	time.sleep(0.5)
def dance():
    for i in range(3):
        print("i am dance lll~")
        time.sleep(0.5)
if __name__ == '__main__':
    sing_thread = threading.Thread(target=sing)
    dance_thread = threading.Thread(target=dance)
    sing_thread.start()
    dance_thread.start()
```

 ![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811202929246.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 线程执行有参数的任务

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811203014328.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



```python
import threading
import time
def sing(num):
    for i in range(num):
        print("i am sing ooo~")
        time.sleep(0.5)
def dance(num):
    for i in range(num):
        print("i am dance lll~")
        time.sleep(0.5)
if __name__ == '__main__':
    sing_thread = threading.Thread(target=sing, args=(3,))
    dance_thread = threading.Thread(target=dance, kwargs={"num": 2})
    sing_thread.start()
    dance_thread.start()
```

 ![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811203327564.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （4）主线程和子线程的结束顺序

- 主线程会**等待所有的子线程执行结束后**再结束

- 设置守护子线程（主完子销）![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811203551908.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

 设置守护子线程有两种方式：

 ![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811203839134.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

###  （5）线程间的执行顺序

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811204034402.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

- 获取当前的线程信息

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811204135844.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

```python
import threading
import time
def task():
    time.sleep(0.5)
    # current_thread:获取当前线程的线程对象
    thread = threading.current_thread()
    print(thread)
if __name__ == '__main__':
    for i in range(5):
        sub_thread = threading.Thread(target=task)
        sub_thread.start()
```

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811204909370.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （6）多线程实现视频文件夹高并发copy器

 同进程不一样之处：

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/20210811210317577.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



```python
# 1.导入包和模块
import threading
import os
def copy_file(file_name, source_dir, dest_dir):
    print(file_name, "--拷贝的进程pid是：", os.getpid())
    print(file_name, "--拷贝的线程是：", threading.current_thread())
    # 1.拼接源文件路径和目标文件所在的路径
    source_path = source_dir + "/" + file_name
    dest_path = dest_dir + "/" + file_name
    # 2.打开源文件和目标文件
    with open(source_path, "rb") as source_file:
        with open(dest_path, "wb") as dest_file:
            # 3.循环读取源文件到目标路径
            while True:
                data = source_file.read(1024)
                if data:
                    dest_file.write(data)
                else:
                    break
                    
                    
if __name__ == '__main__':
    # 1.定义源文件夹和目标文件夹
    source_dir = "源文件夹"
    dest_dir = "目标文件夹"
    # 2.创建目标文件夹
    try:
        os.mkdir(dest_dir)
    except:
        print("目标文件夹已经存在！")
    # 3.读取源文件夹的文件列表
    file_list = os.listdir(source_dir)
    # 4.遍历文件列表实现拷贝
    for file_name in file_list:
        # copy_file(file_name, source_dir, dest_dir)
        # 5.使用多线程实现多任务拷贝
        sub_thread = threading.Thread(target=copy_file,args=(file_name, source_dir, dest_dir))
        sub_thread.start()
```

![img](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/2021081121043070.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)



### （7）线程中的join函数

预想的是，执行完线程1，然后输出All done…“理想很丰满，现实却不是这样的”

```python
# coding:utf-8
import threading
import time

def job1():
    print("T1 start")
    for i in range(5):
        time.sleep(1)
        print(i)
    print("T1 finish")


def main():
    # 新创建一个线程
    new_thread = threading.Thread(target=job1, name="T1")
    # 启动新线程
    new_thread.start()
    print("All done...")


if __name__ == "__main__":
    main()
```

效果图：
![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/3f94a42729554ccf84624d4161400828.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)
为了达到我们的预期，我们使用join函数，将T1线程进行阻塞。

join函数进行阻塞是什么意思？

就是哪个线程使用了join函数，当这个线程正在执行时，**在他之后的线程程序不能执行**，得等这个被阻塞的线程全部执行完毕之后，方可执行！

```python
# coding:utf-8
import threading
import time

def job1():
    print("T1 start")
    for i in range(5):
        time.sleep(1)
        print(i)
    print("T1 finish")


def main():
    # 新创建一个线程
    new_thread = threading.Thread(target=job1, name="T1")
    # 启动新线程
    new_thread.start()
    # 阻塞这个T1线程
    new_thread.join()
    print("All done...")


if __name__ == "__main__":
    main()
123456789101112131415161718192021222324
```

效果图：
![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/3ef89b325c5247f1b52bfc52a73c7014.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （8）使用Queue存储线程的结果

线程的执行结果，**无法通过return进行返回**，使用**Queue**存储。

```python
# coding:utf-8
import threading
from queue import Queue
"""
    Queue的使用
"""

def job(l, q):
    for i in range(len(l)):
        l[i] = l[i] ** 2
    q.put(l)


def multithreading():
    # 创建队列
    q = Queue()
    # 线程列表
    threads = []
    # 二维列表
    data = [[1, 2, 3], [4, 5, 6], [7, 8, 9], [6, 6, 6]]
    for i in range(4):
        t = threading.Thread(target=job, args=(data[i], q))
        t.start()
        threads.append(t)

    # 对所有线程进行阻塞
    for thread in threads:
        thread.join()
    results = []
    # 将新队列中的每个元素挨个放到结果列表中
    for _ in range(4):
        results.append(q.get())
    print(results)


if __name__ == "__main__":
    multithreading()
```

效果图：
![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/acc479d5c5824ef2b8773abdbec2b3a2.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

### （9）线程锁lock

**当同时启动多个线程时，各个线程之间会互相抢占计算资源，会造成程序混乱。**

举个栗子：

当我们在选课系统选课时，当前篮球课还有2个名额，我们三个人去选课。

选课顺序为stu1 stu2 stu3,应该依次打印他们三个的选课过程，但是现实情况却是：

```python
# coding:utf-8
import threading
import time

def stu1():
    print("stu1开始选课")
    global course
    if course > 0:
        course -= 1
        time.sleep(2)
        print("stu1选课成功,现在篮球课所剩名额为%d" % course)
    else:
        time.sleep(2)
        print("stu1选课失败，篮球课名额为0，请选择其他课程")



def stu2():
    print("stu2开始选课")
    global course
    if course > 0:
        course -= 1
        time.sleep(2)
        print("stu2选课成功,现在篮球课所剩名额为%d" % course)
    else:
        time.sleep(2)
        print("stu2选课失败，篮球课名额为0，请选择其他课程")

def stu3():
    print("stu3开始选课")
    global course
    if course > 0:
        course -= 1
        time.sleep(2)
        print("stu3选课成功")
        print("篮球课所剩名额为%d" %course)
    else:
        time.sleep(2)
        print("stu3选课失败，篮球课名额为0，请选择其他课程")


if __name__ == "__main__":
    # 篮球课名额
    course = 2
    T1 = threading.Thread(target=stu1, name="T1")
    T2 = threading.Thread(target=stu2, name="T2")
    T3 = threading.Thread(target=stu3, name="T3")
    T1.start()
    T2.start()
    T3.start()
```

效果图：
![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/b4527a865a3845db9238d16c2c4a18ad.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)
		为了解决这种情况，我们使用lock线程同步锁，在线程并发执行时，保证**每个线程执行的原子性**。

有效防止了共享统一数据时，线程并发执行的混乱。

改进的代码如下：

```python
# coding:utf-8
import threading
import time

def stu1():
    global lock
    lock.acquire()
    print("stu1开始选课")
    global course
    if course > 0:
        course -= 1
        time.sleep(2)
        print("stu1选课成功,现在篮球课所剩名额为%d" % course)
    else:
        time.sleep(2)
        print("stu1选课失败，篮球课名额为0，请选择其他课程")
    lock.release()


def stu2():
    global lock
    lock.acquire()
    print("stu2开始选课")
    global course
    if course > 0:
        course -= 1
        print("stu2选课成功,现在篮球课所剩名额为%d" % course)
    else:
        time.sleep(1)
        print("stu2选课失败，篮球课名额为0，请选择其他课程")
    lock.release()

def stu3():
    global lock
    lock.acquire()
    print("stu3开始选课")
    global course
    if course > 0:
        course -= 1
        time.sleep(1)
        print("stu3选课成功,现在篮球课所剩名额为%d" % course)
    else:
        time.sleep(1)
        print("stu3选课失败，篮球课名额为0，请选择其他课程")
    lock.release()

if __name__ == "__main__":
    # 篮球课名额
    course = 2
    # 创建同步锁
    lock = threading.Lock()
    T1 = threading.Thread(target=stu1, name="T1")
    T2 = threading.Thread(target=stu2, name="T2")
    T3 = threading.Thread(target=stu3, name="T3")
    T1.start()
    T2.start()
    T3.start()
```

效果图：
![在这里插入图片描述](https://haobin-001.oss-cn-hangzhou.aliyuncs.com/imgs-for-typora/4e92f7621f9f488594754c0f04c42994.png?x-oss-process=image/auto-orient,1/quality,q_90/watermark,text_56iL5bqP5ZGY5aW95Yaw,type_ZmFuZ3poZW5na2FpdGk,color_fef6f0,size_30,shadow_100,g_se,x_10,y_10)

## 3、进程和线程对比

| 关系对比 | 线程是依附在进程里面的，没有进程就没有线程**；**一个进程默认提供一个线程，进程可以创建多个线程 |
| :------: | :----------------------------------------------------------: |
| 区别对比 | 创建进程的资源开销比创建线程的资源开销要大，进程可以用多核，但是线程不能用多核；进程是操作系统资源分配的基本单位，线程是CPU调度的基本单位 |

## 4、线程同步和共享资源

在多线程编程中，多个线程可能会**同时访问和修改共享资源**，这会引发一些问题，如数据竞争和线程安全性。

因此，必须采取适当的措施来实现线程同步和保护共享资源的完整性。

Python提供了多种机制来实现线程同步和共享资源的保护，如互斥锁、信号量、条件变量等。

这些机制可以通过`threading`模块中的相应类来实现。

下面是一个示例，展示了如何使用互斥锁来保护共享资源：

```python3
import threading

# 共享资源
counter = 0

# 互斥锁
mutex = threading.Lock()

# 线程函数
def increment_counter():
    global counter
    mutex.acquire()  # 获取锁
    try:
        counter += 1
    finally:
        mutex.release()  # 释放锁

# 创建多个线程并启动
threads = []
for _ in range(10):
    thread = threading.Thread(target=increment_counter)
    threads.append(thread)
    thread.start()

# 等待所有线程结束
for thread in threads:
    thread.join()

# 输出结果
print("Counter:", counter)
```

在上述示例中，我们首先定义了一个名为`counter`的共享资源和一个互斥锁`mutex`。

然后，我们定义了一个线程函数`increment_counter()`，它通过获取互斥锁、修改`counter`的值，然后释放互斥锁来实现对共享资源的安全访问。

最后，我们创建了多个线程并启动它们，等待所有线程执行完毕后输出最终结果。

## 5、线程间的通信

在多线程编程中，线程之间可能需要进行数据交换和通信。

Python提供了一些机制来实现线程间的通信，如队列（Queue）和事件（Event）。

下面是一个示例，展示了如何使用队列来实现线程间的数据交换：

```python
import threading
import queue

# 队列
message_queue = queue.Queue()

# 生产者线程函数
def producer():
    for i in range(5):
        message_queue.put(f"Message {i+1}")
        threading.sleep(1)

# 消费者线程函数
def consumer():
    while True:
        message = message_queue.get()
        print("Received:", message)
        message_queue.task_done()

# 创建生产者和消费者线程并启动
producer_thread = threading.Thread(target=producer)
consumer_thread = threading.Thread(target=consumer)

producer_thread.start()
consumer_thread.start()

# 等待生产者线程结束
producer_thread.join()

# 清空队列
message_queue.join()
consumer_thread.join()
```

在上述示例中，我们首先创建了一个名为`message_queue`的队列，用于存储消息。

然后，我们定义了一个生产者线程函数`producer()`和一个消费者线程函数`consumer()`。

生产者线程通过将消息放入队列中来生产数据，消费者线程通过从队列中获取消息来进行消费。

最后，我们创建了生产者和消费者线程，并启动它们。

等待生产者线程结束后，我们调用`join()`方法等待队列中的所有任务完成，然后再结束消费者线程。

## 6、自定义线程

**继承threading.Thread来定义线程类，其本质是重构Thread类中的run方法。**

```python3
import threading
import time


class MyThread(threading.Thread):
    def __init__(self, n):
        super(MyThread, self).__init__()  # 重构run函数必须写
        self.n = n

    def run(self):
        print('task', self.n)
        time.sleep(1)
        print('2s')
        time.sleep(1)
        print('1s')
        time.sleep(1)
        print('0s')
        time.sleep(1)


if __name__ == '__main__':
    t1 = MyThread('t1')
    t2 = MyThread('t2')
    t1.start()
    t2.start()
```

## 7. 多线程编程的实践

### （1） 使用多线程改善程序性能

多线程编程可以充分利用多核处理器的优势，提高程序的性能。

在某些场景下，多线程可以帮助我们加速程序的执行，特别是对于那些密集计算或需要大量IO操作的任务。

例如，在[图像处理](https://cloud.tencent.com/product/tiia?from_column=20065&from=20065)任务中，可以使用多个线程同时处理不同的图片，从而加速整个处理过程。

类似地，在网络编程中，可以使用多线程同时处理多个客户端请求，提高服务器的性能和并发处理能力。

### （2）注意事项和限制

在使用多线程编程时，需要注意以下事项和限制：

- 线程安全：**多个线程同时访问和修改共享资源**时可能会引发线程安全问题，**需要采取适当的线程同步机制来保护共享资源**。
- 全局解释器锁（GIL）：由于Python的全局解释器锁，多线程程序无法充分利用多核处理器的优势。这意味着在某些情况下，使用**多线程并不能明显提高程序的执行效率**。
- 死锁：如果在多线程编程中未正确处理同步和资源分配，可能会**导致死锁**，即线程互相等待对方释放资源而无法继续执行。
- 调试困难：由于多线程的执行是**异步的**，因此调试多线程程序可能比单线程更加困难。遇到问题时，需要仔细检查代码，使用适当的工具和技术进行调试。



# 项目推荐

[可视化图鉴 - Heywhale.com](https://www.heywhale.com/home/column/60e2740e3aeb9c0017b967a2)

---

> <strong> 🚀<font color = red>先看后赞，养成习惯！</font>🚀</strong>
>
> <strong> 🚀<font color = red> 先看后赞，养成习惯！</font>🚀</strong>

> **🎈觉得文章写得不错的老铁们，点赞评论关注走一波！谢谢啦！🎈**

---



