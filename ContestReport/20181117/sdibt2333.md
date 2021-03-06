### Info
* 英文队名 sdibt2333
* 中文队名 飞鸟牡丹配
* 队员1 许梓炯
* 队员2 赖欢
* 队员3 傅钊进

### 比赛地址
http://acm.sdibt.edu.cn/vjudge/contest/view.action?cid=2117#overview

### 做出来的题目

#### F
* 题意
输出Q，R对应P，D在π里边的位置。。。
* 思路
shabi题，看样例就能找到规律，每次输出r和5。

#### H
* 题意
输入26个英文字母对应的摩斯密码和n个词典上的单词。如果每次的k组输入摩斯密码翻译成英文字母刚好能组成词典里有的单词就输出，没有的话输出没办法翻译的第一行摩斯密码。
* 思路
用两个map来对应记录输出。


### 补的题目

#### C
* 题意
手上会有五张牌，双方手中牌级别高的获胜，级别从大到小分别为：
同花顺：手上五张牌都是同种花色，且构成顺子。
四张：手上有四张一样的牌。（不要问为什么没有五张都一样，好好想想）
三带二：五张牌里边有三张一样的，剩下两张也一样。
同花：五张牌都是同一个花色。
顺子：五张牌都是顺序的。（特殊情况：2,3,4,5，A相当于1,2,3,4,5）
三张：五张牌里边有三张一样的，剩下两张与三张都不一样且各自不一样。
两对两张：五张牌里边有两对各自一样的，剩下的一张与这两对都各自不一样。
两张：五张牌里边有一对一样的，剩下的三张与这一对都不一样且各自不一样。
单张：五张牌都各自不一样。
需要注意如果双方手上都有四张相等的牌，那么点数大的获胜。其他情况也同理。如果数量相同的牌点数相同一样，则把牌从散牌里边从大到小比较直到出现一方牌点数比另一方大，获得胜利。
* 思路
把各种情况模拟一遍而已，只不过情况比较多也比较复杂，如果都考虑到了就能过。

#### B
* 题意
飞机到海平面的高度为h，海平面到潜艇的高度为d，飞机与潜艇之间的水平距离为x，n1,n2分别代表水的折射率和空气的折射率。已知，h、d、x、n1、n2，求与θ1互余的角。
* 思路
这道题就是要二分求值，对θ1的角度进行二分，范围在0-90度，所求的角度φ为90-θ1，可以得到公式h*tan(θ2)+d*tan(θ1)=x，关键是求出θ1和θ2的值。

#### E
* 题意
在a,b,c,d四个位置有一个位置是-1，其余的位置上的数大于1小于10000且单调递增。问-1是否能替换成一个数使得整个数列变成等差或者等比。且替换的这个数不大于1000000.
* 思路
按照-1在各个位置的情况讨论是否符合等差或等比且符合条件的情况。注意在a=-1或d=-1的等比的情况下还要注意等比是否能整除。

#### I
* 题意
给你n个单词,给你一个m*m的矩阵表，可以在这表里沿着八个方向找，如果找到了某个单词就输出它

* 思路
dfs
从表里第一个字符开始找，如果和单词的第一个字母相同，那么沿着该字符的八个方向找，如果某个方向的字符等于单词的第二个字母，那么沿着该方向继续找，记住，每沿着一个方向找的时候，都要标记该字符，防止该字符被重复找到。注意，当其中一个字符的八个方向都满足的时候，return 0,让标记过的字符恢复原来的状态。
递归结束的条件即是，所需要钊的单词的下标大于该单词的长度。


