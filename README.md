# Fresh Signal Researcher：最近 30 天趋势、竞品与市场信号研究 Skill

研究“最近一个月”最容易犯的错，是把刚发布的旧事件、转述同一消息的十篇文章和没有日期的观点混在一起，然后得出一个看似热闹的趋势。

`fresh-signal-researcher` 是一个面向市场、产品、内容和战略团队的开源近期趋势与竞品研究 Agent Skill。它研究最近 7、14、30 或 90 天的真实变化，区分事件日期和发布日期、原始来源和重复转述、事实和社区情绪。兼容 Codex、Claude Code、Cursor 和 OpenCode。

## 使用示例

```text
用 $fresh-signal-researcher 调研过去 30 天 AI 视频工具的变化。
重点看真实产品更新、用户抱怨和购买意向，附每条信号的事件日期。
```

## 默认输出

- 时间窗和查询范围
- 已确认的新事件
- 多来源反复出现的信号
- 热度与真实动量的区别
- 反例、沉默信号和数据缺口
- 接下来值得验证的问题

## 安装

```bash
cp -R skills/fresh-signal-researcher ~/.codex/skills/
```

## 适用场景

- 最近 30 天行业趋势、产品更新和技术变化
- 竞品动态、版本发布、定价调整和用户迁移信号
- Reddit、YouTube、Hacker News、GitHub 等社区反馈研究
- 内容选题、热点判断和用户真实痛点发现
- 区分一次性热搜、营销传播和持续市场动量

## 常见问题

### 为什么要区分事件日期和发布日期？

一篇文章可能刚发布，但讲的是几个月前的事件。Skill 会把这类内容标为“旧事件的新报道”，避免污染近期趋势判断。

### 多篇媒体报道算多个信号吗？

不一定。如果都来自同一公告，会合并成一个事件；只有相互独立的一手证据才会提高置信度。

### 能保证覆盖所有社交平台吗？

不能。输出会说明实际访问的来源、限制和样本偏差，不会虚构帖子、互动量或平台覆盖。

## 方法参考

本项目独立实现。近期多源研究问题域参考了 [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill)，该项目采用 MIT License。本项目没有复用其抓取脚本、供应商接口、输出法则、版本协议、缓存逻辑或文字。

## License

MIT License。

## 商业授权

个人学习、研究、测试和非商业使用可以。商业使用请先联系 **linxu.money@gmail.com** 获得授权，详见 [COMMERCIAL-LICENSING.md](COMMERCIAL-LICENSING.md)。

