# CLAUDE.md 标准模板

> 本文件由 ios-ai-dev skill 在 A1 节点自动生成，放在项目根目录。
> 每完成一个重大功能后更新。

---

```markdown
# CLAUDE.md

## 项目概述
[一句话：这个 App 是什么，解决什么问题]

## 技术栈
- 前端框架：Capacitor + React + TypeScript
- 后端：[Supabase / Firebase / 其他]
- 数据库：[PostgreSQL / Firestore / 其他]
- AI：[Claude / GPT / Gemini + 哪个 SDK]
- 部署：[App Store / TestFlight]

## Screen 列表
[按跳转关系排列，格式：Screen名 → Screen名]
- HomeScreen → PracticeScreen → ResultScreen
- HomeScreen → SettingsScreen

每个 Screen 一句话描述：
- HomeScreen：首页，入口和导航
- PracticeScreen：[做什么]
- ResultScreen：[做什么]

## 数据模型
[核心表和字段，类型要写清楚]

### 表名：[table_name]
| 字段 | 类型 | 说明 |
|------|------|------|
| id | uuid | 主键 |
| user_id | uuid | 关联 auth.users |
| created_at | timestamptz | 创建时间 |

## 格式约定
[AI 输出格式、枚举值等，改了要同步改 parser]
- 状态枚举：[值1 / 值2 / 值3]
- 数组格式：[说明]

## 付费逻辑
[积分 / 订阅 / IAP 规则]
- 产品 ID：[com.appname.xxx]
- 订阅周期：[monthly / yearly]
- 免费额度：[说明]

## 不能动的地方
[已稳定、不允许 AI 随意修改的逻辑，每次出问题就往这里加]
- [文件名 / 函数名]：[原因]

## 当前已知问题
[正在处理的 bug 或未完成的功能，完成后删掉]
- [ ] [问题描述]

## 数据库写入规则（所有写入必须遵守）
- 写入前过滤 \x00 等特殊字符
- 字段长度超限截断，不报错
- 用户未登录时直接 return，不写库
```
