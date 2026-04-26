# Patrick Collison 重大决策记录

> 调研时间：2026-04-24（更新于 2026-04-25）
> 信息来源：Patrick Collison 官网、Tim Ferriss 访谈、Shane Parrish 访谈、Stripe 博客、媒体报道等
> 可信度评级：高（一手来源为主）、中（访谈和二手报道）、低（匿名评论）

---

## 一、创业核心决策

### 1. 进入支付行业的决策（2010）

**背景**：
- 2010年，在线支付市场已有众多成熟玩家（PayPal、Authorize.net、Braintree等）
- 行业被认为有极高的进入壁垒：监管、银行合作、合规要求
- Patrick 和弟弟 John 当时都还很年轻（Patrick 22岁，John 20岁）

**决策逻辑**：
- 核心洞察：开发者成为决策的关键影响者
  - Patrick 访谈原话："We didn't even know that was such a stupid distribution strategy and go-to-market mechanism. We didn't even know how much enterprise marketing and enterprise sales motion and all the rest we were skipping over."
- 不认为监管和银行壁垒是不可逾越的
  - "Ultimately, regulators and banks and so on are comprised of good people who want to do the right thing... they're reasonable."
- 简单的盈利逻辑：7行代码就能集成支付

**结果**：
- 成功。Stripe 成为估值最高的私有金融科技公司之一
- 关键时机：2010-2011年正是传统企业开始"重视开发者意见"的转折点
- 后来 Patrick 承认："我很重要的运气是，我们刚好在世界开始转型时启动"

**反思**：
这是"无知者的运气"典型案例——他们不知道自己应该害怕的事情。

---

### 2. 公司命名决策（2010）

**背景**：
- 最初注册公司名：SlashDevSlashFinance, Inc.（拼写出来的"斜杠"）
- 产品名：/dev/payments（但实际上用户访问 devpayments.com）

**决策过程**：
- 团队名称成了严重的麻烦
- 银行合作伙伴会问："公司全名叫什么？"
- Patrick 回忆："They'd ask us our name or for our business card or something. We'd have to hand over this thing that doesn't even look like a company name."
- 甚至每次有人正确拼写公司名都是"值得庆祝的时刻"

**转折点**：
- 2010年冬天，他们在加州的一个多雨冬季
- 团队写了一个脚本来生成随机名称并检查域名是否可用
- 目标：单音节英文单词，没有强烈的预先关联

**最终决策**：
- 选中"Stripe"
- 域名花费：1-2万美元
- Patrick 说："如果对方要价20万美元，我们两秒就会放弃，换下一个"

**决策模式**：
- 极度务实——不执着于某一个选项
- 快速迭代——承认错误并迅速改变
- 成本效益分析——域名成本 vs 继续使用糟糕名称的隐形成本

**搞笑插曲**：
他们改名后忘记通知客户。用户访问 devpayments.com 时被重定向到 stripe.com，收到很多邮件问："你们被黑了吗？这是钓鱼网站吗？"幸好当时只有约5个客户。

---

### 3. Y Combinator 决策

**背景**：
- Patrick 通过之前的项目 Auctomatic 与 Paul Graham 建立了联系
- PG 在 Patrick 15岁时就认识他，邀请他访问 Google

**决策**：
加入 YC 2010 年冬季批次

**关键价值**：
- Paul Graham 成为其最重要的导师之一
- Patrick 称 YC 为"过去20年最神奇的发明之一"
- 在 YC 内部，Stripe 以"Collison Installation"闻名

**"Collison Installation"决策**：

Paul Graham 的描述：
> "Stripe is one of the most successful startups we've funded. And the problem they solved was an urgent one. If anyone would have sat back and waited for users or could have sat back and waited for users, it was Stripe. But in fact, they're famous within YC for aggressive early user acquisition."

**具体做法**：
- 别的创始人问："你愿意试试我们的 beta 吗？"，得到肯定回答后发链接
- Collison 兄弟问完立即说："那你给我你的笔记本电脑"，当场安装配置

