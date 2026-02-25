# AI资讯雷达 - 核心来源库 (v2.4 Full)

> 架构原则：
> 1. 所有来源必须保留 Web（用于 site: 搜索）
> 2. 有 RSS 的优先使用 RSS（实时模式）
> 3. 无 RSS 标记为 Search Only
> 4. 所有来源必须带 Tags
> 5. 支持实时 + 指定日期回溯双模式

---

# 🟢 Tier 1 - 官方模型与研究（强结构信号）

## OpenAI
- Web: https://openai.com/blog
- RSS: https://openai.com/blog/rss.xml
- Mode: Hybrid
- Tags: [Official, LLM, Research, API, Global]

## OpenAI Research
- Web: https://openai.com/research
- RSS: https://openai.com/research/rss.xml
- Mode: Hybrid
- Tags: [Official, Research, Frontier, Global]

## Anthropic
- Web: https://www.anthropic.com/news
- RSS: https://www.anthropic.com/news/rss.xml
- Mode: Hybrid
- Tags: [Official, LLM, Safety, Research, Global]

## Google DeepMind
- Web: https://deepmind.google/discover/blog/
- RSS: https://deepmind.google/discover/blog/rss.xml
- Mode: Hybrid
- Tags: [Official, Research, Gemini, Frontier, Global]

## Google AI Blog
- Web: https://blog.google/technology/ai/
- RSS: https://blog.google/technology/ai/rss/
- Mode: Hybrid
- Tags: [Official, Infrastructure, Applied AI, Global]

## Meta AI
- Web: https://ai.meta.com/blog/
- RSS: https://ai.meta.com/blog/rss/
- Mode: Hybrid
- Tags: [Official, Llama, Open Source, Research, Global]

## Mistral AI
- Web: https://mistral.ai/news
- RSS: https://mistral.ai/news/rss.xml
- Mode: Hybrid
- Tags: [Official, Open Source, Europe, LLM]

## Stability AI
- Web: https://stability.ai/blog
- RSS: https://stability.ai/blog/rss.xml
- Mode: Hybrid
- Tags: [Official, Image, Video, Audio, Open Source]

## Hugging Face Blog
- Web: https://huggingface.co/blog
- RSS: https://huggingface.co/blog/feed.xml
- Mode: Hybrid
- Tags: [Ecosystem, Open Source, Community, Global]

---

# 🟢 Tier 1B - 模型版本信号（结构化发布）

## Qwen (阿里通义千问)
- Web: https://qwen.ai/research
- Tags Feed: https://github.com/QwenLM/Qwen/tags.atom
- HF: https://huggingface.co/Qwen
- Mode: Hybrid
- Tags: [Official, Model-Release, Open Source, China, LLM]

---

# 🟡 Tier 2 - 权威科技媒体（高频，可聚合）

## TechCrunch AI
- Web: https://techcrunch.com/category/artificial-intelligence/
- RSS: https://techcrunch.com/category/artificial-intelligence/feed/
- Mode: Hybrid
- Tags: [Media, Startup, Funding, Global, LLM]

## The Verge AI
- Web: https://www.theverge.com/ai-artificial-intelligence
- RSS: https://www.theverge.com/rss/ai-artificial-intelligence/index.xml
- Mode: Hybrid
- Tags: [Media, Consumer AI, Policy, BigTech, Global]

## MIT Technology Review (AI)
- Web: https://www.technologyreview.com/topic/artificial-intelligence/
- RSS: https://www.technologyreview.com/topic/artificial-intelligence/feed
- Mode: Hybrid
- Tags: [Media, Research, Policy, DeepTech, Global]

## 机器之心
- Web: https://www.jiqizhixin.com/
- RSS: https://www.jiqizhixin.com/rss
- Mode: Hybrid
- Tags: [Media, LLM, Research, China, Open Source]

## 量子位
- Web: https://www.qbitai.com/
- RSS: https://www.qbitai.com/feed
- Mode: Hybrid
- Tags: [Media, LLM, Startup, China]

## 36Kr AI
- Web: https://36kr.com/information/technology
- RSS: https://36kr.com/feed
- Mode: Hybrid
- Tags: [Media, Startup, Funding, China]

---

# 🔵 Tier 3 - 中国模型厂商（非结构化，Search 优先）

## 字节跳动 Doubao
- Web: https://www.doubao.com/
- News: https://www.bytedance.com/news
- Mode: Search Only
- Tags: [Official, LLM, China, Consumer AI]

## 腾讯 Hunyuan
- Web: https://hunyuan.tencent.com/
- News: https://www.tencent.com/zh-cn/news.html
- Mode: Search Only
- Tags: [Official, LLM, China, Enterprise AI]

## 智谱 AI
- Web: https://www.zhipuai.cn/
- Mode: Search Only
- Tags: [Official, LLM, China]

## 月之暗面 Moonshot
- Web: https://moonshot.cn/
- Mode: Search Only
- Tags: [Official, LLM, China]

---

# 🟣 Tier 4 - 学术与前沿

## arXiv CS.AI
- Web: https://arxiv.org/list/cs.AI/recent
- RSS: http://export.arxiv.org/rss/cs.AI
- Mode: Hybrid
- Tags: [Academic, Research, Frontier, Global]

## Papers with Code
- Web: https://paperswithcode.com/latest
- RSS: https://paperswithcode.com/rss/latest
- Mode: Hybrid
- Tags: [Academic, Code, Benchmark, Research]

---

# ⚙️ 运行规则

实时模式（无 id）：
- 优先使用 RSS
- Search Only 源仅在重大事件时触发搜索

回溯模式（带 id）：
- 默认使用 site:Web 搜索
- RSS 仅在时间窗口覆盖时使用
- 禁止遍历首页

---

# ✅ 结构说明

Mode:
- Hybrid = RSS + 可回溯搜索
- Search Only = 无结构化 Feed，仅搜索

---

# 🧠 Tag 说明

Source 类型：
- Official
- Media
- Academic
- Ecosystem
- Model-Release

内容方向：
- LLM
- Research
- Funding
- Startup
- Policy
- Open Source
- Infrastructure
- Consumer AI
- Enterprise AI
- Frontier
- Benchmark
- Image
- Video
- Audio
- China
- Global
