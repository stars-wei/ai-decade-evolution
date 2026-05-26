# 人工智能十年演化史：2016-2026

> 作者：Codex、Stars Wei。声明：本文由 Codex 与 Stars Wei 共同创作，Codex 为作者之一，Stars Wei 为共同作者。

> 范围说明：截至 2026-05-26。本稿不是“穷尽互联网所有资讯”的数据库，而是按公开可核验资料整理出的关键节点路线图。能落实到日的事件按日写；只有月/年可核验的事件按月/年写。2016 年以前已经存在、但对 2016-2026 十年产生决定性影响的技术，也放入“既有基础”。

## 0. 2016 年之前已经存在的底座

- 1950s-1980s：符号主义 AI、专家系统、搜索、规划、博弈树、反向传播等奠基；但专家系统后期维护成本高、泛化差，成为之后“衰退分支”的典型。
- 1997-05-11：IBM Deep Blue 战胜 Garry Kasparov，代表搜索 + 专用评估函数在封闭规则博弈中的胜利。
- 2006-2012：深度学习复兴。Hinton、Bengio、LeCun 等人的神经网络路线重新成为主流。
- 2012-09：AlexNet 在 ImageNet 上大幅领先，GPU + 大数据 + 深度卷积网络成为视觉 AI 的主干。
- 2013-2014：word2vec、seq2seq、注意力机制、GAN 出现，为后来的大模型、多模态和生成式 AI 铺路。
- 2015：TensorFlow 开源；OpenAI 成立；ResNet 出现；深度强化学习在 Atari 等任务上出圈。

## 1. 年表：从 AlphaGo 到 Agent

### 2016：深度强化学习的公众时刻，框架生态开始成形

- 2016-03-09 至 2016-03-15：DeepMind AlphaGo 与李世石五番棋，AlphaGo 4:1 获胜。意义不是“围棋结束”，而是深度学习 + 蒙特卡洛树搜索 + 强化学习证明可处理高维复杂决策。
- 2016：TensorFlow、Caffe、Theano、Torch、MXNet、CNTK 等框架竞争。最后 TensorFlow 和 PyTorch 路线胜出，Theano/CNTK 等逐渐退出中心。
- 2016：监督学习、CNN、RNN/LSTM、强化学习是主流叙事；NLP 仍以循环网络、注意力、统计特征和任务微调为主。
- 2016：中国 AI 创业潮继续升温，商汤、旷视、依图、云从等视觉公司走强；这一分支在安防、金融、手机视觉里壮大，但后来受隐私、监管、商业化和硬件周期约束，热度下降。

### 2017：Transformer 诞生，政策与产业进入战略竞争

- 2017-06-12：Google 研究者发布论文 *Attention Is All You Need*，提出 Transformer。它抛弃 RNN/CNN 主干，用自注意力并行建模序列，成为之后 GPT、BERT、T5、ViT、扩散模型文本编码器和多模态模型的核心。
- 2017-07-20：中国国务院发布《新一代人工智能发展规划》，将 AI 上升为国家战略，提出到 2030 年成为世界主要 AI 创新中心。
- 2017：AlphaGo Zero 展示从自我博弈中学习，强化学习路线继续辉煌，但走出棋类和模拟环境后，样本效率、可控性和现实成本成为瓶颈。
- 2017：PyTorch 发布后迅速在研究界流行，动态图和易调试体验开始压过 TensorFlow 1.x 的静态图体验。

### 2018：预训练 + 微调成为 NLP 主范式

- 2018-06：OpenAI 发布 GPT-1，证明 Transformer 解码器可通过大规模无监督预训练再迁移到下游任务。
- 2018-10-11：Google 发布 BERT 论文，双向 Transformer + Masked Language Modeling 将 NLP 带入“预训练模型 + 少量任务微调”时代。
- 2018：ELMo、ULMFiT、BERT、GPT 共同推动“特征工程/任务专用模型”退潮。
- 2018：AutoML、NAS 热度上升，但昂贵搜索成本和可复现性问题让它没有成为大模型时代的主路线。

### 2019：生成式语言模型显露社会风险

