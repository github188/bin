# 定义1 -- 什么是股票交易体系呢？

  我的理解是，有一个固定或者稳定的标准来决定你买什么股票，同时在买入后同样有一
  个固定或者稳定的标准来决定什么时候卖，能够严格执行这套标准，并且不轻易因几次
  亏损而随便否定、修改它，这就是交易体系。能做到这样炒股的人，我认为即便还没赚
  钱，也在一个正确的方向上。

# 定义2 -- 另一条路上

  有人说，他好比操作系统。更重要的是，你需要为他不断地打补丁。

  本次(2015-06-02)市场调整之后，小指数的走势也会好于大指数，如果上证指数不学深
  成指一样调整指数成分股，那么，它的未来也就是为改革护航，稳定指数重心才是它的
  主要任务。毕竟这个大指数是公众认同度最高的指数之一，在人们的印象中它的涨跌才
  可以论牛熊，包括管理层在内，也都是对它的关照再多些（不能涨太快哦）。而我们`
  市场二元论分析体系`，早就解决了这一矛盾。涨时看领涨、跌时看领跌，是通过大、
  小指数的差异化波动节律，寻找调整持仓偏重的机会。而现在这个问题越发明确，大跌
  之后率先拉起的动力还是小指数，这已经表明了市场主导力量的新锐基金经理们的态度。

# 交易系统

  1 解释过去
  2 预测未来，买入、卖出、买卖多少？
  3 如果市场向相反方向发展，则应该如何处理？
  4 不断重复1~3，循环往复

# 超短线做T -- 策略预埋单

  1 act为基础(+1%空间，40分钟后延时买回)
  2 缠&ac5辅助
    M顶及W底
  3 大盘及板块指数
  4 放弃波动剧烈及不规则的票
  5 关注收盘收敛的个股
——————————————————————————————————————————————————————————————————————————————
> 处理波动

  - oracle(act, ac5...)不能提前买入，只做买入后立即上涨的形态

  0 参考大盘走势
  1 采用合适的级别ma({F5,F30,},{10,20,...})，总有一款合适你
    ma(F5, 5,10,20)的3种情况==》`收敛，向上发散，向下发散` (收敛之后进入新的级别)
    ma(F30,20) 下跌过程中平滑在均线之内的，上涨时表现也会好(缘自大家的约定，宋朝君臣的一盘棋)
    act的卖点，是ac5级别的买点。
    act与ac5的oracle交叉空间即是缓冲地带，上车的机会。
    oracle下单，先从LEVEL2中挑出阻力价位。
  2 水滴原理
    hilo==》-20%涨跌停板时，使用自动策略挂住
    ma(F5, 120)更好的标的+大波动，会得到更加流畅的走势
  3 增加时间参数(铒兵勿食)
    ratio=(argv_c-argv_p)，如此可以得到更加平滑走势
    结合缠论，第一次突破可能是假突破。
  4 股票轮动
    分兵：`以正合，以奇胜。超短可以更加高效(MV=PQ)`
    10:00达到+5%的两种情况：(1) 卖出进行奇正变换；(2) 直接封涨停。只有这样，阻力才是最小的。
    更加灵活的33制组合
    根据时间及空间结合的odds(风险,收益,备选股票池)，决定卖出的仓位
    a 时间空间是非线性的，早上卖出代表更多的机会
    b 早盘封涨停，比尾盘拉涨停成本要高
    c `卖比买贵`：卖了可以再买，可买了立马被锁定
  5 回避心理波动时段
    上行走势 AM09:30~10:30是波动时间，尽量不`卖出`
    下行走势 PM13:45~14:30是波动时间，尽量可`买入`
    严格意义上讲，只有prev交易日大跌，才会在0轴这上出现(2015-06-11石基信息)买点
    买入方面，上午最好只用`5成仓位`，因流利性大，不确定因素多（2015-06-04招行即是一例）
    买入方面，下午13:45后，可满仓抄底
  6 及时买回
    `向上有无限可能，向下只有1个点`
    a 挂自动策略+1%价格买入<锁定30分钟不操作>（卖飞光荣）
    b 挂突破high后买入<锁定30分钟不操作>（恒信移动2015-06-08即有这样的假突破）
    c 采用缠论来给出当时二买二卖

——————————————————————————————————————————————————————————————————————————————
  熊市中周末出利多叫利多出尽，周一多高开低走。
  牛市中`周末`出利空叫利空出尽，所以周一多低开高走；      -- 按时间正态分布
  牛市中真正的短线客买不选周三周四，卖不选周五周一
——————————————————————————————————————————————————————————————————————————————
  股林秘笈：
  早上大跌要买(不割肉)，早上大涨要卖，下午大涨不追，下午大跌次日买，不涨不跌睡大觉！

# 选股--比价淘汰系统

  1 海量每日选股，不漏掉任何机会，易操作的自动化程式是坚持的关键。
    以数据基础、大概率为 Odd Table，佐之以情绪及梦想。

  比价系统：对每日、5日涨票进行统计分类，跟踪

  a 流通是资金的生命，所有选择皆以大换手.大资金为基础
  0 5周换手100%，即25日off_c周期
  1 地量或小量，价格巨跌即为底背驰，放量后上攻
  2 天量或大量，价格不涨即为顶背驰，缩量后下陷
  3 人性善跟风：diff(volume)>0, 更多人认可当前的价格

  很多专业投资者的判断仍是基于事实和数据这两个基本维度，
  而他们参与的这场游戏，却是在情绪的第三维和梦想的第四维上展开的。
  就是说，了解事实是基础，但了解市场情绪，可以做的更好。

# 三套止盈法

  [聊聊交易习惯](http://www.imaibo.net/longweibo/detail/55097b1a9d24b063370000e7)
  1、当股价出现最近10个交易日内最低价时卖出，这是海龟的止盈机制；
  2、当浮盈低于20%时，设置股价回撤10%即卖出；当浮盈大于20%时，浮盈跌去40%即卖出；
  3、股价在20日线上坚决持有，跌破20日线卖出；

# Checklist odds

  一群蝙蝠，不相互触碰，即可成群体智慧
  唯有量化认知，才可以突破感性，跟随ma5
  odds=f(1)+...+f(n)

  0 复利迭代                        # 年线.1年的资金成本在8%，等待即是最大成本
  1 缠之3类买卖点                   #
  2 odds && 梅花5数                 # 不孤注，得乐视
  3 blk                             # cybz sc40 etf180 etf300 上证300成分股
  4 yjbb                            #
  5 acf(cdiff+rdiff+wchng+大盘)     #
  6 turnover                        # tov5 diff(tov5)增 300238.2015-02-09
  7 nmc                             #
  8 big NMC_RATIO(6jian+9jian)      # NMC_RATIO=2 SCREENER 6jian 泰胜风能
  9 big NUM(ma513 ma144)            #
  0 3级别周期鉴定                   # 200% 2次回探更加靠谱
  1 量比tov5/tov5以上升为更大级别   # 2015-03-05 002502 骅威股价
  2 avrg_up .= sharp_up             # *右击时代*, 正在上升且上升不大之票
  3 ma收敛                          # SELECT ma240 -- x_short x_long
  4 下跌不放量，上涨亦不放量        # 
  a 敏捷指导过程管理                # 
  b 定增+增持                       #
  c 定量小步子上涨                  # 克服追涨心理障碍
  d 平台突破.强者恒强.牛市思维      # 
  e 业绩20%复合增长
