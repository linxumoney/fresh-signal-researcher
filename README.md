# Fresh Signal Researcher：你要的是最近发生了什么，不是旧文章重新排序

研究“最近一个月”最容易犯的错，是把刚发布的旧事件、转述同一消息的十篇文章和没有日期的观点混在一起，然后得出一个看似热闹的趋势。

`fresh-signal-researcher` 是一个面向市场、产品、内容和战略研究的开源 Agent Skill。它使用明确的滚动时间窗，区分事件日期与发布日期，并把事实、社区情绪和分析推断分层呈现。

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

## 方法参考

本项目独立实现。近期多源研究问题域参考了 [mvanhorn/last30days-skill](https://github.com/mvanhorn/last30days-skill)，该项目采用 MIT License。本项目没有复用其抓取脚本、供应商接口、输出法则、版本协议、缓存逻辑或文字。

## License

MIT License。