- 2019-02-14：OpenAI 发布 GPT-2，但最初没有发布完整权重，理由是担心滥用。这是“模型能力 + 发布治理”首次成为大众议题。
- 2019-11：OpenAI 发布完整 GPT-2。开放发布与安全延迟发布的张力成为后续每个前沿模型都要面对的问题。
- 2019：Hugging Face Transformers 生态快速成长，NLP 模型复用、分享、微调门槛大幅下降。
- 2019：BERT 系列、RoBERTa、XLNet、T5 等模型竞争，NLP 仍主要是“编码器理解任务”和“基准榜单”驱动。

### 2020：规模定律与少样本学习

- 2020-05-28：OpenAI 发布 GPT-3 论文，175B 参数、少样本/零样本能力让“提示词”成为新的交互方式。
- 2020：Scaling Laws 论文将“更多数据、更多参数、更多计算”变成工程路线；这一路线壮大为今天的算力、数据中心、GPU、集群训练产业链。
- 2020-11：AlphaFold2 在 CASP14 中取得突破，AI for Science 从示范走向实用。
- 2020：强化学习仍重要，但从“大众主线”退到 RLHF、机器人、游戏、自主系统、推理模型训练等更具体位置。

### 2021：多模态、代码模型、科学模型

- 2021-01-05：OpenAI 发布 CLIP 和 DALL-E。CLIP 让文本-图像对齐成为通用能力，DALL-E 展示文本生成图像。
- 2021-06-29：GitHub Copilot 技术预览发布，AI 编程从研究走向 IDE 工作流。
- 2021-07-15：AlphaFold2 论文发表于 Nature；2021-07-22，DeepMind/EMBL-EBI 发布 AlphaFold 蛋白结构数据库。
- 2021：扩散模型开始取代 GAN 成为高质量图像生成主线；GAN 仍用于特定视觉生成，但“文本到图像”的主舞台逐渐转向 diffusion。

### 2022：生成式 AI 爆发年

- 2022-04：OpenAI 发布 DALL-E 2，图像生成质量与可控性大幅提升。
- 2022-07-12：Midjourney 进入开放 beta，审美化图像生成迅速破圈。
- 2022-08-22：Stable Diffusion 公开发布，开源/开放权重图像生成生态爆发，LoRA、ControlNet、DreamBooth 等社区技术形成庞大支流。
- 2022-11-30：OpenAI 发布 ChatGPT。关键变化不是单个模型指标，而是聊天界面 + 指令微调 + RLHF 使大模型成为普通人的日常工具。
- 2022：Web3/元宇宙叙事退潮，资本与人才大量转向生成式 AI。

### 2023：大模型平台化、开源权重崛起、监管启动

- 2023-02-24：Meta 发布 LLaMA，研究许可模型泄露后催生 Alpaca、Vicuna、llama.cpp、量化和本地模型浪潮。
- 2023-03-14：OpenAI 发布 GPT-4，显著提升推理、编码、可靠性和多模态输入能力。
- 2023-03-16：百度发布文心一言 ERNIE Bot，成为中国大厂追赶 ChatGPT 的标志事件。
- 2023-04：阿里发布通义千问/Qwen beta，后来形成中国最重要的开放模型家族之一。
- 2023-07-11：Anthropic 发布 Claude 2，长上下文和安全训练成为差异化方向。
- 2023-07：Meta 发布 Llama 2 并允许商业使用，开源权重路线真正产业化。
- 2023-10：Moonshot AI 推出 Kimi，以长上下文中文助手切入。
- 2023-11：OpenAI 董事会风波，Sam Altman 被短暂罢免后回归，显示前沿 AI 公司治理与商业化之间的张力。
- 2023-12-06：Google 发布 Gemini 1.0，DeepMind 与 Google Research 合流后的多模态基础模型正式登场。

### 2024：多模态实时化，长上下文、开源和法规并进

- 2024-02：Google 发布 Gemini 1.5，百万级上下文成为前沿模型竞争点。
- 2024-02：OpenAI 预览 Sora，视频生成进入大众视野。
- 2024-03-04：Anthropic 发布 Claude 3 系列，Opus、Sonnet、Haiku 明确分层，长文档和视觉理解增强。
- 2024-03-13：欧洲议会通过 EU AI Act，风险分级、透明度、基础模型义务成为监管模板。
- 2024-04-18：Meta 发布 Llama 3 8B/70B，开放权重模型继续追近闭源模型。
- 2024-05-13：OpenAI 发布 GPT-4o，文本、视觉、语音实时交互成为主叙事。
- 2024-06：Anthropic 发布 Claude 3.5 Sonnet，编程和复杂任务能力受到开发者欢迎。
- 2024-12-09：OpenAI 向付费用户发布 Sora。此时视频生成赛道已更拥挤，Runway、Pika、Kling、Luma 等成为重要竞争者。

