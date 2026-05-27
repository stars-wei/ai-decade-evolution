# AI DECADE | 人工智能黄金十年演化史 (2016 - 2026)

[![GitHub license](https://img.shields.io/github/license/stars-wei/ai-decade-evolution?style=flat-square&color=blue)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/stars-wei/ai-decade-evolution?style=flat-square)](https://github.com/stars-wei/ai-decade-evolution/stargazers)
[![Tech Stack](https://img.shields.io/badge/Stack-HTML5%20%7C%20CSS3%20%7C%20Vanilla%20JS-orange?style=flat-square)](#)

本项目整理并全景展示了以 **2016 年** 为起点到 **2026 年** 间，人工智能（AI）发展黄金十年的演化路线与编年史。内容涵盖这十年间出现的颠覆性技术、框架、模型、公司、产品、核心人物、里程碑论文以及重大新闻。

同时，报告梳理了技术分支的演化脉络——有些分支不断茁壮壮大（如 Transformer、Diffusion、Agentic AI），而有些分支则在历史长河中转型或衰亡（如 RNN/LSTM、GAN、独立 AI 硬件）。

---

## 📂 项目文件结构 (File Structure)

```text
ai-decade-evolution/
├── index.html                           # 网页主程序 (毛玻璃交互式编年史单页)
├── style.css                            # 网页视觉样式表 (暗黑太空科技美学)
├── ai_evolution_history_2016_2026.md    # 核心文档：黄金十年演化史全景编年史报告
├── README.md                            # 项目说明文档
└── images/                              # AI 生成的主题艺术插图
    ├── banner.png                       # 顶部抽象神经网络进化横幅
    ├── era1.png                         # STAGE 01 深度强化学习与基石时代插画
    ├── era2.png                         # STAGE 02 生成式 AI 大爆发时代插画
    └── era3.png                         # STAGE 03 智能体与深度推理时代插画
```

---

## 🎨 网页设计与功能特色 (Webpage Features)

网页采用了现代前端设计美学，提供直观且富有艺术感的交互式历史浏览体验：

1. **太空暗黑视觉主题 (Space Dark Theme)**：背景选用极具深邃感的暗夜紫渐变，搭配荧光青（模型）、极光绿（技术）、魅影紫（框架）与暖金色（公司）等发光标签。
2. **毛玻璃拟态卡片 (Glassmorphism)**：时间轴节点和卡片拥有磨砂玻璃的半透明质感，并伴随柔和的侧边悬停光晕和上浮微动画。
3. **多维动态过滤 (Interactive Filtering)**：顶部的维度过滤器支持一键筛选“模型”、“技术/算法”、“框架/工具”或“公司/事件”，卡片隐现顺滑自然。
4. **滚动高亮追踪 (Scrollspy)**：顶部导航栏根据页面滚动进度，自动点亮当前阅读所处的历史阶段。
5. **图文并茂 (Artistic Illustrations)**：每个核心发展阶段都配有一张由 AI 图像模型生成的极具科幻感与逻辑线条美的专题插画。

---

## 🚀 本地快速预览 (How to Run)

该网页是一个**零依赖的纯静态项目**，无需搭建任何开发或服务器环境：

1. 将本仓库克隆至本地：
   ```bash
   git clone https://github.com/stars-wei/ai-decade-evolution.git
   ```
2. 进入目录并直接双击 **`index.html`** 文件，即可在任意主流浏览器（Chrome, Edge, Safari 等）中打开查看。

---

## 📈 AI 核心演化路线摘要 (Evolution Branches)

| 茁壮成长的绝对主线 (Growing Branches) | 式微 / 转型的技术分支 (Faded/Withered) |
| :--- | :--- |
| **Transformer 架构**：一统 NLP 与 CV 底层。 | **RNN / LSTM**：受限于无法并行计算和遗忘瓶颈。 |
| **Diffusion 扩散模型**：替代 GAN，主宰多模态生成。 | **GAN 生成对抗网络**：训练不稳定，且难与文本对齐。 |
| **推理时计算 (Test-Time Compute)**：依靠 CoT 突破瓶颈。 | **单一监督微调 (SFT)**：效率较低，正向 In-Context 演进。 |
| **Agentic AI (智能体)**：从单问单答进化为全闭环自主行动。| **独立 AI 硬件**：物理设备遭遇延迟痛点，转向系统级网关。 |

---

## 📝 授权说明 (License)

本项目采用 [MIT License](LICENSE) 开源协议。欢迎学习、参考或二次开发。
