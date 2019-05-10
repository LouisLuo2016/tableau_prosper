这份是一份关于Prosper信用评分增长趋势的tableau可视化分析报告。

### Tableau链接

第一个版本的链接：
[ProsperScore Story 1](https://public.tableau.com/profile/louis4937#!/vizhome/ProsperScoreStory1/ProsperScoreStory1)

最终版本的链接：
[ProsperScore Story 2](https://public.tableau.com/profile/louis4937#!/vizhome/ProsperScoreStory2/ProsperScoreStory1)

### 总结
借助Reinhard Hsu关于Prosper的风险评分分析文章，我分析了持续6年来，prosper借款记录数的增长趋势，以及信用评分和与其相关因素记录数的增长趋势。从分析中，我得出Prosper这种借贷模式正在被越来越多的人接受，人们从开始的趋向于对高信用评分有稳定工作的借款人借贷，发展到可以接受更低的信用评分和多种形式雇佣关系，说明人们对风险的防控降低，更乐于追求更高的收益。

### 设计和分析
对于Prosper的借款数据，我感兴趣的是这些年来，Prosper的不同信用评分增长呈什么样的趋势，以及在不同时期，在同一信用评分下，影响信用评分因素的增长趋势。

#### 1. 借款记录数的增长趋势
我用直线图描绘了这些年Prosper借款记录数的增长趋势， 在年份的时间维度下，prosper的借款记录数每年持续增长，增长最大的年份是2013年，从2009年的2178条持续增长到2013年的35413条，相比2009年，增长了16倍。说明更多的人接受了Prosper这种借贷模式。由于统计数据只有2014年1季度的数据，与2013年全年相比，图上呈现出记录数下降，并不是全年记录数发生了下降。

#### 2. 信用等级借款记录数的增长趋势
在信用等级借款记录数的增长趋势中，我用ProsperScore作为维度查看不同信用评分这些年的增长趋势。开始的2009和2010两年，借款记录数几乎按照信用评分从高到低分布，信用评分越高借到钱的次数越多，这可能也和初期Prosper这种借贷模式被投资者认可的程度低有关，人们更愿意把钱借给信用评分高的用户；2011年和2012年两年4-8的中低评分记录数增长起来，并超过了高评分9的记录数，说明Prosper的借贷模式被投资者认可程度提高，并且投资者更愿意将钱借给中低信用评分的用户以获取更大的收益；2013和2014两年2-4的低评分记录数增长更快，并超过了5-8的中高信用评分记录数，说明越来越多的人参与到Prosper这种借贷模式中，并更青睐高收益低信用评分的借款项目；从整个信用评分借款记录数发展趋势看，人们从开始的谨慎逐步发展到更趋向于承担更大的风险以获取更高的收益。

#### 3. 雇佣状态借款记录数的增长趋势
整体数据分布看，人们更信任有雇佣关系的人，这些人占据了绝大部分记录数。2009到2010年，Full-time类型雇佣关系的记录数要高过Employed，说明此时段借款人更看重贷款人的工作稳定性，更加注重防范风险。在2011年之后，Employed的记录数快速超过了Full-time，大部分的贷款贷给了有雇佣关系的人，不再严格要求是Full-time全职。职业的多样性和人们对风险评判标准有所转变。

#### 4. 雇佣状态持续时间借款记录数增长趋势
由于绝大部分记录数都是有雇佣关系的人产生的，这里的雇佣状态持续时间指的是在雇佣状态下持续的时间。雇佣状态持续时间借款记录数随着整体记录数增长而整体增长，不同持续时间记录数占比并没有太大变化，工作持续时间越短的人越倾向借钱。

#### 5. 借款时间段记录数增长趋势
保持大部分借款发生在正常工作和生活时间，在23点之后到凌晨4点这段时间少量借款分布状况持续增长，23点之后到凌晨4点这段时间借钱的人一般都是财务状况不佳和突发状况的人，这一时间段的记录数持续稳定，没有太大增长，说明经济状况稳定，并没有太多的人发生债务危机。

#### 6. 账期借款记录数增长趋势
贷款人更多贷的是3-5年的长期贷款，2009年和2010年时段内，1年期的贷款几乎没有，从2010年开始，账期更长的5年期贷款出现并持续高速增长。账期越长利息越高，说明借款人更愿意将钱借给利息较高的中长期贷款，而贷款人也更喜欢长期的贷款，用来分摊每月的还款压力。

### 反馈
1. 最初版本记录数的直线趋势图中2014年的记录数发生了大幅度下降，会引起误解，后面增加了对应于季度的记录数趋势图，可以发现是因为2014年只有1季度数据造成。
2. Dashboard中设置直线图和条形图的颜色图例同时应用到两张表，让分类选择一致性。去掉Dashboard中设置的信用评分筛选器，只关注同一纬度下记录数增长趋势。
3. ResultDashboard中信用评分柱状图与趋势展示并没有太大关系，去除这个多余工作表。
4. Result Dashboard中设计的EmployedStatus等饼图体现不出各分类记录数的增长趋势，改用直线图。

### 引用
[数据分析 - 美国金融科技公司Prosper的风险评分分析](https://www.cnblogs.com/msdynax/p/8119912.html)