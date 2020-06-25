# 作业4: 德州扑克牌型比较

**实现规则: 标准规则**

* 同花大顺（皇家同花顺，Royal Straight Flush）
  同花色的A，K，Q，J和10.
  平手牌：公牌开出同花大顺，则所有未盖牌的牌手平手平分筹码。

* 同花顺（Straight Flush）
  五张同花色的连续数字牌。同时有同花顺时，数字最大者为赢家。
  平手牌：公牌开出同花顺为最大时，则所有未盖牌的牌手平手平分筹码。

* 四条（铁支，Four of a kind）
  其中四张是相同数字的扑克牌，第五张是剩下牌组中最大的一张牌。若有一家以上持有四条（公牌开出四条），则比较第五张牌（起脚牌），最大者为赢家。
  平手牌：公牌开出四条时，最后一张杂牌（或称为kicker、次大牌、踢脚牌，一副牌型组合中剩下来没有用作凑牌型的牌，用于牌型相同时比大小）数字也相同时。

* 葫芦（满堂红，Full house）
  由三张相同数字及任何两张其他相同数字的扑克牌组成，如果同时有多人拿到葫芦，三张相同数字中数字较大者为赢家。如果三张牌都一样，则再比两张牌中数字较大者赢家。
  平手牌：五张牌数字都一样，则平分彩池。

* 同花（Flush）
  此牌由五张不按顺序但相同花色的扑克牌组成，如果不止一人有此牌组，则牌面数字最大的人赢得该局，如果最大数字相同，则由第二、第三、第四或者第五张牌来决定胜负。
  平手牌：公牌的同花就是最大的同花牌型时，平分彩池。

* 顺子（Straight）
  此牌由五张连续数字扑克牌组成，如果不止一人有此牌组，则五张牌中数字最大的赢得此局，10-J-Q-K-A为最大的顺子，A-2-3-4-5为最小的顺子。
  平手牌：如果五张牌数字都相同，平分彩池。

* 三条（Three of a kind）
  由三张相同数字和两张不同数字的扑克牌组成，如果不止一人有此牌组，则三张牌中数字者最大赢得该局，如果三张牌数字大小相同，则比较不同点数的两张牌中数字较大者，若相同时再比第五张，数字大的人赢。
  平手牌：如果五张牌数字都相同，则平分彩池。

* 两对（Two pair）
  两对数字相同但两两不同的扑克和一张杂牌组成，共五张牌。
  平手牌：如果不止一人持有此牌型，持有数字比较大的对子者为赢家，若较大数字对子相同，则比较小对子的数字，如果两对对子数字都相同，那么第五张牌（kicker）数字较大者赢。如果连第五张牌数字也相同，则平分彩池。

* 一对（One pair）
  由两张相同数字的扑克牌和另三张无法组成牌型的杂牌组成。
  平手牌：如果不止一人持有此牌型，则持有较大数字对子者为赢家，如果对牌数字相同，则依序比较剩下的三张牌，数字最大者为赢家，如果五张牌都一样，则平分彩池。

* 散牌（高牌, High card，No-pair，Zitch）
  无法组成以上任一牌型的杂牌。
  平手牌：如果不止一人抓到此牌，则比较数字最大者，如果数字最大的相同，则依序比较第二、第三、第四和第五大的，如果五张牌都相同，则平分彩池。

## 输入格式

Heart : H, Spade : S, Club : C, Diamond : D

2 : 2, 3 : 3, 4 : 4, 5 : 5, 6 : 6, 7 : 7, 8 : 8, 9 : 9, 10 : T, 11 : J, 12 : Q, 13 : K, 14 : A

```
Black:2H,5D,3C,TS,AS White:5S,6S,7S,8S,9S
```



