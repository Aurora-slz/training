# Day 1 

早早的起了床，然后搭毛老师的顺风车一起到了车站。在车站遇到了烟大的盆友们，和超神他们聊了聊，不禁又一次的感受到了来自友校的压力，但其实我们的对手归根结底还是自己。高铁上，记了一路六级词，每天的任务还是要坚持下去。

济南好热，济大好大，忽然间觉得学校小也是蛮好滴...但济大这次是真的用心了，从去年办趣味编程的时候就深有感触，每个或大或小的比赛，背后都需要大量的人力物力，各个方面都要考虑全面，稍有偏差就会被喷的很惨，更何况还是这全省的比赛。从报道时接到队服还有挂牌的时候就能感受的到，白色的队服，几乎看不到广告的印记，质量感觉和优衣库买的甚至没太大区别，袋子和挂牌上居然有自己的队名和队名，真的太有纪念意义了。

## 热身赛: 
据说第三道好像是青岛区域赛原题，不过第四个题是真的醉了..哇..死肥宅..懵逼了一会就开始测后台了。

## 赛后
赛后去芙蓉街还有泉城广场转了一圈，音乐喷泉真好看。回来之后就在想，明天一定要先保住水题，保证正确率，然后就早点睡了。

# Day 2

## 正式赛: 
开始之前，我先把头文件写在了纸上，比赛开始我就直接对着敲，队友分别先看两个题，刚开始A没仔细读，直接按输入输出揣测了样例，然后犹豫了一会，浪费了一些时间。于是先搞了红色的M题，然后上来交了一发T，妈呀1e9暴力肯定超啊，然后想着怎么把循环去掉，后来一想转对数也就20根本超不了啊...淡定淡定，稳住别慌，A了。
然后顺便瞄了一眼A的题意，只看了两句发现怎么跟刚才理解的不大一样，啊都是30天，一周都按5天啊，一年360天，跟闰不闰年没关系啊，同时队友先写F，然后我接着敲了这个，这俩基本是紧接着直接过了。
然后我开始翻C，队友开始搞D，WA了，然后我们一起找bug，后来猛然间发现，k也有可能小于n啊..哇..又是没仔细看题。
然后C，大概有了思路，举了几组栗子好像没找到什么反例，然后就试了一下，然后一直WA，也没找到手误，这时候顺便看了一眼榜，发现就这几个题出的人多，其他题出的都比较少，想想去年不算那个没数据的F题的话，当时真正能出的也就俩，就感觉其他题肯定都是比较难搞的算法题了，还是再继续想想这个吧，就抱着一种“这道题搞不出来的话，就总会比其他队缺一个，而且这个肯定比剩下的容易些”的心态。
然后队友出了另一个思路，恰好当时举的几个栗子也都对，于是就先把之前代码打了出来，让她再按这种方式试一试，然后我和另一个队友就开始疯狂找样例，敲完测试的时候，发现了一组错误，改来改去，好像又改回了最初敲的模样。我们又找回第一次代码记录，继续测试，试了大概十几组也没找到特殊情况，于是开始反思是不是思路出了问题.. 直到封榜之后，一直以为其他题都是很难的算法题，剩下的肯定也不太够搞了，就继续找样例吧，结果到最后也没A。

## 赛后
出来之后，和其他人讨论了一路，终于找到了问题，我们没有测试过那么长的，那种情况如果在次数不算太多的时候都是对的，但如果不断移动，越轴并且超过了之前，这种思路得出的结果就是错的了。

回来之后补题，发现H居然就是个裸的优先队列，但是我们看都没看，还有L Floyd，我们也没看，B好像dp也能过，我们也没看，还有K题是hdu原题，我们之前还见过，但是还是没看。

ps:真的是血亏啊，心里真的难受了很久很久，但是想一想，也真的是暴露出了很多问题：
1. 策略问题，最起码在出完水题之后卡题的时候，该把所有题都看一遍，放着三个人这么好的翻译资源不用，结果都压在了一个题上原地转圈，大海捞针找反例。还有取舍，如果真的卡的很厉害，还不如转战一下其他的，最起码不能三个人都压在这里了。当时如果能舍弃C，去看一下其他几个，可能也不见得比这样差。
2. 翻译问题，本是我们队的优势，但是为了题出的快些，看题就变得很快，但是也真的很容易漏掉特殊条件，可以适当慢一点，但是一定要仔细，或者下次可以尝试一个人在敲，另一个人帮看手误的同时也适当再看一下题，一定确保无误。
3. 测试问题，测试样例也一定不要再大海捞针了，漫天撒网测试真的是没有任何意义。一定要尽可能找几个极端或者边界情况，如果都没找到，一定要再考虑下是不是思路问题，不要被固化。

近期计划：
队内每个人每天至少刷一道cf的C题，不做同一道，各做各的。做完之后再互相交流一下今天所做题目和思路。
南京，一定要好好加油！
冲冲冲啊啊啊啊啊啊啊！！！！！！

# end



---

PS. 