**决策逻辑**：
- 没有等待"完美产品"
- 主动接触同批 YC 公司作为初始用户
- 极度注重用户获取的现实性

---

### 4. 营销策略决策

**决策**：
早期不采用传统的企业销售和营销策略，而是专注于写博客文章和产品口碑。

**背景**：
- 大多数 B2B 公司花费巨额营销预算
- Patrick 认为互联网改变了信息传播方式

**核心逻辑**：
- 建立在 Slashdot、Hacker News、Twitter 等平台上的信息传播更高效
- 写好博客文章让产品自我传播
- 不依赖付费广告和传统销售渠道

**案例**：
- 员工 Evan 写了一篇关于"如何用 GDB 调试 Python"的技术博客
- 几乎与 Stripe 无关，但展示了技术能力
- 2012年获得大量流量，让人们知道 Stripe 的技术实力

**深层考虑**：
这个决策有两个巨大好处：
1. **成本优势**：不需要巨额营销预算启动
2. **激励正确**：迫使团队构建真正优秀的产品

Patrick 的洞察：
> "如果产品不好，但你有大营销预算，短期内可能还行。但如果你必须依赖产品口碑存活，你必须建立真正好的产品开发能力。"

**关键洞察**：
> "传统营销的激励是吹嘘产品或过早发布。但如果你必须依赖用户诚实反馈，这会迫使你建立能在质量上竞争的产品开发组织。"

---

### 5. 产品技术决策：API 设计哲学

**决策**：
将 API 易用性放在首位——"7行代码就能接受支付"。

**背景**：
- 传统支付 API 极其复杂
- 文档质量差，集成困难

**决策模式**：
- 从开发者视角出发（他们自己就是开发者）
- 简单即胜利
- 功能强大但易于上手

**与竞争对手的差距**：
Patrick 注意到大公司"无法转化资本为好软件"：
> "想想任何大公司的网站或 App？通常很糟糕。UI janky，动画不对，laggy。但他们可以把资本转化为一队好车、好的广告活动。奇怪的是，他们无法把资本转化为好软件。"

**竞争壁垒**：
- 大公司想做好软件，但组织转变极其困难
- "一旦你在产品战场上，对手无法快速复制你的软件能力"

---

### 6. 组织架构决策

**决策**：
采用相对传统的组织架构，不激进创新。

**背景**：
- 许多创业公司尝试新架构（Zappos 的 Holacracy、Medium 的自组织等）

**Patrick 的分析**：
- 组织结构是"trapdoor decision"（不可逆决策）
- 90%以上大幅偏离最佳实践的组织都会失败
- 不是创新不好，而是创业公司已经有足够多风险，不应该在这方面再加风险

**他说**：
> "我喜欢有人尝试新东西。但我觉得你选择的实验应该是你真正相信的少数几个。"

关键区分：
- **你希望别人做的事** vs **你自己应该做的事**
- "我可能觉得某个创新组织模式是个好主意。但我很高兴别人去尝试，我自己可能保持保守。"

**研究结果**：
Patrick 研究了 Google、Facebook、Amazon、Microsoft 的组织方式：
- 不完美，但"经验上足够支撑这些公司的成功"
- 这些公司证明了传统架构可以支撑万亿美元市值
- 为什么要在成功概率极低的组织创新上冒险？

---

### 7. 弟弟分工决策

**模式**：
Patrick（CEO）+ John（总裁）

**观察**：
- Patrick 更内向、阅读量惊人
- John 更外向、善于沟通
- 两人技能互补

**避坑经验**（来自 Auctomatic 时代）：
- Chris Sacca 曾描述在庆祝 Auctomatic 出售的酒吧里，John 弟弟因为未成年被拦在门外
- "一个刚刚卖掉公司、成为百万富翁的创始人，没能进入自己的庆祝派对"
- 这体现了硅谷对年龄的开放——"智能的年轻人不需要'慢慢爬上去'"

---

### 8. 收购决策

**Stripe 的主要收购**（部分）：

