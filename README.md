# Debate Coach AI - 使用说明

## 📋 项目简介

这是一款专为 12-14 岁初高中生设计的全英文辩论口语陪伴与训练智能体应用。

### 核心特性

- 🎤 **实时语音交互** - 使用浏览器原生语音识别和合成
- 📚 **教学模式** - 苏格拉底式引导，一步步构建论点
- ⚔️ **对练模式** - 纯粹辩论对手，结束后获得复盘报告
- 🧠 **Bo Seo 辩论方法论** - 专注 Warrant 和 Impact
- 💾 **本地数据存储** - API Key 和自定义话题自动保存

## 🚀 快速开始

### 1. 获取 DeepSeek API Key

1. 访问 [DeepSeek 官网](https://platform.deepseek.com/)
2. 注册/登录账号
3. 进入 API Keys 页面
4. 创建新的 API Key（格式: sk-xxxxx）

### 2. 启动应用

**方法一：直接打开（推荐）**
```bash
# 在 Finder 中双击 index.html 文件
```

**方法二：使用本地服务器**
```bash
# 进入项目目录
cd ~/Desktop/debate-coach-app

# Python 3
python3 -m http.server 8000

# 然后访问 http://localhost:8000
```

### 3. 配置应用

1. 在 "API Configuration" 区域输入你的 DeepSeek API Key
2. 点击 "💾 Save" 保存密钥（存储在浏览器本地）
3. 点击 "Test" 测试连接

## 🎯 使用指南

### 选择训练模式

#### 📚 教学模式 (Tutorial Mode)
- AI 角色是教练，使用苏格拉底式提问引导你
- 可选择训练重点：
  - **Clarity** - 清晰表达
  - **Rebuttal** - 有效反驳
  - **Arguments** - 构建论点

#### ⚔️ 对练模式 (Sparring Mode)
- AI 角色是对手，进行实战交锋
- 期间不进行任何教学
- 点击 "🏁 End Sparring" 查看复盘报告

### 配置辩论设置

1. **选择话题**
   - 从下拉菜单选择经典 THBT 辩题
   - 或输入自定义话题并保存

2. **选择立场**
   - Proposition (正方)
   - Opposition (反方)

3. **输入模式**
   - Voice (推荐) - 语音输入
   - Text - 文本输入

### 开始训练

1. 点击 "🚀 Start Session"
2. AI 会用充满鼓动性的语言开场
3. 使用语音或文字输入你的观点
4. 实时查看转写文本（绿色文本框）

### 语音控制

- **🔊 Sound On** - 开启 AI 语音播报
- **🔇 Sound Off** - 关闭语音播报
- **🔉 Test** - 测试语音
- **🔇 Stop Speaking** - 中断 AI 播报（当 AI 说话时出现）

### 查看复盘报告

对练模式结束后，点击 "🏁 End Sparring - 查看复盘" 获取：

**✨ Aura Check (气场仪表盘)**
- 流畅度星级
- 脱水率 (无冗余词比例)
- 语速评价

**🧠 Logic Check (逻辑体检)**
- 证据链诊断
- 逻辑漏洞标注

**👑 Golden Rewrite (金句重写)**
- 原始表达对比
- 升级版金句

## ⚙️ 系统要求

### 浏览器兼容性

| 浏览器 | 语音识别 | 语音合成 | 推荐度 |
|--------|----------|----------|--------|
| Chrome | ✅ | ✅ | ⭐⭐⭐⭐⭐ |
| Edge | ✅ | ✅ | ⭐⭐⭐⭐⭐ |
| Safari | ⚠️ | ✅ | ⭐⭐⭐ |
| Firefox | ❌ | ✅ | ⭐⭐ |

**推荐使用 Chrome 或 Edge 获得完整体验。**

### 网络要求

- 需要稳定的互联网连接
- 用于访问 DeepSeek API 和语音识别服务

## 🔒 数据安全

- API Key 存储在浏览器 localStorage 中
- 自定义话题保存在本地
- 对话内容不会上传到任何第三方服务器
- 仅与 DeepSeek API 通信用于生成 AI 回复

## 📝 辩论技巧提示

### AI 教练的教学风格

1. **先有气势，再有道理** - 注重表达的自信度
2. **逻辑剥洋葱** - 每次只解决一个逻辑点
3. **Warrant + Impact** - 每个论证必须包含这两个要素

### 减少冗余词

- 注意: um, uh, like, you know
- AI 会在冗余词过多时温和提醒

### 论证结构

```
Claim (主张) → Warrant (为什么是真的) → Impact (为什么重要)
```

## 🐛 故障排除

### 语音识别不工作

1. 确认使用 Chrome/Edge 浏览器
2. 检查麦克风权限
3. 检查网络连接

### API 调用失败

1. 确认 API Key 正确
2. 检查 DeepSeek 账户余额
3. 查看浏览器控制台错误信息

### 语音播报不工作

1. 确认声音已开启
2. 检查系统音量
3. 尝试点击 "Test" 按钮

## 📂 文件结构

```
debate-coach-app/
├── index.html    # 主应用文件（包含 HTML/CSS/JS）
└── README.md     # 本说明文档
```

## 🎓 学习资源

- **Bo Seo 辩论方法论**: 《Good Arguments》
- **THBT 辩论格式**: World Schools Debate Championship
- **演讲技巧**: TED 演讲分析

---

**版本**: 1.0.0
**更新日期**: 2026-04-15
**开发**: Claude Code

有问题？请检查浏览器控制台的错误信息。
