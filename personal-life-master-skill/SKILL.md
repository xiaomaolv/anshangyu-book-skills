```yaml
---
name: personal-life-master-skill
alias: 个人全域管控中枢
description: 统一接管【股票交易、学习计划、日常健身运动、乒乓球专项训练】四大业务模块，所有行为必须严格遵从内置刚性规则，AI仅依据规则输出方案、研判结果，禁止自主主观推演、自由发挥、随性优化规则
version: 1.1
update_date: 2026-07-30
trigger_words:
  股票类:
    - 股票分析
    - 个股操作
    - 建仓布局
    - 持仓风控
    - 盘面复盘
    - 价位研判
    - 止盈止损执行
  生活类:
    - 制定学习方案
    - 健身规划
    - 乒乓球训练指导
    - 训练复盘
    - 运动计划调整
scope: 个人投资交易管理 + 自我提升作息运动管理
hard_mode: true
---

# 模块一：股票交易管控体系（最高优先级刚性约束）
stock_system:
  # 1. 持仓池划分
  position_pool:
    main_hold_list:
      - 金发科技
      - 洛阳钼业
      - 银华创新药ETF
    watch_only_list:
      - 多氟多
      - 钒钛股份
      - 哈药股份

  # 2. 仓位刚性红线
  position_red_line:
    total_asset_rule:
      structural_bull: 总仓位上限50%，永久预留50%现金底仓
      weak_shock_market: 主线模糊、弱势震荡行情，总仓位强制≤30%
    single_variety_limit: 单只个股/单只ETF最高占用总资产12%
    trading_principle: 采用分批止盈+动态止损；禁止高开追入、禁止亏损补仓摊薄成本

  # 3. 标的分析规则
  target_analysis_frame:
    金发科技:
      core_business: 改性塑料、特种工程塑料、LCP材料、AI服务器配套材料、车用塑料原料
      focus_dimension:
        - 半年报业绩与一季度利润延续性
        - LCP、高温尼龙新材料放量情况
        - 原油价格、上游石化原料成本波动
      trading_property: 稳健修复型波段标的，只适合低吸，不参与涨停博弈
      hidden_risk: 中报业绩不及预期，容易出现估值回落
    洛阳钼业:
      core_business: 铜、钴、钼、钨有色金属资源龙头
      focus_dimension:
        - 铜、钴、钼价格走势
        - 全球宏观、美联储政策、大宗商品周期
        - 矿产储量、产能释放、生产成本
      trading_property: 周期品种，行情跟随大宗商品价格波动
      hidden_risk: 金属价格波动剧烈，不宜短线追涨
    银华创新药ETF:
      core_business: 创新药、CXO、医药研发全产业链指数基金
      focus_dimension:
        - 集采、医保谈判、医药行业政策变动
        - CXO订单、药企临床管线、行业盈利周期
        - 北向资金、避险资金板块流向
      trading_property: 中长期分批布局+波段止盈，拒绝短线爆炒
      hidden_risk: 政策收紧、研发不及预期会压制指数估值

  # 4. 交易执行标准
  execution_spec:
    build_position:
      rule1: 个股大涨后，次日高开禁止开仓、加仓
      rule2: 标准介入方式：回踩支撑位+分时企稳低吸
      rule3: 资金分2~3批建仓，不一次性满仓
      rule4: 仅持仓浮盈才可加仓，亏损状态严禁补仓
    take_profit:
      rule1: 短线盈利8%~12%进行部分减仓
      rule2: 触碰压力位、放量滞涨时分批止盈
      rule3: 利好兑现不恋战鱼尾行情
    stop_loss:
      rule1: 跌破关键支撑立即止损
      rule2: 亏损单子禁止加仓摊成本
      rule3: 账户大幅回撤优先降仓防守，不硬扛

  # 5. 禁止行为列表
  forbidden_behavior:
    - 涨停、大阳线之后重仓追入
    - 被套持续加仓摊薄成本
    - 单个标的仓位超过总资产12%
    - 未设置支撑、止损位随意建仓
    - 把短线题材炒作当作长期重仓逻辑
    - 脱离基本面，仅凭K线涨跌交易

  # 6. 固定复盘输出格式
  review_output_template:
    1. 当前持仓：金发科技、洛阳钼业、银华创新药ETF
    2. 标的状态：强势 / 震荡 / 走弱
    3. 关键价位：支撑位、压力位、止损位
    4. 操作计划：持有 / 减仓 / 低吸 / 观望
    5. 仓位检查：核验总仓位、单个标的仓位是否合规
    6. 纪律检查：排查追涨、亏损补仓、重仓等违规行为

# 模块二：学习、运动、乒乓球管理
life_management_system:
  execution_rule: 该模块原有规则保持不变，严格按照原有制度执行落地