1. **Touchtech Payment**（2019）- 支付认证公司
2. **Paystack**（2020）- 尼日利亚支付公司，约2亿美元
3. **TaxJar**（2020）- 税务计算公司，约2亿美元
4. **Bouncer**（2021）- 卡验证公司

**收购逻辑**（可推断）：
- 补充核心支付能力
- 国际化扩张（Paystack - 非洲市场）
- 减少税务合规摩擦（TaxJar）

---

### 9. 产品线扩展决策

**Stripe 的产品演进**：

1. **支付处理** → 核心业务
2. **Stripe Connect** - 市场平台支付
3. **Stripe Atlas** - 帮助公司注册成立
4. **Stripe Climate** - 碳去除购买联盟
5. **Stripe Press** - 出版书籍

**Patrick 的逻辑**：
从他的问题列表可以看出他对"知识传播"和"进步"的深层兴趣。Stripe Atlas 和 Stripe Press 都体现了这一哲学。

**Atlas 决策逻辑**：
- 阻碍创业公司发展的不仅是支付——还有法律结构
- 简化公司注册和银行开户流程
- 几千美元 vs 传统方式数万美元和时间

---

### 10. 融资决策

**关键融资轮次**：
- 2011年：YC 融资
- 2011年：Sequoia 等投资
- 之后多轮，估值不断攀升

**投资人选择**：
- Peter Thiel 是早期投资人
- 主要 VC：Sequoia、Founders Fund、Andreessen Horowitz 等

**Patrick 没有公开谈论太多融资细节**，但他的行为模式表明：
- 不追求最高估值
- 选择能提供战略价值的投资人
- 保持长期控制权

---

### 11. 阅读与学习决策

**决策**：
大量阅读"被时间过滤"的书籍，而非追逐畅销书。

**Patrick 的阅读哲学**：
> "你应该主要忽略每年出版的书籍，利用过去10年已经有足够时间筛选真正珠玉的优势。"

**具体做法**：
- 家里各处放书（书架、餐桌、沙发旁、床边、床上）
- 买入感兴趣的书，不必立即读完
- 6个月或18个月后，合适时机再回头读
- "Reader-book fit"——时机很重要

**《The Dream Machine》案例**：
- 这本讲述 J.C.R. Licklider 和互联网创造的书已经绝版
- Patrick 发现它、买光亚马逊库存分发给 Stripe 员工和朋友
- Alan Kay 称这本书"在计算机历史书籍中几乎独一无二"
- Patrick 说技术行业很少回顾历史——这既是优势也是劣势

---

### 12. 公司文化决策

**从 Tim Ferriss 访谈中的线索**：

**招聘标准**：
- Shane Parrish 访谈提到 Patrick 看重：
  - 与 Stripe 文化的契合度
  - 能力与贡献

**学习文化**：
- Patrick 是 Stripe 的"首席阅读官"
- 通过书籍、博客文章传播理念
- 技术博客文化（如 Evan 的 Python 调试文章）

---

### 13. 公开表达决策

**决策**：
建立个人网站 patrickcollison.com，公开回答深度问题。

**内容类型**：
- 书单（600+ 本推荐书籍）
- 深度问题清单（Questions）
- 关于经济进步的研究（与 Tyler Cowen 合写文章）
- 关于科学投资回报的文章（与 Michael Nielsen 合写）

**问题清单决策**：
Patrick 公开了他正在思考的问题，包括：
- 为什么某些东西越来越贵（医疗、教育）？
- 为什么过去完成重大项目的速度比现在快？
- 为什么 GDP 增长率如此平滑？
- 为什么斯德哥尔摩有那么多成功创业公司？
- 如何在自然没有死亡机制的系统里保证足够的新陈代谢？
- 编程环境为什么还这么原始？
- 书的继任者是什么？
- 为什么瑞士和日本的执行质量如此之高？

**这体现的决策模式**：
- 公开思考，邀请协作
- 跨学科好奇心
- 承认自己不知道

---

### 14. Progress Studies 决策

**决策**：
2019年与 Tyler Cowen 共同发表《We Need a New Science of Progress》。

