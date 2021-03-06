Finished at 2018.10.29.

[Domingos P](https://homes.cs.washington.edu/~pedrod/). The Master Algorithm[J]. 2015. 

2015 年美国出版，2016年有中文译本，2017.01 中文出版，滞后了两年时间的知识。还是要关注国际趋势，留意新动向。

机器学习可谓是百家争验，本书介绍的五个学派符号学派、连结学派、进化学派、贝叶斯学派和类推学派，在历史长河中都曾经或仍在辉煌，总能找到现实的影子。作者通过「终极算法」这个目标将各个学派柔和到了一起，从更高的层次寻找算法间的共性和契合点。从低层次来说，我们可以更深入更全面的了解各个学派的发展、兴衰和优缺点，从更高层次来说，我们可以试图取长补短融合或创造出更强大的终极算法。从实际应用场景来看，很多复杂问题难以通过单一算法来解决，对终极算法存在强烈需求。我个人倒是欣于寻找这样的终极算法，并且从直觉上告诉我现在的ensemble算法正是终极算法的雏形。

看书过程中有一个感触，作者的比喻有些时候很难理解，不知道是否源于思想差异，还是自己功力尚浅。本书给我带来的更多是层次化、体系化和全面化的思想，外加一些新思想的惊喜。

#### 目录

- [机器学习革命](#01)。首先介绍了机器学习算法和传统计算机算法的不同。计算机：输入 + 算法 --> 输出；机器学习：输入 + 输出 --> 算法。然后从商业、科学以及未来走向等角度介绍了机器学习革命已到来，并逐渐成为不可或缺的能量，驱动着各领域发展。
- [终极算法](#02)。首先通过神经科学、进化论、物理学、统计学、计算机科学的角度来论证“通用方法可归结为发现宇宙最深层的规律”。从不同角度论述单模型的不足以及其由此带来的挑战：黑天鹅事件的无法性；需要取长补短得到更好的方法；单一或部分数据很难反映整体；获取完整的数据或知识几乎不可能；可选的记忆、微处理器和或非门是未达标准的终极算法候选项。由此引出 5 大学派：符号学派、联结学派、进化学派、贝叶斯学派、类推学派。
- [符号学派：休谟的归纳问题](#03)。理想主义和经验主义之间的博弈，而符号学是经验主义的推崇对象。作者先以“约不约”为例，介绍机器学习问题以及学习过程中泛化能力的重要性。介绍并论述“天下没有免费的午餐”定理。由对知识泵进行预设引出“合取概念”。除了从经验中归纳出规则以外，还要把握准确度。作者由演绎引出符号学派中核心的优化算法逆向演绎，即从众多事实中归纳出一般规则。通过治愈癌症，20问游戏进一步论述逆向演绎的流程。最后引出并介绍符号学派，核心概念为所有和智力相关的工作都可以归结为对符号的操纵。
- [联结学派：大脑如何学习](#04)。联结主义相信知识储存在神经元之间的联结关系之中。感知器被提出，然而因为只能学习线性函数的限制而导致神经网络沉寂大约 15 年。后来物理学家，霍普菲尔德发现了大脑和自旋玻璃（spinglass）惊人的相似之处，由此启发他确定了第一种神经网络。后来杰夫·辛顿等人将以上神经网络的计算改成概率驱动了，接下来的几十年里，辛顿全身心投入到神经网络的研究中，比任何人付出都多。深度介绍了世界上最重要的曲线—S 型曲线、又称逻辑函数、S 型函数。介绍反向传播算法、梯度上升。最后迎来多层感知机的复兴。后来的几大突破包括自动编码器、玻尔兹曼机器、卷积神经网络。
- [进化学派：自然的学习算法](#05)。由达尔文的进化算法引入。介绍探索：利用困境，由此介绍遗传算法的特点，基于某种规则进行遗传选择。程序的适则生存法则，介绍了遗传算法的几个 milestone，早起研究团队主要由约翰·霍兰德和他的学生组成。但最终由于“性”在遗传算法中的不解之谜而使其备受冷落。演化新论者和联结学派之间的博弈，演化新论可以学习架构然后交由联结学派完成参数学习。最后论述谁学的最快，谁就会赢。
- [贝叶斯学派：在贝叶斯教堂里](#06)贝叶斯第一个描述用新方法来考虑概率，在50年后，皮埃尓-西蒙·拉普拉斯（最伟大的数学家之一）创造了贝叶斯定理。**先验概率** vs. **后验概率**，问题的关键是，随着你看到的证据越来越多，后验概率应该如何演变，答案就是在贝叶斯定理里面。—— 贝叶斯定理：P(结果|原因)=P(原因|结果)P(结果)/P(原因)。所有模型都是错的，但有些却有用，通过条件独立性的假设来规避组合爆炸问题。从《尤金·奥涅金》到 Siri，HMM的成功应用。所有东西都有关联，但不是直接关联——贝叶斯网络。推理问题的求解存在计算难的问题，因此大多时候采用的是近似计算，最受青睐的算法是MCMC (Markov chain Monte Carlo)。值得注意的是，在贝叶斯定理中，概率是包含主观程度的信任。贝叶斯学派的观点是，选择什么表示方法由你决定，但得利用贝叶斯定理来掌握它。20 世纪 90 年代，他们声势浩大地接管了 NIPS。符号学派 vs. 贝叶斯定理。
- [类推学派：像什么就是什么](#07)。类比是推动许多历史上最伟大科学进步的动力。最近邻算法是人类有史以来发明的最简单、最快速的学习算法，同时最近邻算法是史上第一个能够利用不限数量的数据来掌握任意复杂概念的算法，基于此优化的有 k 最近邻算法、加权k最近邻算法等。难以规避的「维数灾难」，去掉无关维度、属性选择、弱相关性的处理。直到 20 世纪 90 年代，应用范围最广泛的类比学习算法就是最近邻算法，但后来被来自其他学派更引人注目的“表亲”夺去光芒。当时一种新的以相似性为基础的算法横空出世了，横扫之前的所有算法。它就是支持向量机（Support vector machines, SVM），求解方法为约束优化。类比推理中的两大子问题：相似度函数、基于相似性由旧推新。符号学派 vs. 类推学派。
- [无师自通](#08)。聚类和维度简化。聚类，k-means：物以类聚，人以群分，可以通过期望最大化演算法（Expectation Maximization, EM 算法）来优化。维度简化，线性 vs. 非线性，PCA。
- [揭开迷惑](#09)。终极算法的雏形，ensemble 算法。“堆叠”，“袋装”，“推进”。
- [建立在机器学习之上的世界](#10)。拥抱机器学习变革。


<h4 id="01"> 机器学习革命 </h4>

- Introduction:
	- “如果我无法创造某样东西，那么也就无法理解它”——理查德·费曼
	- 在科学的任何领域，如果某个理论无法用算法表示，那么它就不是很严谨（更别提你无法用计算机来解决这个问题，因为你能让计算机替你做的事实在太有限）。
	- 程序员（创造算法并将其编码的人）是一个“小神灵”，能任意创造不同的世界。
	- 复杂性怪兽：空间复杂性、时间复杂性和人类的复杂性。
- 学习算法入门
	- 流程差异：
		- 计算机：输入 + 算法 --> 输出
		- 机器学习：输入 + 输出 --> 算法
	- 不需要畏惧，因为编写算法需要智力、创造力、问题解决能力，这些都是机器没有的。   
	- 几种联系：
		- 数据是养料、机器学习是一把剑
		- 知识 ～ 统计，技能～程序
		- 计算机科学 ～ 准确思维，机器学习～统计思维 
- 为何商业拥护机器学习
	- 谷歌的点击率预估为什么比雅虎的有价值？市场价值是巨大差异背后的主因：谷歌年收入 500 亿美元，点击率每提升 1% 就能为公司带来每年额外利润 5 亿。
	- 公司不断壮大后要经历的三个阶段：
		1. 所有事都由人工完成；
		2. 最辛苦的时期，公司变得越来越大，需要用到计算机；
		3. 没有足够的程序员和顾问满足公司的需要，因此公司不可避免地向机器学习寻求帮助。（amazon, facebook）
	- 学习算法是“媒人”，客服信息过载。学习算法并不是完美的，决定的最后一步通常还得由人来做，但学习算法很智能，为人们减少了需要做的选择。最好的选择权仍在你手里——从算法给你展示的所有选项中挑选，但99.9%的选择由算法做出。
	- 现有鸡还是先有蛋：
		- 谁有最佳算法、数据最多，谁就能赢
		- 谁有最多的用户，谁就能积累最多的数据，谁有最多的数据，谁就能学到最好的模型，谁学到最好的模型，谁就能吸引最多的用户，这是一个良性循环（如果你在竞争，就会变成恶性循环）。
	- 现状
		- 数据的饱和点还没有出现，长尾效应持续起作用。“数据是新型石油”，业界将数据看作战略资产。
		- 机器学习是很棒的新技术，但这并不是商业界用户它的原因——真正的原因是别无选择。      
- 给科学方法增压
	- 科学：产生假设、验证、放弃或完善；机器学习使科学的发现过程自动化。
	- 科学的每个领域都需要足够的数据才能取得进步；好消息——之前缺乏数据的学科现在拥有很多数据；但如果数据不能变成知识则毫无用处；机器学习是大海捞针的利器（科学分支越来越细，知识太多难以甚至无法整合，组合爆炸）。 
- 10 亿个比尔·克林顿
	- 2012 年机器学习决定了谁能当上总统。
	- 决定总统选举的因素包括：经济、候选人的亲民度等，但这些因素没有起到作用，而选举的结果受到几个“摇摆州”的影响。
	- 选举是机缘巧合。机器学习的作用就是，让每位选民都觉得克林顿对待他们亲力亲为、非常用心。
- 学习算法与国家安全
	- 每天美国国家安全局窃听着全球10亿多个通话，还有其他通信；
	- 将机器人与事件连接起来，这些事件单个看起来并无危害，但集中起来可能就预示着不详。（可能可以阻止9·11事件的发生）。
	- 机器学习与博弈论相结合：别只想着打击对手当前想做的事，要学会巧妙地回避对手对你的学习算法的损害。
- 我们将走向何方
	- 突破 
		- 在金融领域：预测股票的起伏波动，直接营销、客户关系管理、资信评分以及诈骗侦查等领域；网络和电商：搜索、广告；国家安全：打击恐怖主义战争；社交网络。
	- 困难：
		- 在工业上起作用的学习算法的生成还是受到了很大限制。
	- 比尔·盖茨说机器学习的突破产生的价值将相当于10家微软，说得保守了。  

<h4 id="02"> 终极算法 </h4>

实际上，大量的机器学习应用仅仅由几个算法来负责。例如朴素贝叶斯算法，最近邻算法，决策树算法。  
如果你为学习算法提供足够、适当的数据，该算法可以实现任一功能。但值得注意的是**足够数据**也可能是无限的。  
发现一种通用的学习算法可归结为发现宇宙最深层的规律，然而，这并不意味着通用的学习算法要和专用算法一样高效。  
中心假设——**所有知识，无论是过去的、现在的还是未来的，都有可能通过单个通用学习算法来从数据中获得**。

- **来自神经科学的论证**   
	对于天生开不见的人，视觉皮层可以负责大脑和其他功能。对于听不见的人，听觉皮层也可以这么做。 
- **来自进化论的论证**  
	生物多样性源于单一机制：自然选择。值得注意的是，计算机科学家对该机制非常熟悉：我们通过反复研究尝试许多备选方法来解决问题，选择并改进最优方案，并尽可能多地尝试这些步骤。
- **来自物理学的论证**  
	在物理学中，适用于不同数量的方程，往往可以用来描述发生在不同领域的现象，例如量子力学、电磁学、流体动力学。波动方程、扩散方程、柏松方程表明：一旦我们在某个领域发现它们，也很快能在其领域发现它们；一旦我们在某个领域懂得解开它们，也能在所有领域将它们解开。 
- **来自统计学的论证**  
	根据一个统计学派的观点，所有形式的学习都是基于一个简单的公式——如我们所知，就是贝叶斯定理。贝叶斯定理会告诉你，每当你看到新的证据后，如何更新你的想法。
- **来自计算机科学的论证**  
	 如果我能能解决任意一个 NP 问题，那么 P=NP。人工智能的其中一个定义是，人工智能包括找到NP完全问题的所有启性解决方案。
- **机器学习算法与知识工程师**
	- 反对者1——知识工程师（最大的敌人），明斯基
	- 反对者2——语言学家，诺姆·乔姆斯基
	- 反对者3——心理学家，杰瑞·福多
- **天鹅咬了机器人**
	- “无论你的算法多么聪明，总会有它无法掌握的东西。”
	- 机器学习首先要区别可预测的事与不可预测的事。
	- 反对者——“数据无法代替人类直觉”。这句话应该反过来说，要依靠数据而不是与之斗争。 
	- 反对者——“机器学习能从数据中找到规律，但它绝不会发现更深刻的东西，如牛顿定律”。但深刻的科学真理并不是那么容易就能获得，科学历经了三个时期：布拉赫时期、开普勒时期、牛顿时期。
- **终极算法是狐狸，还是刺猬**
	- 这可能是反对终极算法观点中最严肃的一个。
	- 对多个算法，求同存异，取长补短，或许就能得到终极算法。 
	- 当今学习算法最大的问题，不是它们数量太多，而是尽管它们有用，却不能完成我们让它们做的所有事情。我们利用机器学习来发现深刻的真理之前，得先找到关于机器学习的深刻真理。
- **我们正面临什么危机**
	- 单中药不能治疗癌症。
	- 数据记录了我们的每一个印记，但我们应该如何充分利用这些数据呢？
	- 我们要担心的是，它们服务我们的方法可能会对我们有害，而不是有益。 
- **新的万有理论**
	- 机器学习所做的，就是从数据中引出理论。
	- 首先明白什么是科学理论，什么不是。
	- 理论强大之处在于它简化了我们对世界的描述。
	- 我们可以做得更好的两个原因：
		1. 实际上，我们没有足够的数据来完全确定世界，甚至忽略不确定性原则；
		2. 虽然我们在某个时间点拥有关于世界的完整知识，物理定律还是不能让我们确定这个世界的过去和未来。
	- “人们一开始认为这太困难，于是放弃了，直到一个孤独的天才解决了这个问题”——真理往往掌握在少数人手里。  
- **未达标准的终极算法候选项**
	- 第一个候选项——记忆 
		- 对于未来你可能看到的事物，你现在看到的也只是一小部分。
		- 只会记忆的机器会陷入瘫痪。 
	- 第二个候选项——微处理器
		- 最好的硬件应该是特定用途集成电路
	- 第三个候选——或非门
		- 这不是终极算法，就像乐高砖不是万能玩具一样  
- **机器学习的五大学派**
	- 进化学派、进化结构、遗传编程
	- 联结学派、学习参数、反向传播
	- 符号学派、组成动态中的元素、逆向演绎
	- 贝叶斯学派、权衡证据、贝叶斯定理
	- 类推学派、映射到新的情形中、支持向量机

<h4 id="03"> 符号学派：休谟的归纳问题 </h4>

- 前言：理性主义 vs. 经验主义
    - 理性主义：喜欢在迈出第一步前，就提前规划好一切
        - 理论家和知识工程  
        - 早期：柏拉图
        - 代表：笛卡尔、斯宾诺莎、莱布尼茨
    - 经验主义：喜欢尝试新鲜事物，然后看看结果会怎样
        - 黑客和计算机学者 
        - 早期：亚里士多德
        - 代表：洛克、贝克莱、休谟
        - 大卫·休谟是最伟大的经验主义者，以及有史以来最伟大、以英语为母语的哲学家，可以说他是符号学派的守护神。
- **约不约**
    - 通过例子来介绍机器学习问题以及学习过程中泛化能力的重要性。
    - 例子：通过约会记录来预测某人是否会答应当下的约会。
    - 这是一个机器学习问题：将结果推广到我们没有见过的事件中。
    - 泛化能力：我们不可能预先知道所有的可能性，因此必须懂得一般化。 
- **“天下没有免费的午餐”定理**
    - 休谟提出爆炸问题之后的 250 年, David Wolpert 赋予了这个问题优雅的数学形式。Wolpert 原来是一名物理学家，后来成为机器学习者。他的研究成果被人们称为“天下没有免费的午餐”定理，**规定“怎样才算是好的学习算法”。这个规定要求很低：没有哪个学习算法可以比得上随意猜测**。
    - 我们不关心所有可能存在的世界，而只关心我们生存的这个世界。
    - “天下没有免费的午餐”这个实际的结论表明，**不靠知识进行学习，这样的事情不存在**。
    - 数学家认为机器学习是一个 **ill-posed problem**：这个问题没有唯一解，解此问题的唯一方法就是引入附加假设。
    - Tom Mitchell 是典型的符号学者，称机器学习体现“无**偏见**学习的无用性”。
    - 亚里士多德曾经说过，在知识领域，没有什么东西不是首先凭借感觉来形成的。莱布尼茨又加了一句，“除了知识本身”。
    - 就像进化过程一样，机器学习不是时时刻刻都知道自己是否可以准确无误地运行。
    - 我们一旦掌握新的知识，基于前面的步骤，就可以得出更多的知识。唯一的问题就是，从哪里开始。
- **对知识泵进行预设**
    - 我们见过的所有真实的东西，在宇宙中也是真实的。
    - 牛顿法则是机器学习的第一个不成文的规则。我们归纳自己能力范围内、应用最广泛的规则，只有在数据的迫使下，才缩小规则的应用范围。
    - 如何从原始数据中找出规律。标准的解决方法就是假设我们知道真理的形式，而算法的任务就是把这个形式具体化。
    - 如果所有两个因素的预测都失败了，你可以尝试任意个数因素的组合，机器学习者和心理学家称之为**“合取概念”（conjunctive concept）**。 托尔斯泰在写《安娜·卡列尼娜》的开篇时，出现在他脑海里的就是合取概念：“所有幸福的家庭都是相似的，每个不幸的家庭各有各的不幸”。
    - 首先做有条件的假设，如果这样无法解释数据，再放松假设的条件，这是典型的机器学习。但现在的问题是，**合取的概念太多，没有足够的时间逐个尝试**。
    - 这里有一个方法：暂且假设每个配对都合适，然后排除所有不含某品质的搭配，对每种品质重复同样的做法。最后你可以丢掉数据，然后只留下这个定义。
- **如何征服世界**
    - 我们要做的就是学习经过一系列规则定义的概念，而不仅仅是单个规则。
    - 利用我们之前见过的算法来学习合取概念。我们学习每个规则之后，会排出该规则包含的正面例子。 
- **在无知与幻觉之间**
    - 拥有完美记忆力看起来非常幸运呢，但其实它是可怕的诅咒。
    - 过拟合，无法避免，论文最多。学习意味着将细节遗忘，只记住重要部分。
    - 对噪音/细节的关注会让你无法找到整套规律。
    - 组合爆炸。当你有过多假设，而没有足够的数据将这些假设区分开来时，过拟合就发生了。坏消息是，即便对最简单的合取概念算法来说，假设的数量也会随着属性的增多而呈指数级增长。
    - 学习是数据量和假设数量之间的较量。 
- **你能信任的准确度**
    - 如何验证你的算法：爱因斯坦的广义相对论也只是在亚瑟·爱丁顿对其证实之后才广泛被人们接受。但你也不必等待新数据的到来，你可以将已有的数据集分成**训练集和测试集**来用。**对于机器学习来说，对不可见数据的测试是必不可少的，因为这是判断学习算法过拟合的唯一方法。**
    - 知道何时过拟合还不够，我们需要第一时间避免过拟合。这就意味着不再对数据进行完全拟合，可以运用**统计显著性检验**来确保我们看到的模型真实可靠。显著性检验是决定一项研究结果是否值得出版的“黄金标准”。
    - 另一个流行的方法是**选择更加简单的假设**，著名的 ocam's razor 原理。
    - 如果你的学习算法检测集准确度不尽如人意，那就要诊断问题在哪。**variance vs. bias**。 
- **归纳是逆向演绎**
    - 主算法应该能以大量的知识作为启动。
    - 演绎：一般 ---> 特殊
    - 逆向演绎：众多事实 ---> 一般
- **掌握治愈癌症的方法**
    - 逆向演绎是在生物学中发现新知识的重要方法，这也是治愈癌症要迈出的第一步。
    - 治愈癌症意味着在不破坏完好细胞的情况下，阻止受损细胞的繁殖。这就需要知道完好细胞和受损细胞的区别在哪里，特别是它们染色体组的区别在哪里。
    - 掌握哪种药物对哪种变异有效，这需要关于患者的数据库、他们的癌基因、服用过的药物以及药效。最简单的规则**对基因与药物之间一对一的对应关系进行编码**。 
- **20 问游戏**
    - 逆向演绎的另外一个局限性在于，它涉及很密集的计算，因此很难扩展到海量数据集中。因此，符号学家选择的算法是**决策树归纳**。
    - 有一个突出的问题——如何挑选最佳属性以便在节点处进行预测。方法：熵。
    - 防止过拟合的方法：显著性检验和针对树的大小设定惩罚制度。
    - 在机器学习领域，决策树源于心理学方面的知识。
    - 决策树是应用最为广泛的方法，因为其具有以下优点：易于理解、快速掌握、通常无需太多调整就可以得到准确无误。
    - 昆兰石符号学派中最卓越的研究者——决策树。
    - 应用：微软的 Kitnet. 
- **符号学派**
    - **核心概念：所有和智力相关的工作都可以归结为对符号的操纵**。
    - 知识的交易：（1）手动输入的知识，供学习算法使用；（2）归纳得出的知识，用来加入知识库中。
    - 符号主义是通往终极算法最短的路程。
    - 逆向演绎就像是一个超级科学家，系统查看论据，思考可行的归纳法，整理最有利的证据，然后将这些和其他论据一起，进一步提出假设——所有过程都基于计算机的速度。
    - 逆向演绎的缺点：归纳法数量广泛、容易被噪音迷惑。
    - 联结学派对符号学派尤其不满。 

<h4 id="04"> 联结学派：大脑如何学习 </h4>

- 前言：
    - 联结主义相信知识储存在神经元之间的联结关系之中。
    - 符号学派 vs. 联结学派
        - 前者：符号和它们代表的概念之间有一一对应的关系；后者：代表方式是分散式的，每个概念由许多神经元来表示。
        - 前者：按次序的；后者：平行的。
    - 计算机晶体管的数量已经赶上人类大脑里神经元的数量，但在连接数量上，人类的大脑轻易获胜。
    - 实际上，目前计算机和人脑相比，主要的限制是能量损耗。  
- **感知器的兴盛与衰亡** 
    - 第一个正式的神经元模型由 Warren McCulloch 和 Walter Pitts 于 1943 年提出，看起来像是组成计算机的逻辑门。
    - 感知器于 20 世纪 50 年代由康奈尔大学的心理学家 Frank Rosenblatt 发明。Rosenblatt 在早期机器学习领域形成的过程中，比任何人付出的都要多。“感知器”这个名称源于他的兴趣，他喜欢将自己的模型应用到诸如演讲和字符识别的感知任务中。
    - 祖母细胞。
    - 感知器碰壁：只能学习线性边界。具有讽刺意味的是，马文·明斯基的博士论文和神经网络相关，但对于神经网络他越来越不包幻想。1969 和他的同事还专门出了一本书《感知器》，详细介绍了同名算法的缺陷。对 XOR 没有学习能力是经典的案例。
    - 尽管明斯基和派普特承认，几层相互连接的神经元能做的应该更多，但他们找不到研究这些神经元的方法，其他人也找不到。
    - 神经网络开始沉寂（大约 15 年）。
- **物理学家用玻璃制作大脑**
    - 1982 年，霍普菲尔德发现了大脑和自旋玻璃（spinglass）惊人的相似之处，自旋玻璃是深受统计物理学家喜爱的特殊材料。这引起了联结学派的复兴。霍普菲尔德注意到自旋玻璃和神经网络之间有趣的相似点：一个电子的自旋对其相邻电子的活动所做的反映和一个神经元的反映十分相似。在电子的情况中，如果相邻电子的加权和超过界限值，电子就会向上翻，反之则向下翻。**受这一点的启发，他确定了第一种神经网络**。
    - 但自旋玻璃仍然是大脑的一个不现实的模型：（1）对于一个电子来说，自旋相互作用是对称的，而大脑中神经元之间的连接却不是对称的；（2）霍普菲尔德的模型忽略了另一个大问题就是，真正的神经元是和统计相关的。
    - 1985 年，大卫·艾克利、杰夫·辛顿、特里·索诺斯基把霍普菲尔德网络里的确定性神经元用可能性神经元代替。这一概率由著名的热力学中的玻尔兹曼分布得出，因此他们称自己的网络为玻尔兹曼机器。
    - 杰夫·辛顿在接下来的几十年继续在玻尔兹曼机中尝试了许多变量。为了了解大脑如何运转，他比任何人付出的时间、精力都要多。
- **世界上最重要的曲线**
    - S 型曲线、又称逻辑函数、S 型函数 
    - S 型是所有种类相变的形状
    - 宇宙就是相变的巨大集合体，从宇宙到微观世界，从世俗到人生的改变
    - 我们认为是线性的现象，其实都是 S 形曲线，因为没有什么能够毫无限制的增长下去。
- **攀登超空间里的高峰**
    - 在感知器算法中，错误信号要么是全有，要么是全无。
    - 反向传播算法、梯度上升。
    - 全局最低值隐藏在浩瀚的超空间的某个角落里，找到它就走运了。这也是明斯基、派普特和其他人无法找到学习多层感知器的部分原因。他们可能想象到用 S 形曲线来代替阶跃函数，然后进行梯度下降，不过他们会遇到误差的局部最小值这个问题。在那个年代，研究者们不相信计算机模拟，他们需要数学来证明算法可以起作用，而反向传播却没有这样的证据。
    - 我们需要意识到，多数情况下局部最小值挺好的，不会有不良影响。实际上，局部最小值可能更合适，因为它和全局最小值比，不太可能证明对我们的数据过拟合。
    - 超空间是一把双刃剑：一方面，空间的维度越高，它越有可能存在高度复杂的表面和局部最优解；另一方面，被困在局部最优解中，意味着被困在每个维度中，所以被困在多维中的难度会比困在三维中的难度大。
    - 要当心，不要过于重视反向传播找到权值的意义。记住，可能会有许多不同的优良权值。
    - S 形曲线是线性函数非智性和阶跃函数难解性的完美中专站。 
- **感知器的复仇**
    - 多层感知机
    - 第一次最大成功：准确预测股票市场，然后以惊人速度进入对冲基金。
    - 另一个成功：掌握驾车技术。
    - 今天越来越多的成功。 
- **一个完整的细胞模型**
    - 符号学派：构建复杂，组合爆炸
    - 联结学派：反向传播很适合解决复杂网络问题，因为他能够有效掌握非线性函数。但信息缺失是不可避免的矛盾，要掌握有用的模型就需要利用贝叶斯方法。 
- **大脑的更深处**
    - 再度沉寂：网络变深后很难学习。（20世纪90年代中期，只有一些中坚力量还在坚持）
    - 如今再度兴起：计算机变快了，数据变的更大了。辛顿和其他人答道：确实，我们一直都没错！
    - 联结学派实质性的进步：
        - 自动编码器：20 世纪 80 年代为人所知，虽然只有一个单个隐藏层，但它很难学习。后来花了十余年来寻找诀窍：（1）让隐藏层比输入层和输出层大一些；（2）在任何特定时间，只把几个隐藏的单位赶走。---> 稀疏自编码器 ---> 叠加自动编码器。
        - 玻尔兹曼机器作为基础的延展
        - 以视皮质模型作为基础的卷积神经网络。 

<h4 id="05"> 进化学派：自然的学习算法 </h4>

- 前言：机器人公园
- **达尔文的算法**
    - 传承：达尔文 ---> 亚瑟·伯克斯，冯·诺伊曼 ---> 约翰·霍兰德（开始研究的是神经网络，他的兴趣使情况发生转变）。
    - 随着霍兰德的创作渐渐为人所知，遗传算法的关键输入是一个**适应度函数**。开始，是一群适应力不那么强的个体，遗传算法得找出变量，然后这些变量依据适应度而被选择。变量，无论在 DNA（4个基本组成单位）序列中，还是在位串中，都可以通过集中方法产生。比如**交叉**、**突变**。对于霍兰德来说，遗传算法的真正威力在于更复杂的东西：**性**。
    - 1972 年，尼尔斯·埃尔德雷奇和史蒂芬·杰伊·古尔德提出**进化过程由一系列“间断平衡”组成，长期的停滞与短暂的快速变化相互交替**。一旦算法达到适应度的局部最大值（适应度中的峰值），算法会在这一点停很长时间，直到某次幸运的变异或者交叉，让处于坡上的个体等到更高的峰顶，在这一点上该个体会进行大量繁殖，然后和过往的每一代来爬上这个坡。 
- **探索：利用困境**
    - 反向传播 vs. 遗传算法：
        - 反向传播：在任何给定时间坚持单一假设，而且这个假设会渐渐改变，直到其适应某个局部最优值；
        - 遗传算法：在每一步中考虑整个群体的假设，而由于交叉行为，这些假设可以从这一代跨到下一代。
    - 遗传算法的特点：
        - 陷入局部最优值困境的可能性较小，而且原则上可以找到更新颖的东西，但遗传算法分析起来也要难得多。（与反向传播对比）；
        - 指数空间，“基模”，使得算法更高效；适应度更高的基模会主导群体。
    - 探索——利用困境：老虎机，继续尝试还是选择当前最优？遗传算法就像一群赌徒中的元凶，同时在市里的每个赌场玩老虎机。依据最优策略：以成倍增长的频率去玩看起来赢得越来越多的机器。   
- **程序的适者生存法则**
    - 在开始的几十年，遗传算法的阵营主要由约翰·霍兰德和他的学生组成。
    - milestone：
        - 1983，遗传算法解决的最大问题是学会控制天然气管道系统；
        - 1985，第一次会议
        - 1987，约翰·科扎发明“遗传编程”，以树的结构来表示（在飞机上恍然大悟）。遗传编程器的适应度 = accuracy + complexity
        - 1995，遗传变成的第一次成功，也就是成功设计了电子电路
        - 2005，美国专利及商标为一项专利颁奖，该专利根据遗传算法设计，是工厂的优化系统。
- **性有何用**
    - 尽管他们取得了成功，也对诸如渐进主义与间断平衡的问题发表见解，但**遗传算法还有一个很大的谜团没有解开：性在进化过程中所起的作用**。霍兰德没有哪个理论结果表明，交叉行为能起作用，能够保持群体中的多样性。
    - 消除性别对演化新论者来说，就只剩下变异作为其理论的推动力。
    - 没有人知道为什么性在自然界中无处不在。人们已经提出几个理论，但没有一个被广泛接受。
    - 为了回应越来越多的批评者，科扎 1992 年的书《遗传编程》包含的实验表明，遗传编程在布尔电路合成问题上打败了随机生成备选项，但胜利的优势很小。
    - 接着 1995 年 ICML 上，凯文·朗发表了一篇论文，表明爬山法在相同问题上打败了遗传算法，而且胜利的优势很大。科扎和其他演化新论者已经不断尝试 ICML，但总是因为经验验证不足而被拒。
    - 论文被拒和朗的论文让科扎气急败坏，他以 ICML 的两栏格式，整理了一篇 23 页的论文，反驳朗的结论。
    - 随之，遗传编程员开始举办自己的会议，这些会议与遗传算法会议合并，成为“遗传与进化计算会议”（GECCO）。对于演化新论者这部分，机器学习主流学派已经很大程度上把他们忘记。这是一个悲伤的结局，但在历史上并不是第一次，性是决裂的原因。
- **先天与后天**
    - 演化新论者和联结学派重要的共同点：他们都因为收到自然启发而设计了学习算，不过后来分道扬镳了。 
    - 先天：演化新论者关注的是**学习架构**，通过参数优化来对演化的架构进行微调是次要的事情。
    - 后天：联结学派更喜欢用一个简单、手工编写的结构，加上许多连接行为，然后让**权值学习**来完成所有工作。 
    - 先天与后天之争中，两方都没有完整的答案，关键在于找到如何将两方结合起来。终极算法既不是遗传编程，也不是反向传播，但它得包含这两者的重要部分：结构学习和权值学习。
- **谁学的最快，谁就会赢**
    - 进化寻求好的结构，而神经学习则填满这些结构：这样的结合是我们走向终极算法最简单的一步。
    - “自然”对计算机来说就是它运行的程序，而“人工”则是获取的数据。“这两个哪个重要”这样的问题明显有点荒唐。
    - 你也许会想，都到这点了，为什么我们还没有完成目标呢？（1）目前我们只是大概知道自然如何学习，对许多应用来说已经足够，但对于真实的东西来说，还只是灰蒙蒙的影子；（2）即使已经弄明白自然如何学习，我们也不会满足。一方面，这个过程太缓慢，另一边是更加智能的软件。
    - 与联结学派及演化新论者相反，符号学派和贝叶斯学派不相信“法自然”的说法。他们想从基本原理中找出学习算法该做什么，而且也包括我们人类。 

<h4 id="06"> 贝叶斯学派：在贝叶斯教堂里 </h4>

- **统治世界的定理**
    - **贝叶斯**是一位 18 世纪的英国牧师，他是第一个描述用新方法来考虑概率的牧师。而贝叶斯主义是由**皮埃尓-西蒙·拉普拉斯**（最伟大的数学家之一）创作的，他是比贝叶斯晚生 50 年的法国人，他把想法变成了定理并以贝叶斯定理命名。
    - 贝叶斯定理不仅仅是一个简单的规则，当你收到新的论据时，它用来改变你对某个假设的信任度：如果论据和假设一致，假设成立的概率上升，反之则下降。 
    - 对于贝叶斯学派来说，学习“仅仅是”贝叶斯定理的另外一个运用，将所有模型当作假设，将数据作为论据：随着你看到的数据越来越多，有些模型会变得越来越有可能性，而有些则相反，直到理想的模型渐渐突出，成为最终的胜者。
    - 拉普拉斯是概率论创始人之一，而他认为概率论仅仅是种可简化为计算的常识。他对于概率的探索本质上是对于休谟问题的专注。例如，我们怎么知道明天太阳会升起？**他的回答由“无差别原则”和“理由不充分原则”组成**。
    - 我们称太阳会升起来是**先验概率**，因为这发生在看到任何证据之前。“先验概率”的基础并不是数过去这个星球上太阳升起的次数，因为过去你没有看到；它反映的是对于将要发生的事情，你优先相信的东西，这建立在你掌握的宇宙常识之上。
    - **后验概率**，这个概率是在看到一些证据后得出的。**问题的关键是，随着你看到的证据越来越多，后验概率应该如何演变，答案就是在贝叶斯定理里面**。—— **贝叶斯定理：P(结果|原因)=P(原因|结果)P(结果)/P(原因)**
    - 贝叶斯定理之所以有用，是因为通常给定原因后，我们就会知道结果，但我们想知道的是已知结果，如何找出原因。
    - 贝叶斯定理作为统计学和机器学习的基础，受到**计算难题**和**巨大争议**的困扰。争议在于相信贝叶斯定理的人怎么知道推导该定理的各个概率，以及那些概率的含义是什么。**贝叶斯学派的回答是：概率并非频率，而是一种主观程度上的信任。因此，用概率来做什么由你来决定，而贝叶斯推理让你做的事就是：通过新证据来修正你之前相信的东西，得到后来相信的东西**。
- **所有模型都是错的，但有些却有用**
    - **组合爆炸**——无法枚举所有可能的概率。我们照着生活中常发生的那样做：妥协。我们做简化的假设来减少概率的数量。一个很简单且受人追捧的假设是，**在给定原因的情况下，所有的结果多相互独立**。
    - 统计科学家乔治·博克斯说的一句话——**所有的模型都是错的，但有些却有用**。虽然一个模型过于简化，但你有足够的数据用来估算那就比没有数据的完美模型要好。
    - 没有人能肯定是谁发明了朴素贝叶斯算法。在 1973 年的一本模式识别教科书中，它被提到过，当时并没有注明出处，但它真正流行起来是在 20 世纪 90 年代，那时研究人员惊喜地发现，它很多时候比许多更为复杂的学习算法还要准确。
    - 运用朴素贝叶斯法来解决预测问题的列子几乎数不胜数。彼得·诺尔维格（谷歌的研究主任）一度告诉我，这是谷歌应用最为广泛的算法，谷歌的机器学习在每个角落都利用了该算法的功能。
    - 起初看起来不是这样，但朴素贝叶斯法和感知器法密切相关。 
- **从《尤金·奥涅金》到 Siri**
    - 1913 年第一次世界大战前夕，俄国数学家安德烈·马尔可夫发表了一篇文章，将所有事情的概率运用到诗歌当中。马尔可夫假设（假设错误但有用）文中每个位置的概率都是一样的，因此只需要估计3个概率：P(元音1 = 真)，P(元音 i+1 = 真 | 元音 i = 真)，P(元音 i+1 = 真 | 元音 i = 假)。
    - 马尔可夫链无处不在，而且是人们研究最多的数学话题，但它仍是受到很大限制的概率模型。
    - 隐藏的马尔可夫模型（HMM）。 HMM 和 Siri 一样，处于语音识别系统的中心。在语音识别过程中，隐藏的状态是书面形式的单词，而观察值则是对 Siri 说的声音，而目标则是从声音中推断出单词。
    - 除了 Siri， 你每次用手机来通话时都会用到一个 HMM。
    - HMM 还是计算生物学家最为喜爱的工具。
    - 如果状态和观察值都是连续而非离散变量，那么 HMM 就变成人们熟知的卡尔曼滤波。当导弹巡航到目的地时，就是卡尔曼滤波器使它保持在轨道上。 
- **所有东西都有关联，但不是直接关联**
    - HMM 有助于模拟所有种类的序列，但它们远远不如符号学派的“如果...那么...”规则灵活。如果我们允许如此随意的结构在实践中存在，那么需要掌握的概率数量将会呈爆发式增长。很长一段时间，没有人知道该如何打破这个循环。
    - 20 世纪 80 年代终于有了突破。**朱迪亚·珀尔**（加州大学洛杉矶分校的一名计算机科学教授）发明了一种新的表示方法：贝叶斯网络。珀尔是世界上最为卓著的计算机科学家之一，他的方法在机器学习、人工智能，以及其他许多领域迅速传播。2012 年，他获得图灵奖。
    - 珀尔最喜欢的例子之一是**防盗报警器**。贝叶斯网络是依赖关系的表示，附带一张包含每个变量的表格，给出变量父节点的每个值的组合概率。**条件独立**。
    - 贝叶斯网络揭穿这样一个常识性错误：机器学习无法预测鲜有的时间，或者纳西姆·塔勒布口中的“黑天鹅”。
    - 我们可以看到朴素贝叶斯、马尔可夫链、HMM 都是贝叶斯网络的特殊例子。
    - **贝叶斯网络是“生成模型”，即从概率的角度，形成世界状态的方法**。
    - 应用：
        - 最激动人心的应用之一——模拟基因在活细胞中如何相互管制。
        - 开辟机器学习在垃圾邮件的应用之后，大卫·赫克曼开始转向讲贝叶斯应用于抵抗艾滋病的斗争中。
        - 微软的 Xbox Live 游戏用贝叶斯网络来对选手进行排名，并对技术水平相似的选手进行配对。
    - 以下困扰经常发生：即使我们将所有条件独立性都考虑进来，贝叶斯网络中的一些节点仍有太多的父节点。 
- **推理问题**
    - 遗憾的是，推理问题是一个巨大的障碍。贝叶斯简单的表达了概率分布，但并不意味着基于此可以进行有效推理。贝叶斯完整的概率分布表格很难获取。
    - 求助于**近似推理**。
    - 有一个方法，珀尔在关于贝叶斯网络的书中，将其当作练习，也就是假装图形没有闭环，并来来回回传播概率，直到这些概率集中于一点。这被人们称为**“环路信念传播（loopy belief propagation）”**，因为它在含有闭环的图形中能起作用，也因为这是一个疯狂的想法。 
    - 最受人青睐的选择还是**MCMC (Markov chain Monte Carlo)**，核心思想是随便走走，就像醉汉一样，以这样的方式从网络的这个状态跳到另一个状态。这样长期下来，每个状态受访的次数就与它的概率成正比。
    - **但，MCMC 的收敛速度往往慢得让人难以忍受，或者在未完成收敛时欺骗你已经收敛。**
    - 贝叶斯网络中的推理不仅限于计算概率，它也包括为证据找到最可信的解释方法。
- **掌握贝叶斯学派的方法**
    - 对于贝叶斯学派来说，学习只是另一种形式的概率推理。**你需要做的只是运用贝叶斯定理，把假设当作可能的原因，把数据当作观察到的效果**。 即 P(假设|数据) = P(假设)P(数据|假设)/P(数据)。其中假设可以很复杂也可以很简单。贝叶斯假设计算每个可能假设的后验概率，然后在做预测时容纳所有假设，所有假设的概率之和等于1，此消彼长，取最大的为结果。**你有一个优先于假设的分布，在见到数据后，它变成了后验分布，这是贝叶斯定理给出的说法，也就是贝叶斯定理的全部**。
    - 缺点：携带不止一个而是大量的假设是一种巨大的痛苦。
    - 优点：几乎所有的假设都会以微小的后验概率作为结尾，而我们可以安然地忽略它们。实际上，只考虑单个最可能的假设通常是一种非常好的近似方法。
    - 如果我们愿意假定所有的假设都和先验概率均等，那么贝叶斯法现在就简化为**极大似然法**。
    - 未出现 ！= 概率为 0 
    - 贝叶斯学派可以做更有意义的事情。他们可以利用先验概率来编码专家对该问题的观点。但医生也不是完全可靠的，所以我们让数据来覆盖它们。
    - 如果你是**频率论者**，那么只能对那些发生次数超过一次的事件的概率进行估算。但对于贝叶斯学者来说，**概率是包含主观程度的信任**，所以他可以自由地做有根据的猜想，而且推理演算会使他们所有的猜想都一致。
    - **贝叶斯学派的观点是，选择什么表示方法由你决定，但得利用贝叶斯定理来掌握它。20 世纪 90 年代，他们声势浩大地接管了 NIPS。**
- **马尔可夫权衡证据**
    - 朴素贝叶斯的假设，虽然是错误的，但有效，并且可以大程度的简化问题。
    - 马尔可夫网络在过去 20 年中已渐渐取代贝叶斯网络，它是一组特征以及对应的权值，特点和权值共同定义概率分布。应用例子：“潘多拉”音乐基因组计划，计算机视觉。 
- **逻辑与概率：一对不幸的组合**
    - 符号学派 vs. 贝叶斯学派
        - 符号学派不喜欢概率，并指出因为概率而付出的代价高昂。推理突然变得更加珍贵，所有那些数据都变得难以理解，我们得处理好先验概率，一大批“僵尸”假设会永远追着我们。
        - 贝叶斯学派指出了逻辑的错弱性。因为在逻辑当中，任何事都可以从矛盾中推理出来。再者，如果知识是从数据中掌握得来的，那么我就无法肯定它是对的。为什么符号学派却假装肯定？无疑休谟会对这样漫不经心的态度感到不满。
    - 贝叶斯学派和逻辑学派一致认为，先验假设不可避免，但对于他们认可的先验知识种类却存在分歧。
    - 终极算法：我们既需要逻辑，也需要概率。只有逻辑可以将所有碎片组合到一张连贯的图片中；但逻辑无法处理不完整或包含嘈杂因素的信息，这在实验生物中较普遍，但贝叶斯网络可以沉着地处理这个问题。  

<h4 id="07"> 类推学派：像什么就是什么 </h4>

- 前言：
    - 类比是推动许多历史上最伟大科学进步的动力。
    - 尼采说，真理是一支由暗喻拟人组成的队伍。
    - 类比算法在机器学习中扮演重要角色就不足为奇了。刚开始它进展缓慢，甚至被神经网络夺走了光芒。它的第一个算法的化身出现在一份写于 1951 年、名不见经传的技术报告中，作者是两位伯克利的统计学家——伊夫琳·菲克斯和乔·霍奇斯。这篇报告几十年之后才发表于主流期刊中。
    - 5 个学派中，类推学派是最不具有凝聚力的一个学派。他们的统一依靠的是对于作为学习基础的、相似性判断的信任。在机器学习中，相似性是核心思想之一，而类推学派会以各种伪装的方式来保护它。 
- **完美的另一半**
    - 最近邻算法是人类有史以来发明的最简单、最快速的学习算法。
    - 懒惰学习算法会胜出的原因在于，和构建全局模型（例如，决策树）相比，只要每次弄明白指定的点在哪里会较为简单。要从数据库中学习东西可能代价很大，因为这种算法要明确划分脸部和非脸部的界线。然而，对于最近邻算法来说，界线隐含在数据点和距离度量中，而唯一要付出的就是查询时间。
    - 通常科学家利用线性回归来预测连续变量，但大多数现象是非线性的。幸运的是，**从局部来看，它们是线性，因为平滑曲线可以局部近似为直线**。 
    - **最近邻算法**的第一次成功——流行病。最近邻算法容易过拟合。**K 最近邻算法**更可靠，因为只有在多数 k 近邻受干扰时才会出错。直觉上来说，与测试例子最接近的例子应该更重要，由此有了 **加权k最近邻算法**。
    - 所有种类的算法都被用于为用户推荐项目，但加权 k 最近邻算法是第一个受到广泛运用的算法，而且要打败它仍然很困难。
    - 使最近邻算法更加有效的简单算法，就是删除所有被它们的近邻准确分类的例子。
    - 1967 年，汤姆·科韦尓和彼得·哈特证明，在给定足够数据的情况下，最近邻算法最糟糕时易于出错的概率也仅仅是最佳可行分类器的两倍。
    - **最近邻算法是史上第一个能够利用不限数量的数据来掌握任意复杂概念的算法**。
- **维数灾难**
    - “维数灾难”对最近邻算法的危害尤其大。
        1. 多数属性是不相关的是。
        2. 拥有更多的属性可能也会有害，即使这些属性是相关的。最近邻算法的基础是找到相似物体，而在高维情况下，相似性的概念就会无效。（例子：一个橘子的皮-肉比。高维正太分布中，你比较有可能得到远离而不是接近平均值的样本）。 
    - 决策树也无法幸免于维数灾难。
    - 实际上，没有那种算法能够幸免于维数灾难。这是机器学习中，继过拟合之后，第二个最糟糕的问题。维数灾难这个术语由理查德·贝尔曼在 50 岁时提出的，他是一位控制理论家。 
    - 解决方案：
        - 摆脱不相关维度。决策树会通过计算每中属性的信息增益来自动做好这一点。
        - 一个代价更大但也更智能的选择，就是围绕学习算法来选择属性。
        - 要处理弱相关的属性，一个选择就是掌握属性权值。 
- **空中蛇灾**
    - 直到 20 世纪 90 年代，应用范围最广泛的类比学习算法就是最近邻算法，但后来被来自其他学派更引人注目的“表亲”夺去光芒。当时一种新的**以相似性为基础的算法横空出世了，横扫之前的所有算法。它就是支持向量机（Support vector machines, SVM）**. 
    - 表面上看，支持向量机看起来很像加权 k 最近邻算法。支持向量机只会记住那些用于确定边界的关键例子——**支持向量**。
    - 为了学习支持向量机，我们需要选择向量和它们的权值。如何找到最优边界？**约束优化**，解决约束优化问题的方法，不是沿着坡面走，而是走与约束面平行的那部分坡面，然后当该部分为零时，停下来。
    - 在现实中，我们通常会让支持向量机违背一些限制条件，否则它容易过拟合。
    - 支持向量机可以当作感知机的一个概括版，因为当你利用某个特定的相似性度量时，得到的就是类别之间的超平面边界（向量之间的点积）。
    - 支持向量机早期较大的功绩还在于文本分类。
    - 通常，支持向量机选择的支持向量越少，就能更好地进行概括。随着维度的上升，这部分也会上升，因为支持向量机无法幸免于维数灾难，但它们最能抵抗这个灾难。
    - 然而，支持向量机唯一最让人吃惊的属性就是，无论它形成多么弯曲的边界，那些边界也总是直线（或者一般为超平面）。
- **爬上梯子**
    - 两个东西如果在一些方面意见一致，那么它们就是相似的。类比推理中的两大子问题：
        1. 弄明白两个事物的**相似度**，确定由它们的相似度还能推导出什么。
        2. 弄明白在已经发现的相似点的基础上，如何推导出新的东西。
    - 案例：求助台、
    - 类比法的强大：
        - 类比学者最棒的技巧在于跨越问题域来进行学习；
        - 有类比无法做到的事情吗？道格拉斯·霍夫斯泰特认为没有，他是一位认知科学家。  
- **起床啦**
    - 符号学派 vs. 类推学派：实际上，规则就是概括的实例，这种情况下我们已经“忘记”一些属性，因为它们并不重要。
    - 在 “我” 博士论文中，设计了一种算法，RISE，将基于实例的学习和基于规则的学习结合起来。RISE 比当时最好的规则和实例学习算法预测得还要准确，而实验也表明，这是因为算法结合了两者的最佳特征。
    - RISE 是通往终极算法的一个步骤，因为它将符号与类比学习结合起来了。不过这仅仅是一小步，还有很多要改进和细化。 

<h4 id="08"> 无师自通 </h4>

- 前言
    - 较大的孩子和成年人可以进行时空旅行，也就是记住过去的事，但也只能回忆到 3 岁的事。
    - 当然，问题在于罗比出生时，脑子里该运行哪种算法。我们需要以更抽象的水平来模拟儿童的学习，以免只见树木、不见森林。孩子很多时候是在没人监督的情况下进行自学。 
- **物以类聚，人以群分**
    - 将世界组织成客体和类别，对于成年人来说，这是第二天性；对于婴儿来说却不是；对于机器人罗比来说，更没有可能。我们需要一种能够自发将所有相似物体或者一物体的不同图片集中起来的算法。这就是聚类问题，这在机器学习当中也是人们研究最多的主题之一。
    - 对事物进行聚类，这是人类的天性，也是获取知识的第一步。 
    - 大数据和机器学习的全部要点在于避免粗糙的思考。
    - **k-means algorithm**，起源可以追溯到 20 世纪 50 年代。
        - 优势：精密、简单、人气很高
        - 缺点：提前确定集群的数量；k 均值算法只有在集群易于区分的情况下才能起作用
    - 先有鸡还是先有蛋的问题。1997 年，来自哈佛大学的三个统计学家（亚瑟·邓普斯特、南·莱尔德、唐纳德·鲁宾）表明，以下计划可以生效：每次我们绕着圈走时，集群模型就会变得更好，而当模型是可能性的一个局部最大值时，循环结束。他们称这个计划为期望最大化。**他们称该计划为期望最大化演算法（Expectation Maximization, EM 算法），其中 E 表示期望（推断预期概率），而M代表最大化（估算可能性最大的参数）。**
    - **当我们想掌握某个统计模型，但又缺乏一些关键信息时（例如，例子的类别），就可以利用 EM。这使它在所有机器学习中成为最受欢迎的算法。**
    - k 均值和 EM 之间的某个相似性，因为它们都交替进行两项工作：将实体分配给集群，然后更新集群的描述。
- **发现数据的形状**
    - 数据的战役
        1. 将大量实体分类成更小数量的集群
        2. 缩短每个实体的描述
    - **维数约减**：大量的可见维度（像素）简化成几个隐性维度（表情、面部特征）。
        - 线性：PCA (principle-component analysis)
        - 非线性：等距映射算法。
- **拥护享乐主义的机器人**
    - problem：**聚类**和**维度简化**虽然使我们更加靠近人类学习，但仍**丢失**了一些很重要的东西。
    - solution
        - 使用 step-by-step instruction 的指令，把传感器读数和正确的行为组成一对，但这只对**精密任务**可行。
        - 前几章中学习算法都由“即时满足”这一原则引导：每个行为都会从“老师”那里得到及时奖励。有一个机器学习的子域致力于这样的算法：进行主动探索，偶然得到奖励，然后弄清楚将来怎样才能再得到奖励。这很像婴儿到处爬和把东西放到嘴里。—— 这样的过程称为**“强化学习”**。
    - 强化学习的一个重要先驱是跳棋游戏程序，这是 IBM 的研究员阿瑟·塞缪尔于 20 世纪 50 年代编写的。
    - 强化学习
        - **首要思想**是：并不是所有的状态都有奖励（正面或者负面），但每种状态都会有价值。
        - **目标**往往是采取那个能获得最丰富奖励的行为。
        - 强化学习通过估算每个状态的价值来做到这一点。
    - 强化学习中的**利用——探索困境：**为了使奖励最大化，你很自然地想选择能达到高价值状态的行动，但这可能会阻止你发现其他价值更高的奖励。
        - 强化学习算法解决这个问题的方法是时而选择最佳行动，时而随机选择。
        - 实际上，强化学习就是一种加速进化过程——尝试、丢弃，然后在单个生命一生而不是几代中改进行动——有了这个标准，它的效率会更高。 
- **熟能生巧**
    - “幂法则（a power law）”：随着时间达到某负幂时，表现会出现变化。比如：随着尝试次数的累加，完成任务所需的时间呈幂级下降。几乎每项人类技能都会遵循幂法则，不同的幂会对应不同的技能。
    - 1979 年，艾伦·纽厄尔和保罗·罗森布鲁姆开始探索这个所谓的“幂法则”实践存在的原因。当时，没有哪个实践模式可以解释幂法则，纽厄尔和罗森布鲁姆怀疑这**可能与组块有关**。**组块**是一个来自感知与记忆心理学的概念。我们以组块的形式来感知并记住东西，而在任意给定的时间内，我们只能通过短暂记忆来记住这么多组块。
    - 在感知和记忆中，组块仅仅是一种符号，代表了其他符号的模式，就像 AI 代表人工智能。他们发现，**人类解决问题的方式是将问题分解为小问题，再将小问题再分解为更小的问题，然后系统地减少初始状态（比如第一个公式）与目标状态（第二个公式）之间的差异**。这种意义下，组块有两个部分：**刺激**（你从外部世界或者短暂记忆中识别出模式）和**反馈**（你因此而执行的行动顺序）。
    - 接下来他们将组块并入“猛增（Soar）”理论中。通过对数据和类推法进行组块，它甚至可以应用到掌握新知识中。
    - 组块和强化学习在商业中的应用不如在监督式、聚类或者维数简约中广泛，但是通过与环境互动进行的相似学习类型是掌握行动（或相应行动）的效果。
    - **A/B Test**.
- **学会关联**
    - **世界是一张相互联系的网络**。了解一个实体的最佳方法——无论它是人、动物、网页还是分子——就是了解它如何与其他实体进行连接。
    - 困难：
        - 当数据变成整个大网络时，似乎就没有许多例子来学习了，只剩下一个，而且这不够。我们想确认流感是传染性疾病，方法就是通过观察在社交网络中的感染模式。解决办法就是找到一组特征，并掌握它们的权值，就像在马尔可夫网络中那样。从局部上看，大型网络往往和小型网络的表现没有差异。
        - 关联学习算法能达到的最佳效果就是让懒散的老师变得勤奋。对于普通分类器来说，没有归类的例子毫无用处。
        - 从实体的属性推断出其类别，这就涉及几次查找工作和一些计算。
    - 关联学习历史悠久，可以至少追溯到 20 世纪 70 年代，以及符号派技巧（如逆向演绎）。但随着互联网的出现，它需要新的动力。一个有趣的现象——口碑传播。
    - 如果你想了解世界如何运转，那么关联学习就是很好的工具。
    - 对于大数据，抱怨较普遍的就是拥有的数据越多，就越容易在大数据中发现伪模式。 
    - 应用：社交网络、细胞如何运作  

<h4 id="09"> 揭开迷惑 </h4>

- 前言：
    - 机器学习既是科学，也是技术。 
- **万里挑一**
    - 主要介绍集成（ensemble）学习的思想。—— 元学习
    - “堆叠”：大卫·沃尔珀特提出，他是「天下没有免费的午餐」定理的创作者。
    - “袋装”：里奥·布雷曼发明，通过重新取样的方法来产生训练集的随机变量，将同样的学习算法应用到每个训练集中，然后通过投票将结果结合起来。
    - “推进”，最聪明的元学习方法之一。两位学习领域的理论家约阿夫·弗罗因德和罗伯·夏皮尔创造。核心思想：将相同的分类器不断应用到数据中，利用每个新的模型来纠正前面模型的错误。想法起源：该过程可以推进只比随机猜测好一点的分类器，但如果持续如此，就会接近完美。
- **终极算法之城**

| 学派     | 优化           | 评价  | 代表法 | 
| ---     |---             | --- | --- |
| 符号学派 | 逆向演绎 | 准确度 | 逻辑 | 
| 联结学派 | 梯度下降      |   平方误差 | 神经网络 |
| 进化学派 | 遗传搜索     |    适应度 |  遗传程序 |
| 贝叶斯学派 | 概率推理      |    后验概率 |  图解模型 |
| 类推学派 | 约束优化      |    边际 | 支持向量机 |
- **马尔可夫逻辑网络（MLN）**
    - 2003 年，“我”开始思考如何将逻辑和概率统一起来。  
- **从休谟到你的家用机器人**
    - 炼金术就像一台归纳图灵机，我们可以对图灵机进行编程，使其行动起来像非常有力量的或者受到极大极限的学习算法。 
- **行星尺度机器学习**
    - 欧洲的“未来信息和通信技术”项目旨在建造整个世界（真正含义即字面意思）的模型。社会、政府、文化、技术、农业、疾病、全球经济等不能落下一样。 
- **医生马上来看你**
    - CanceRx 会利用她的正常细胞和肿瘤细胞来将它的模型实例化，并尝试所有可能的药物、直到它找到一种能杀死癌细胞而又不伤害健康细胞的药物。
    - 现在人们已经在努力建造最终会成为 CanceRx 的东西。在系统生物学的新领域中的研究员会模拟整个代谢网络，而非个体基因和蛋白质。 

<h4 id="10"> 建立在机器学习之上的世界 </h4>

- **性、谎言和机器学习**
    - 学习算法越好，就越值得你花时间让它了解你。但根据经验，你想让自己足够与众不同，这样它就不会将你和“普通人”混淆，但也别太与众不同，这样它就没办法理解你了。
    - 模型需以人类能理解的方式呈现。 
- **数码镜子**
    - 各个维度的数据可以反应你不同的侧面。 
    - 有一个令人冷静（也许是安心）的想法，就是当今世界上没有哪种学习算法可以利用所有数据（甚至美国国家安全局也不可以）。 
- **充满模型的社会**
    - 每个人都会有一个机器人随从。 
- **分享与否？方式、地点如何？**
    - 如果其他人了解你的速度比你了解他们的速度要快，那么你就会陷入麻烦。解决办法就是——分享。
    - 当今你的数据可以分为遗下 4 类：
        1. 你和所有人分享的数据；
        2. 你和朋友或者同事分享的数据；
        3. 你和各种公司（不论是否有意）分享的数据；
        4. 你不与别人分享的数据。
    - 所有 4 类数据的分享都有问题。这些问题有一个共同的解决办法：**新型公司与你的数据的关系，就像银行和你的钱的关系一样**。
    - **完整的数据比各部分的总和要多。**
    -“隐私”。最好让人们现在树立意识，选择该分享什么、不该分享什么，以及如何、在哪里分享。  
- **神经网络抢了我的工作**
    - 一个普遍的主题是，狭义定义的任务很容易通过数据来完成，但那些需要技能与知识广泛结合的任务却不能。
    - 一项任务需要的背景信息越多，计算机能迅速完成它的可能性越小。
    - **把大数据看作你知觉的延伸，把学习算法看作你大脑的扩展**。
    - 通过机器低成本完成的事情越多，人类学家的贡献就越有价值。 
- **战争不属于人类**
    - 机器人的主要用途之一就是完成那些对人类来说过于危险的任务，战争也一样危险。
    - 反对的原因：
        - 让机器人观察人类来学习道德标准不是一个好主意，当人类违反准则时，机器会困惑。
        - 机器的参与让战争变得容易。
    - 但禁止机器人战争也许不可行。和所有武器一样，自己拥有机器人，比信任另一方认为不该有机器人更安全。
- **谷歌+终极算法=天网？**
    - 备有终极算法的人工智能接管世界的概率是零。原因很简答：不像人类，计算机本身并没有自己的意志。因此我们可以张开怀抱迎接比我们大脑强大很多的计算机。
    - 但以下忧虑也是存在的：
        - 最大的忧虑是，和所有技术一样，人工智能可能会落入不法之徒手里。
        - 人类会自愿屈服于统治。人类太容易遵守别人的规则。
        - 机器会给我们要求的而不是想要的东西。  
- **进化的第二部分**
    - ”奇点“，黑洞。智能无法永远都在提高。 
    - 我们一直生活在这样一个只能理解某些部分的世界中。主要的差别在于，我们的世界现在部分创造了我们。
    - 我们所处的轨道不是奇点，而是相变。计算机程序是世界上最快的复制者，但创造它们却比较缓慢。
    - 自然进化最后不会只有两种物种，一种物种顺从另一种物种。这就意味着下一个瓶颈就是界限，虽然现在我们还没看到它。其他过渡期会到来，有些长，有些短，有些快，有些不会持续很长，但在地球的生命历程中，接下来的几千年很有可能是最为令人惊叹的一段历程。