### 2025：推理模型、低成本冲击、Agent 产品化

- 2025-01-20：DeepSeek 发布 DeepSeek-R1，开源推理模型以较低成本冲击市场，引发关于训练成本、蒸馏、算力壁垒和中国 AI 能力的全球讨论。
- 2025-01-23：OpenAI 发布 Operator 研究预览，浏览器操作型 agent 成为产品方向。
- 2025-02-02：OpenAI 发布 Deep Research，面向多步资料检索、阅读和报告生成。
- 2025-02-24：Anthropic 发布 Claude 3.7 Sonnet，称其为混合推理模型，并推出 Claude Code。
- 2025-03-25：Google 发布 Gemini 2.5 Pro Experimental，显式强化“thinking model”路线。
- 2025-04-14：OpenAI 发布 GPT-4.1 API 系列，强调编码、指令跟随和长上下文。
- 2025-04-16：OpenAI 发布 o3 和 o4-mini，推理模型开始内置工具使用、图像理解、搜索/代码/文件分析等能力。
- 2025-05-22：Anthropic 发布 Claude Opus 4 和 Sonnet 4，突出长时间编码、agent 和复杂任务。
- 2025-08-07：OpenAI 发布 GPT-5，统一快速回答与深度思考路线，替代 GPT-4o、o3、o4-mini、GPT-4.1 等多个前代 ChatGPT 模型。
- 2025：AI 编程成为最先大规模落地的“生产力杀手级场景”：Cursor、GitHub Copilot、Claude Code、Codex、Cline、Devin 类产品形成竞争。

### 2026：模型走向系统，竞争从“聊天”转向“工作流/代理/科学”

- 2026-02-12：Google 发布 Gemini 3 Deep Think，进一步面向科学、工程和复杂推理。
- 2026-04：Anthropic 系统卡列出 Claude Opus 4.7 等 2026 模型更新，Claude 家族继续强化 coding/agent/safety。
- 2026-04-23：OpenAI 发布 GPT-5.5；2026-04-24 API 可用，强调编码、计算机使用、研究和复杂文档/表格工作。
- 2026-05-19：Google I/O 2026 继续把 Gemini 深度嵌入 Search、YouTube、Android、XR/眼镜和订阅服务。
- 2026 截至 05-26：前沿竞争焦点从单一聊天机器人转向：模型路由、工具调用、浏览器/电脑使用、长上下文记忆、代码代理、企业知识库、科学发现、安全评测和监管前置测试。

## 2. 技术路线的兴衰

### 壮大的分支

- Transformer：从 NLP 架构变成通用序列/多模态/代理系统底座。
- 预训练基础模型：从 BERT/GPT 发展为 LLM、VLM、音视频模型和统一多模态模型。
- 扩散模型：从图像生成壮大到视频、3D、音频、编辑和设计工具。
- AI for Code：从 Copilot 自动补全发展为代码库理解、自动修 bug、测试、重构和长时 agent。
- AI for Science：AlphaFold 带动蛋白、材料、药物、天气、数学和实验设计。
- 开放权重生态：Llama、Mistral、Qwen、DeepSeek、Kimi 等形成与闭源 API 并行的路线。
- Agent/工具调用：从 function calling、ReAct、AutoGPT 实验，走向 Operator、Deep Research、Claude Code、Codex 等产品。

### 退潮或边缘化的分支

- 传统专家系统：可解释但脆弱，维护成本高，未能适应开放世界。
- 纯规则聊天机器人：被大语言模型和检索增强生成取代。
- RNN/LSTM 作为 NLP 主干：仍在部分低延迟/时序场景存在，但中心位置被 Transformer 取代。
- GAN 作为通用图像生成主线：被扩散模型压过，但仍在特定实时生成、风格迁移、数据增强中存在。
- 早期 AutoML/NAS 热潮：没有消失，但被更粗暴有效的规模化预训练、模型蒸馏和工程调参吸收。
- 早期 AutoGPT 式 agent：概念重要，但未经约束的循环代理不稳定；后来被工具权限、工作流、评测、沙箱和人工确认机制重构。