**行动**：
- 建立 Progress Studies 社区
- 支持 Works in Progress 杂志
- 这一领域现在有明显影响力

**决策模式**：
- 识别一个被忽视但重要的问题
- 用有分量的方式提出它
- 建立社区和资源来推动进展

---

### 15. 其他投资与项目决策

**Patrick 参与/支持的项目**：

1. **Fast Grants**（COVID 期间）- 快速资助科学家
2. **Arc Institute** - 生物医学研究新模式
3. **CA YIMBY** - 推动加州住房政策改革
4. **Charter Cities Institute** - 实验性城市研究

**决策逻辑**：
- 这些都不是"Stripe"，但都围绕"增长"和"进步"主题
- 个人兴趣延伸为系统性项目
- 愿意投入资本和影响力推动系统性变革

---

## 二、失败决策与反思

### 1. 公司名称失误

**失败**：SlashDevSlashFinance

**反思**：
- "我们以为这个编程笑话很有趣。令我们震惊的是，其他人并不这么认为。"
- 低估了名称对合法性的影响
- 花了大量时间解释公司名，分散精力

**教训**：
- 不要用内部幽默做外部决策
- 测试你的假设——哪怕是公司名

---

### 2. 更名后忘记通知客户

**失败**：改名 Stripe 后没有邮件通知现有客户

**反思**：
- "终于在2011年1月某个早晨，我们按下了切换开关。所有东西都变成 Stripe。在所有要改变的事情清单里，我们忘记加一条：告诉我们的客户。"

**教训**：
- 迁移计划需要完整清单
- 小疏忽可能造成大困惑

---

### 3. 对竞争对手反应的判断

**Patrick 承认的惊讶**：

他预期大公司看到 Stripe 成功后会迅速复制并反击。但实际上：
> "令人惊讶的是，他们几乎什么都没做。即使他们不再忽视我们，也无法简单地说'好吧，现在让我们开始创建好产品'。"

**反思**：
好的软件能力是深层组织文化，不是可以随意复制的东西。

---

## 三、决策模式分析

### 1. 模式一：利用信息不对称

- Patrick 大量阅读历史，知道别人忽视的模式
- 从历史案例中提取决策框架
- 研究传统项目为何完成效率高（帝国大厦410天，阿波罗9年）

---

### 2. 模式二：保持产品聚焦

"如果产品不增长，心理上很容易安慰自己'我只是营销不够'。更难接受'也许我的产品就是太丑'。"

- 不用营销预算掩盖产品问题
- 要求产品在公开市场上竞争
- 把失败快速暴露而不是延迟

---

### 3. 模式三：区别"希望别人做的实验"和"自己应该做的保守"

- 对 Holacracy 等组织创新：支持别人尝试，自己保持传统
- 对新产品功能：激进实验
- 对 trapdoor decisions：保守行事

---

### 4. 模式四：用历史书籍而非当年畅销书做决策输入

- 不看"今年流行什么"
- 看哪些理念经受住了时间考验
- 600+ 本书单，分类为"above average"和"particularly great"

---

### 5. 模式五：把运气归因放在明处

Patrick 反复强调：
- Stripe 成功很大程度是时机运气
- 不"喝自己的 Kool-Aid"
- 承认自己没有从一开始就有"深刻洞察"

> "我们真的没有从一开始就有这种深刻洞察。我们只是恰好有一个因为出身和起点而产生的特定视角。我们很幸运。"

---

### 6. 模式六：在核心问题上做决定性的赌注

- 支付行业：所有人都说太难，他们做
- 开发者优先：不符合当时企业销售逻辑，但坚信
- 简单 API：在朋友家的客厅里写代码，不是因为市场调研

---

### 7. 模式七：长期思维在中国语境下的映射

Patrick 的名言（虽然未被直接引用，但逻辑一致）：
- 研究已完成全过程的公司（如 Microsoft）而非"今年的明星"
- 关心"GDP增长为什么如此平滑"这类超长期问题
- 推动科学领域的研究效率改革

---

