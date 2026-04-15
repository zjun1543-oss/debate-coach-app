# 更新日志 (CHANGELOG)

## [v1.0.3] - 2026-04-15

### 🎉 初始发布版本

**当前最新版本**: v1.0.3
**发布日期**: 2026-04-15
**GitHub**: https://github.com/zjun1543-oss/debate-coach-app

---

### ✨ 核心功能

#### 1. 双训练模式
- **教学模式 (Tutorial Mode)**: 苏格拉底式引导，AI 作为教练
  - 可选训练重点: Clarity (清晰表达) / Rebuttal (有效反驳) / Arguments (构建论点)
  - 引导式提问，不直接完成学生论点

- **对练模式 (Sparring Mode)**: 纯辩论对手，AI 作为对手
  - 期间不进行任何教学
  - 点击 "End Sparring" 生成复盘报告

#### 2. 语音交互
- **语音识别 (STT)**: 实时转写，支持停顿累积
- **语音合成 (TTS)**: 可选择多种自然语音
- **打断功能**: 按下语音键自动打断 AI 说话
- **一键发送**: 第一次点击开始录音，第二次点击停止并发送

#### 3. DeepSeek API 集成
- API Key 本地存储 (localStorage)
- 自动连接测试

#### 4. 话题管理
- 内置经典 THBT 辩题库
- 自定义话题输入
- 本地缓存保存话题

#### 5. 复盘报告系统
- **Aura Check (气场仪表盘)**: 流畅度 / 脱水率 / 语速
- **Logic Check (逻辑体检)**: 证据链诊断
- **Golden Rewrite (金句重写)**: 原始表达 vs 升级版本

---

### 🔄 版本更新记录

#### v1.0.3 → v1.0.4 (待开发)
- [ ] TODO: 未来功能

#### v1.0.2 → v1.0.3
**修复**: 语音输入累积显示
- 修复语音识别在停顿后丢失前面内容的问题
- 现在所有说的话都会累积显示，直到手动停止
- 停顿不再影响内容保留

#### v1.0.1 → v1.0.2
**重构**: 简化 UI
- 移除绿色实时转写框
- 语音输入直接显示在输入框中
- 界面更简洁，专注对话

#### v1.0.0 → v1.0.1
**功能**: 手动发送确认
- 移除语音自动发送功能
- 用户可以查看和编辑语音转写内容后再发送

#### 初始版本 v1.0.0
**核心功能发布**
- 教学模式和对练模式
- DeepSeek API 集成
- 语音识别和合成
- 话题管理和缓存
- 复盘报告系统

---

### 🛠️ 技术栈

- **前端**: HTML5 + CSS3 + Vanilla JavaScript
- **语音 API**: Web Speech API (SpeechRecognition + SpeechSynthesis)
- **AI 模型**: DeepSeek API
- **数据存储**: LocalStorage (API Key + 自定义话题)
- **版本控制**: Git + GitHub

---

### 📂 项目结构

```
debate-coach-app/
├── index.html          # 主应用文件 (单文件)
├── README.md           # 使用说明文档
├── CHANGELOG.md        # 本更新日志
└── backup/             # 版本备份目录
    ├── debate-coach-v1.0.0-*.html
    ├── debate-coach-v1.0.1-*.html
    ├── debate-coach-v1.0.2-*.html
    └── debate-coach-v1.0.3-*.html
```

---

### 🚀 本地运行

```bash
# 方法一: 直接打开
open index.html

# 方法二: 使用本地服务器
cd ~/Desktop/debate-coach-app
python3 -m http.server 8000
# 访问 http://localhost:8000
```

---

### 🔑 配置要求

1. **DeepSeek API Key**: 从 https://platform.deepseek.com/ 获取
2. **浏览器**: 推荐 Chrome 或 Edge (完整语音支持)
3. **麦克风权限**: 需要授予浏览器麦克风访问权限

---

### 📝 AI 角色设定 (Persona)

- **年龄**: 24岁
- **身份**: WUDC 冠军辩论教练
- **性格**: 温暖、幽默、逻辑严密
- **语言风格**: 高度口语化，拒绝 AI 腔
- **反馈原则**: 先提供情绪价值，再进行逻辑打击

---

### 🎯 教学方法论

基于 **Bo Seo 辩论方法论**:
1. **Aura First**: 气场优先，关注表达自信度
2. **Logic Layer**: 确保论点包含 Warrant (为什么真实) + Impact (为什么重要)
3. **Real Talk**: 温和指出冗余词 (um, uh, like)

---

### 🐛 已知问题

- [ ] Safari 浏览器语音识别支持有限
- [ ] Firefox 不支持语音识别
- [ ] 需要稳定的网络连接

---

### 💡 未来计划

- [ ] 添加更多训练模式
- [ ] 支持多语言 (中文)
- [ ] 导出辩论记录
- [ ] 统计数据面板
- [ ] 多人辩论模式

---

### 📞 支持

**问题反馈**: https://github.com/zjun1543-oss/debate-coach-app/issues

---

**最后更新**: 2026-04-15 23:14
**维护者**: zjun1543-oss
**AI 助手**: Claude Code