## 3. 公司、人物与产品版图

- OpenAI：Sam Altman、Greg Brockman、Ilya Sutskever、Mira Murati 等；产品线从 GPT、DALL-E、Whisper、ChatGPT、GPT-4、Sora、o 系列、Operator、Deep Research 到 GPT-5/5.5。
- Google DeepMind：Demis Hassabis、John Jumper、Pushmeet Kohli 等；路线包括 AlphaGo、AlphaFold、Gemini、AI for Science 和搜索/Android/Workspace 集成。
- Anthropic：Dario Amodei、Daniela Amodei、Jared Kaplan 等；路线是 Claude、Constitutional AI、长上下文、安全分级、Claude Code。
- Meta AI：Yann LeCun、Joelle Pineau、FAIR 团队；最大影响是 Llama 开放权重生态。
- NVIDIA：Jensen Huang；从 GPU 供应商变成 AI 基础设施核心公司，CUDA、H100/B系列、网络、推理栈和数据中心构成算力底座。
- Microsoft/GitHub：Azure OpenAI、Copilot、Office Copilot、GitHub Copilot，把生成式 AI 嵌进企业软件。
- 中国公司：百度文心、阿里 Qwen、腾讯混元、字节豆包、智谱 GLM、月之暗面 Kimi、DeepSeek 等，形成中文、开源权重、长上下文和低成本推理路线。

## 4. 一句话总路线

2016-2026 的 AI 演化可以概括为：

> 从“专用模型解决专用任务”，走向“通用基础模型 + 多模态输入输出 + 工具调用 + 长上下文/记忆 + 可执行代理 + 行业工作流”。

更细一点：

1. 2016-2017：深度学习证明复杂决策能力，Transformer 出现。
2. 2018-2020：预训练、规模定律、少样本学习形成语言模型主线。
3. 2021-2022：多模态、扩散模型、代码模型和 ChatGPT 把 AI 推向大众。
4. 2023-2024：闭源前沿模型与开放权重模型双线竞争，监管启动，AI 进入产品平台。
5. 2025-2026：推理模型和 agent 化系统成为核心，竞争从“谁会聊天”转向“谁能完成复杂工作”。

## 5. 主要参考来源

- AlphaGo vs Lee Sedol：Wikipedia、TechCrunch、The Guardian 对 2016-03-09 至 03-15 比赛记录。
- Transformer：Vaswani et al., *Attention Is All You Need*, arXiv, 2017-06-12.
- BERT：Devlin et al., *BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding*, arXiv, 2018-10-11.
- GPT-2：OpenAI, “Better language models and their implications”, 2019-02-14.
- GPT-3：OpenAI, “Language Models are Few-Shot Learners”, 2020-05-28.
- CLIP/DALL-E：OpenAI, “CLIP: Connecting text and images”, 2021-01-05.
- GitHub Copilot：GitHub Blog, “Introducing GitHub Copilot”, 2021-06-29.
- AlphaFold：Nature, “Highly accurate protein structure prediction with AlphaFold”, 2021-07-15；DeepMind/EMBL-EBI AFDB, 2021-07-22.
- ChatGPT：OpenAI, “Introducing ChatGPT”, 2022-11-30.
- GPT-4：OpenAI, “GPT-4”, 2023-03-14.
- Gemini：Google Blog, “Introducing Gemini”, 2023-12-06；Gemini 1.5, 2024-02；Gemini 3/Deep Think, 2025-2026.
- Claude：Anthropic Claude 2/3/3.7/4 announcements and system cards, 2023-2026.
- Llama：Meta AI Llama/Llama 2/Llama 3 announcements, 2023-2024.
- EU AI Act：European Parliament/Council AI Act records, 2024.
- OpenAI 2025-2026：Operator, Deep Research, GPT-4.1, o3/o4-mini, GPT-5, GPT-5.5 official announcements.
- 中国 AI：Stanford DigiChina translation of China’s 2017 AI plan；Baidu ERNIE Bot 2023；Alibaba Qwen/Tongyi Qianwen 2023；Moonshot/Kimi 2023；DeepSeek-R1 2025.