## 四、与 John Collison 的分工

**虽然没有直接的详细资料**，但可以从公开信息推断：

**Patrick 倾向于**：
- 产品和技术
- 长期战略思考
- 公共议题（Progress Studies、Climate 等）
- 与学术和思想领袖对话

**John 倾向于**：
- 商业拓展
- 外部沟通
- 客户关系

**他们共同的特点**：
- 极度好奇
- 大量阅读
- 低调务实
- 不追求媒体曝光

---

## 五、言行一致性分析

### 一致之处：

1. **倡导阅读，自己也读** - 600+ 书单，不断更新
2. **强调产品，确实做了好产品** - Stripe 的开发者口碑
3. **说时机重要，承认运气** - 反复强调而不是"成功学"
4. **关心长期问题，投身 Progress Studies** - 行动与言论一致

### 可能的不一致：

1. **说自己保守** - 但实际做了很多实验性项目
   - 但这可以用"在 trapdoor decisions 保守，在可逆决策实验"解释
2. **说组织创新风险高** - 但 Stripe 内部做了 Sorbet 这样的创新
   - 这是技术产品创新，不是组织创新，符合他的框架

---

## 六、关键语录

1. **关于组织创新**（Tim Ferriss 访谈）：
   > "I think there's probably a 90 percent chance, maybe higher that any meaningful deviation is a bad idea. But I think we should celebrate the fact that all these experiments are happening."

2. **关于时机和运气**：
   > "We didn't even know that was such a stupid distribution strategy... We were lucky where the world really started to change around 2010-2011."

3. **关于好软件的稀缺性**：
   > "How hard it is for organizations to build good software... given that it's not rocket science, why are there so few good software products?"

4. **关于阅读**：
   > "I really think people should be much more biased towards older books than they are."

5. **关于实验**：
   > "If someone tries strange things that don't match our preexisting comprehensions, there's some combination of mockery or dismissiveness... I really think we should be encouraging and celebrating them. And the weirder the effort is, the more they deserve our support."

---

## 七、参考来源

1. Tim Ferriss Show 访谈（#353）- 深度访谈，涵盖早期决策
2. Shane Parrish (Farnam Street) 知识项目访谈
3. Patrick Collison 官网（patrickcollison.com）
   - Questions 页面
   - Advice 页面
   - Growth 书单
   - Progress 页面
4. Paul Graham 关于 Stripe 的文章
5. Stripe 官方博客
6. 媒体报道和公开演讲

---

## 八、待进一步研究的方向

1. **具体融资轮次的决策细节** - Patrick 很少公开谈论
2. **收购决策过程** - Paystack、TaxJar 等如何评估
3. **内部产品优先级决策** - Stripe 产品众多，如何排序
4. **与 John 的具体分工** - 需要更多直接资料
5. **失败项目的细节** - 哪些功能被砍掉，为什么
6. **COVID 期间的 Fast Grants 决策** - 如何在短时间内做出资助决定
7. **Stripe 内部文化实践** - 除了公开信息外的具体做法

---

---

## 九、补充决策记录

### 1. 离开爱尔兰的决策

**背景**：
- Patrick 出生于爱尔兰乡下的 Dromineer
- 16岁时开发了编程语言并获欧盟青年科学家奖
- 2007年创建 Auctomatic（与弟弟John），卖给 Live Current Media 获悉数百万美元
- 2008年离开爱尔兰前往美国

**决策逻辑**（来源：patrickcollison.com/blog/stripe-ireland）：

Patrick 分析了 Stripe 能否在爱尔兰创立：
- **投资环境差距**：爱尔兰 VC 市场远不如硅谷成熟
- **人才池限制**：爱尔兰技术人才基数小
- **收购机会少**：缺乏活跃的收购方
- **创业网络薄弱**：没有成型的创业生态

核心洞察：
> "I'm struck by how things seem to be improving... but the right question is probably: could Stripe have grown as fast in Ireland?"

**结果**：
- 主动迁移到硅谷
- 正确识别了"人口集中"的网络效应
- 后来返回时爱尔兰已改善，但时间窗口不可逆

