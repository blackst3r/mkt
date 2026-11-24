# mkt · 产品研究与商业决策 Skills

这里有 **11 个可独立安装的 Codex skills** 和 **9 份可直接填写的模板**。用它们审核用户需求、决定下一笔打样预算、排查购买路径，或把客户的一句话需求写成能验收的试点。每个 skill 都附有虚构例子，读者可以对照自己的材料试用。

[选择 skill](#选择-skill) · [安装与调用](#安装与调用) · [模板目录](#模板目录) · [作者主页](https://blackst3r.github.io/)

## 选择 skill

| 我手上有什么问题？ | 使用哪个 skill | 拿到什么 |
| --- | --- | --- |
| 一百条评论里，有多少个独立购买请求？ | [用户需求逐条审核](skills/customer-request-audit/SKILL.md) | 可追溯的事件明细、角色和统计分母 |
| 两个细分商品，先为哪个打样？ | [小众选品初筛](skills/niche-product-screening/SKILL.md) | 具体到国家、人群和 SKU 的比较，以及最小付费测试 |
| 两家工厂都说能定制，谁能按这个规格交货？ | [供应商询价与验样](skills/supplier-sample-audit/SKILL.md) | 同条件报价表、能力证据和验样标准 |
| 大尺寸加价后，每笔订单还能多赚多少？ | [实物商品定价](skills/physical-product-pricing/SKILL.md) | 订单贡献、物流临界点及可承担的获客成本 |
| 访客选好了规格，为什么在下一步卡住？ | [独立站转化路径复查](skills/storefront-journey-review/SKILL.md) | 可复现的问题、修改优先级和验收步骤 |
| 用户已有手机或平板，专用硬件还值在哪里？ | [AI 硬件必要性验证](skills/hardware-value-test/SKILL.md) | 替代方案、剩余问题和低成本对照实验 |
| 什么问题能帮团队决定下一版产品做什么？ | [产品决策问卷](skills/product-decision-survey/SKILL.md) | 筛选题、分支逻辑、有效分母和分析办法 |
| 客户想试一个方案，双方如何判断试点是否成功？ | [客户 POC 范围与验收](skills/customer-poc-scope/SKILL.md) | 一页试点范围、演示路线和验收证据 |
| 报表有汇总数，分析还缺哪些明细？ | [业务数据缺口与补数规格](skills/data-gap-spec/SKILL.md) | 字段、粒度、关联键、时间窗和交接验收表 |
| 响应稿与附件是否逐条覆盖采购要求？ | [招投标响应审阅](skills/bid-response-review/SKILL.md) | 条款对照、缺失证据及需澄清的问题 |
| 同一款商品，给不同人群拍什么内容？ | [商品事实转内容简报](skills/product-content-brief/SKILL.md) | 有依据的卖点、场景、选题和拍摄简报 |

**一次选品可以这样串起来。** 先用「小众选品初筛」确定试卖对象，把同一规格交给「供应商询价与验样」，拿到报价后再用「实物商品定价」判断试卖价能否覆盖运费和获客成本。单个问题也可以直接使用其中任一项。

## 安装与调用

以 macOS 或 Linux 为例，下面安装「供应商询价与验样」。安装其他 skill 时，把最后一行的目录名替换为上表链接对应的目录名。

```sh
git clone https://github.com/blackst3r/mkt.git
cd mkt
dest="${CODEX_HOME:-$HOME/.codex}/skills"
mkdir -p "$dest"
cp -Ri skills/supplier-sample-audit "$dest/"
```

新开一个 Codex 会话，附上采购需求或现有报价，然后输入：

> $supplier-sample-audit 对比这两份定制收纳袋报价。目的地是同一个美国邮编，需要单件印图和白牌包装。请标出哪些费用还没报，样品到手后要验什么。

也可以下载仓库 ZIP，把所需的整个 skill 文件夹复制到个人 skills 目录。每个安装目录的入口文件都是 `SKILL.md`。

## 模板目录

模板可以复制到文档、表格或任务说明中直接填写。

| 使用场景 | 模板 |
| --- | --- |
| 外部市场和平台调研 | [众筹项目与发售链路](templates/crowdfunding-launch-audit.md) · [机会变化周报](templates/opportunity-delta-report.md) · [平台能力核查](templates/platform-capability-check.md) |
| 内容和用户运营 | [短视频同品类对照](templates/video-cohort-comparison.md) · [单条社媒素材发布包](templates/social-post-brief.md) · [生命周期邮件触发与停发](templates/lifecycle-email-rules.md) |
| 产品和分析交接 | [工业设计打样简报](templates/industrial-design-brief.md) · [dplyr 与 SQL 结果对账](templates/dplyr-sql-parity.md) |
| 个人作品与履历 | [用证据改写简历经历](templates/evidence-based-resume.md) |
