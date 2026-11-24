# mkt

电商调研与独立站 Skills。

这套工作流用于回答三个业务问题：用户提出了哪些真实需求，哪个细分商品值得先花钱测试，以及访客在网站哪一步遇到困难。

## 3 个可独立安装的 skills

| Skill | 适合什么时候用 | 一句调用示例 |
| --- | --- | --- |
| [用户需求逐条审核](skills/customer-request-audit/SKILL.md) | 手上有评论、帖子或访谈，需要区分求购、旁人推荐和已购体验，算清独立请求数 | `$customer-request-audit 审核这批论坛讨论，按购买对象统计独立请求，列出分母并保留原话定位。` |
| [小众选品初筛](skills/niche-product-screening/SKILL.md) | 正在比较国家、人群和 SKU，需要决定下一笔打样或试卖预算投给谁 | `$niche-product-screening 对比这两款商品在墨西哥的需求、当地成交证据和履约成本，设计一次低成本付费测试。` |
| [独立站转化路径复查](skills/storefront-journey-review/SKILL.md) | 有网站、页面录屏或截图，需要定位买家走到哪一步会卡住，改版后怎么验收 | `$storefront-journey-review 从手机首页走到把指定规格加入购物车，列出优先级、白话改法和复测条件。` |

## 安装到 Codex

克隆或下载此仓库后，进入仓库根目录，把需要的子目录复制到个人 skills 目录。例如安装用户需求审核：

```sh
dest="${CODEX_HOME:-$HOME/.codex}/skills"
mkdir -p "$dest"
cp -Ri skills/customer-request-audit "$dest/"
```

安装其余 skill 时，替换最后一行的目录名。新开一个 Codex 会话，输入表中的调用示例并附上材料。每个 skill 的 `SKILL.md` 都含一个合成示例，可以先用示例核对输出。

## 2 份配套模板

- [短视频同品类对照](templates/video-cohort-comparison.md)适合已有逐条视频观察、想决定下一轮拍什么的团队。
- [单条社媒素材发布包](templates/social-post-brief.md)用于将一条已有素材整理成可交给运营同事的发布稿。

模板可直接复制填写。仓库内示例均为演示用的虚构情境。