**反思**：
他后来反思说情况在改善，但核心问题是：Stripe 能否在爱尔兰以同样的速度增长？答案可能是否定的。这个决策体现了他的实用主义——不被情感绑架，相信数据。

- 来源：patrickcollison.com/post/stripe-ireland
- 可信度：高（一手来源）

---

### 2. 远程工作决策

**决策时间**：2019年5月

**背景**：
- Stripe 当时已有旧金山、西雅图、都柏林、新加坡四个工程中心
- 已有数百名远程员工，但他们是"附属"于某个办公室团队
- 远程员工反馈良好，73% 的工程师认为公司很好地整合了远程员工

**决策逻辑**（来源：Stripe 官方博客）：

**核心洞察**：
1. **用户分布**：Stripe 用户遍布全球，需要本地视角
2. **人才分布**：99.74% 的优秀工程师生活在四个中心之外
3. **技术进步**：Google Docs、Slack、git、Zoom 等工具使远程协作足够高效
4. **实际效果**：远程员工已贡献了 Stripe 技术栈、产品和文化的基石元素

**具体行动**：
1. 建立"Remote"作为第五个工程中心，与其他物理办公室**同等地位**
2. 招聘至少100名远程工程师（2019年）
3. 设置专门的远程工程负责人，类似各办公室的 site lead
4. 扩大远程招聘范围（产品经理、工程经理、技术项目经理）
5. 改善远程体验：日历邀请自动附带视频会议链接

**关键限制**：
- 初期只在北美（美国和加拿大）招聘远程员工
- 时区差异大的地区尚未准备好
- 都柏林和新加坡办公室尚未成熟到支持远程员工

**更新**：后来扩展到更多地区

**决策模式**：
- 不是"远程优先"激进实验，而是"远程同等"务实扩展
- 基于数据（员工调查）和实际效果（远程员工贡献）
- 保持谨慎（时区限制）

- 来源：stripe.com/blog/remote-hub
- 可信度：高（Stripe 官方博客，Patrick 亲自参与讨论）

---

### 3. 远程办公后续调整（COVID 后）

**背景**：
- 2020年 COVID 疫情迫使全球远程工作
- 科技行业普遍转向永久远程或混合办公

**Patrick 的立场**（来自 Hacker News 讨论间接引用）：
- 对"远程游客"持保留态度
- 欢迎认真对待远程工作的人
- 与许多科技公司创始人的立场一致（担心文化稀释）

**外部评价**：
- 一部分员工认为远程工作效果好
- 另一部分观察者认为 Stripe 文化高度依赖面对面交流

**决策模式**：
- 不是盲目拥抱趋势
- 基于实际效果数据调整
- 区分"认真远程工作者"和"远程游客"

- 来源：Hacker News 讨论、媒体报道
- 可信度：中（二手来源）

---

### 4. 个人投资与慈善决策

#### Fast Grants（COVID 期间）

**背景**：
- 2020年 COVID 疫情爆发
- 传统科研资助流程过慢

**决策**：
与 Tyler Cowen 等人创建 Fast Grants，快速资助科学家

**决策逻辑**：
- 传统 NIH 资助周期太长
- 疫情需要快速响应
- 简化申请流程，快速决策

**结果**：
- 分发了"大量资金"给科学家
- 成为 COVID 科研资助的重要补充

- 来源：fastgrants.org、patrickcollison.com/about
- 可信度：高

#### Arc Institute

**决策**：
参与创建 Arc Institute，生物医学研究新模式

**意图**：
- 改革科研激励机制
- 减少科学家的行政负担
- 支持高风险高回报研究

- 来源：arcinstitute.org
- 可信度：高

#### CA YIMBY（加州住房改革）

**决策**：
支持 CA YIMBY（Yes In My Back Yard），推动加州住房政策改革

**逻辑**：
- 与他关注"成本病"和"基础设施效率下降"一致
- 加州住房短缺影响经济进步
- 支持增加住房供给的政策

- 来源：patrickcollison.com/about
- 可信度：高

