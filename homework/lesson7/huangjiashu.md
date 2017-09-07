### [网页预览地址](https://mycolourfullife.github.io/showYourBeautifuHeart/)

### [项目地址](https://github.com/MyColourfulLife/showYourBeautifuHeart.git)

### 团队名： 火力全开

#### 团队组成（排名不分先后）：
	- 黄家树
	- 张丽娜
	- 张大美
	- 唐芳
	- 郭威

#### 一些感想

1. 万事开头难

万事开头难，课是听了，半天没下去手，就在VScode里敲了个hmtl自动给我补全了不少代码，
然后就去老师的网页抄代码 右键 检查  。。。，抄的其表，难抄其心。整了一两个小时，没啥进展，搭个结构都丑爆了。

终于想起去老师讲课时的源代码了，这才是经典，核心内容都在里面了，于是直接搬过来，算是好看些了，使用vue，绑定数据，
使用bootstrop 打打框架。还好，能看。

**万事开头难，是因为没掌握正确的打开方式。**

2. 有些问题，在说明文档里就有答案

按道理来讲，是应该好好看看vue的说明文档的。但是也没怎么看，太多了看完也不现实，作为工具书 用到时候查查就好了。但是总会遗漏一些东西。
比如 直接给列表赋值，vue并不会去渲染这种赋值操作，这个bug也困扰了我一个多小时吧，为了解决这个bug，愣是自己调试调出来的。
自己也在思考这是为什么，我想的原因是 直接对数组赋值，地址指向发生了改变，而数组追加数据 地址指向并非发生改变。像对象这种东西，称之为容器，
直接改变容器的地址，vue没有渲染，我想vue是在监听之前地址所指向的对象的变化。而对于一个新的对象，它并不理会。这是我个人的理解。

后来在群里向老师问了为什么直接赋值不渲染页面，老师给了[这个](https://cn.vuejs.org/v2/guide/list.html#数组更新检测)，我要是有仔细看这个文档，应该就不存在我那个所谓的bug了。
 
 有些坑，能不踩最好，不小心踩上了，也不是什么坏事，早早踩上了，才会印象深刻。

 **有些问题，费尽心思搞明白的东西，其实赫然写在说明文档里，你遇到问题是闷头解决问题，还是抬起头去搜搜文档呢？**

3. 一个健壮的程序

自从老师讲了写一个函数 要先判断参数 再执行逻辑 最后返回结果
就对参数判断这个环节格外印象审核，为什么呢？因为有太多的错误，太多的崩溃是因为参数不对引起的。
所以在写部分函数时，就会额外增加对参数的判断，甚至有些时候，即便函数没有参数也要对用到的变量做判断。

** 一个健壮的程序，要对逻辑处理中用到的必要的参数或者变量 做判断 **

4. vue的数据绑定

最基本的原则是 定义一个id作为 映射的起点， 数据部分写到 data 里 函数部分 写到methods里，用到的时候直接用里面的内容即可。
- 绑定的方式是用双挂括弧括起来，在使用中发现，这只是其中的一种方式，在不用的场景下有不同的绑定方式，这种方式适用于文本标签或者可以直接输入文本内容而非用字符串引起来的。此外，对于属性，方法的绑定，通常都以v字开头，比如v-on v-for v-bind 等。
- v-bind: 在标签的属性中 内容通常在写字符串里，比如 a标签的herf 不使用v-bind： herf = "item.url"  双引号表示的是什么就是什么，因此如果想让双引号里面的内容不这么按原班人马显示，就要用v-bind标示，这个字符串里的内容需要vue特殊处理。
- 其他 v-on：应该是对事件的监听，还有好些写法，没有做研究，但不同的绑定方式肯定是针对不同的场景而生的。当然还有经典的v-for = 这种应该是用来写表达式的，有for应该就有v-if，我想这个东西在vue里都用，用到的时候看看应该就明白了，**瞎想不如直接看文档**。

** 数据绑定是vue的核心，掌握其绑定规则，让网页渲染数据变得简单 **

5. axios 灰常好用的网络请求
之前展示心里话的时候，直接就是复制的数据。老师开放了API，又教了axios这个好东西，直接搬过来，简单改下代码，就可以获取数据了，
再经过简单的调试，就能和之前的 vue 联合起来显示数据了。
axios这种链式的书写方法写起来真的好爽。

** 老师说，先把一个东西用熟了就好，js网络请求就用 axios了 **


#### 后记
上面都把事情想的简单了，每一点其实都需要付出大量的时间和精力才有可能做好。有时候做的不够好，扪心自问下，我在这上面耗费了多少时间，又耗费了多少注意力？
不过，老师讲的那些，已经可以让我搭建一个简单的网页了，这就是起步的力量。