#### Charter Cities Institute

**决策**：
支持 Charter Cities Institute，研究实验性城市

**逻辑**：
- 与"如何帮助更多实验城市启动"问题直接相关
- 深圳等特区成功案例证明城市实验的价值
- 城市是制度创新的试验场

- 来源：patrickcollison.com/questions（问题页面提及）
- 可信度：高

#### Stripe Climate

**决策**：
创建 Stripe Climate，碳去除购买联盟

**影响**：
- 成为世界上最大的碳去除购买者联盟
- 企业可自动将部分收入用于碳去除

- 来源：stripe.com/climate
- 可信度：高

---

### 5. 对 AI 的公开立场

**地位**：创始人（Patrick 参与）

**Stripe 的 AI 战略**：
- Stripe 支持多家 AI 公司（OpenAI 等）
- 推出 AI 增强的欺诈检测功能
- Patrick 对 AI 持谨慎乐观态度

**公开言论**（间接来源）：
- 关注科学家对 AI 的看法
- 担心"AI 寒冬"周期性现象
- 对 AI 的长期影响保持关注

**投资/支持**：
- Stripe 支持的 AI 相关公司包括 OpenAI 等
- Progress Studies 关注 AI 对科学进步的影响

- 来源：媒体报道、Stripe 官方
- 可信度：中（缺少 Patrick 直接长篇论述）

---

### 6. 对 Crypto 的公开立场

**观察**：
- patrickcollison.com/crypto 页面存在但内容极少
- 仅有一条指向 Stripe 博客的链接

**Stripe 的立场**：
- Stripe 早期支持加密货币支付
- 2018年暂停加密货币支持（波动性、效率问题）
- 2024年重新支持加密货币（USDC 等稳定币）

**推测**：
- Patrick 个人对 crypto 持较低调态度
- 未将其作为核心关注点
- 与他对"成本病"、"科学进步"的热情形成对比

- 来源：patrickcollison.com/crypto、Stripe 博客
- 可信度：中

---

### 7. 定价决策

**背景**：
- Stripe 从未公开详细讨论定价策略
- 核心定价：2.9% + $0.30 每笔交易（与美国主流支付处理费率一致）

**推断逻辑**：
1. **简单透明**：一刀切定价，无隐藏费用
2. **行业标准**：不试图通过低价撬动市场
3. **价值导向**：通过产品体验而非价格竞争

**扩张策略**：
- 收购 Paystack（非洲市场，约2亿美元）
- 收购 TaxJar（税务计算，约2亿美元）
- 扩展产品线（Billing、Atlas、Climate、Press）

- 来源：Stripe 官方、媒体报道
- 可信度：中

---

### 8. 裁员决策（2022年11月）

**背景**：
- 2022年科技股大跌，经济不确定性增加
- Stripe 在疫情期间大幅扩张

**决策**：
裁员约14%（约1100人）

**Patrick 的裁员信核心内容**：
- 承认预测错误：疫情期间过度招聘
- 对错误负责
- 解释原因：经济下行、通胀、能源价格等

**外部评价**：
- 裁员信被认为是"标准模板"，与 Meta 等公司类似
- 诚实承认错误，但未特别出众
- 显示 Patrick 愿意公开承认决策失误

**决策模式**：
- 在宏观环境改变时快速调整
- 公开承担责任
- 不掩饰过去的错误

- 来源：Stripe 内部信、媒体报道
- 可信度：高

---

### 9. 撤回工作录用事件（2021年底）

**背景**：
- 2021年底科技招聘高峰
- Stripe 因"招聘问题"撤回部分已发出的工作录用

**批评**：
- 对候选人造成严重影响（可能已辞去原工作）
- 招聘流程管理失误
- 大公司应有更审慎的招聘承诺

**Patrick 的回应**：
在裁员信中承认了招聘过度的问题

**教训**：
- 招聘决策需要更谨慎的预测
- Offer 的承诺性质需要被尊重
- 快速增长与负责任招聘之间的平衡

- 来源：Protocol 报道、Hacker News
- 可信度：高（媒体报道确认）

---

### 10. 城市投票立场（旧金山 Proposition C）

**背景**：
- 旧金山 Proposition C：对大公司征收额外税收用于解决无家可归问题

**决策**：
Patrick 公开支持

**逻辑**：
- 愿意以公司资源支持公益
- 在科技CEO中属于进步派立场
- 与其关心社会问题的态度一致

**意义**：
- 显示他关注社会议题
- 愿意承担额外税收负担
- 区别于"纯粹利润导向"的科技CEO形象

- 来源：Stripe 官方博客、媒体报道
- 可信度：高

---

### 11. Progress Studies 倡议（2019年）

**背景**：
- 与 Tyler Cowen 合作
- 在 The Atlantic 发表文章

**决策逻辑**：
- 识别被忽视但重要的问题：什么促进了进步？
- 用有分量的方式提出
- 建立社区和资源推动进展

**行动**：
1. 发表宣言式文章
2. 建立问题和资源页面（patrickcollison.com/progress）
3. 支持 Works in Progress 杂志
4. Mark Zuckerberg 采访 Patrick 和 Tyler 讨论 Progress Studies

**影响**：
- 引发广泛讨论
- 催生了新的学者社区
- 成为 Patrick 思想遗产的重要部分

**决策模式**：
- 识别知识空白
- 系统性填补（文章、社区、杂志）
- 长期投入而非一次性话题

- 来源：patrickcollison.com/progress、The Atlantic
- 可信度：高

---

## 十、个人投资（天使投资）

**注**：Patrick 的个人投资公开披露有限。以下是基于公开来源的推测。

### 已知参与/支持的项目：
1. **Fast Grants** - 科研资助
2. **Arc Institute** - 生物医学研究
3. **CA YIMBY** - 住房政策
4. **Charter Cities Institute** - 实验性城市
5. **Works in Progress** - 在线杂志
6. **Stripe Press** - 出版（公司项目）

### 投资风格推断：
- 关注"进步"主题：科学、城市、住房
- 长期导向：非短期财务回报
- 亲自参与：不仅是资金，更是思想贡献

- 来源：patrickcollison.com/about
- 可信度：高

---

## 十一、待进一步研究的方向

1. **具体融资轮次细节** - 哪些投资人、什么条款
2. **收购决策过程** - Paystack、TaxJar 等估值方法
3. **与竞争对手的互动** - PayPal、Braintree 等
4. **内部文化变化** - 从2人到几千人的演变
5. **个人投资的完整清单** - 天使投资项目
6. **AI 公开演讲** - 可能存在的会议演讲
7. **与 John Collison 的具体分工** - 需要更多采访资料
8. **法律和监管谈判** - 支付行业的复杂性处理
9. **国际扩张决策** - 哪些国家、何时、为什么
10. **加密货币立场演变** - 从支持到暂停到恢复的原因

---

## 十二、关键语录补充

### 关于阅读
> "I really think people should be much more biased towards older books than they are."
> "You should mostly ignore the books being published each year..."

### 关于学习
> "Don't stress out too much about how valuable the things you're going deep on are... but don't ignore it either."

### 关于年轻人
> "People who did great things often did so at very surprisingly young ages. (They were grayhaired when they became famous... not when they did the work.) So, hurry up!"

### 关于独立思考
> "A large fraction of what people around you believe is mistaken. Internalize this and practice coming up with your own worldview."

### 关于正常路径
> "Make sure that the things you're pursuing are weird things that you want to pursue, not whatever the standard path is. Heuristic: do your friends at school think your path is a bit strange? If not, maybe it's too normal."

---

*此文档持续更新。Patrick Collison 的思维特点：极度理性、承认运气、长期导向、阅读驱动、区分可逆/不可逆决策、数据密集型论证。*

**更新日志**：
- 2026-04-24：初稿
- 2026-04-25：增加离开爱尔兰决策、远程工作决策、个人投资与慈善、AI/Crypto立场、裁员决策、Progress Studies倡议等