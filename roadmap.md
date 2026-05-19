# 🗺️ HSBTVBrowser Roadmap & Future Plans / 开发路线图与未来规划

Welcome to the **Tanghulu Browser (糖葫芦浏览器)** project roadmap! This document outlines our future development plans and key milestones as we build the next-generation web browsing experience for Apple TV.

欢迎来到 **Tanghulu Browser (糖葫芦浏览器)** 项目开发路线图！本文档概述了我们未来的开发计划与核心里程碑。我们致力于为 Apple TV (tvOS) 带来极致的大屏网页浏览与多媒体娱乐体验。


## 🇨🇳 简体中文版

### 📌 阶段一：现有系统稳定性与细节体验打磨 (Focus: Core & Stability)
* **核心目标**：提供更加顺滑、无 Bug 的基础大屏浏览体验。
* **具体计划**：
  * **深度缺陷修复**：深入排查并彻底解决目前系统遗留的少量偶发性问题与交互边界缺陷。
  * **内存与渲染优化**：针对 tvOS 内存共享机制（RAM & VRAM）进行专项优化，最大化释放可用内存，保障在大屏 4K 场景下网页渲染的丝滑与稳定。

### 🤖 阶段二：浏览器与播放器深度接入大语言模型 (AI & LLM Integration)
我们相信 AI 将重新定义电视端的人机交互。我们将通过以下两种极具创新的方式，为浏览器和播放器插上 AI 的翅膀：

#### ⚙️ 两种大模型接入方案：
1. **端侧本地大模型 (On-Device Local AI)**
   * **运行机制**：我们将在配套的手机端遥控器 App 中直接加载本地轻量级大模型。tvOS 端通过局域网与遥控器进行高效数据通讯与指令分发。
   * **优势**：借用手机强大的本地 AI 算力，既保护了用户隐私，又彻底摆脱了 Apple TV 电视端硬件配置的瓶颈。
   * **开源生态**：配套遥控器项目已完全开源，欢迎共同建设：👉 [HSBRemoteBrowserTV](https://github.com/never88gone/HSBRemoteBrowserTV)。
2. **云端自定义大模型 (Cloud AI API)**
   * **运行机制**：在 App 设置中集成标准 API 配置界面，允许用户自主配置第三方主流大模型（如 OpenAI 兼容接口）的 URL 和 API Key。
   * **优势**：给予用户最大的自由度，随心选择体验最新、最强性能的云端大模型服务。

#### 🎯 三大 AI 核心落地场景：
* **🎙️ 自然语言语音控制网页**：摆脱繁琐的遥控器按键，用户直接通过语音发出指令（如“帮我点赞第一个视频”、“向上滚动半屏”），AI 智能解析意图并精确转化为网页点击和手势操作。
* **🌐 智能大屏网页翻译**：结合大语言模型，对各类英文及外文网站进行智能上下文双语翻译与排版重构，消除屏幕距离感，打造完美的电视大屏阅读体验。
* **🎬 播放器实时智能字幕**：在视频播放器中无缝整合语音识别 (ASR) 与大模型翻译。实时抓取视频背景音轨，自动生成高精准度的实时字幕与双语对齐翻译，让看外语视频不再困难。

### 🔬 阶段三：WebKit 内核定制与深度编译探索 (Deep Research)
* **核心目标**：打破 tvOS 平台的条条框框，探索在 Apple TV 上编译和运行高度定制化 WebKit 内核的可行性。
* **背景与现状**：
  * 前期我们已在本地开启了 WebKit 源码的编译尝试，由于目前 Apple TV (tvOS) 设备极度苛刻的硬件内存限制，编译与内存溢出问题导致该项研究暂时搁置。
  * **前瞻计划**：我们将持续关注苹果下一代新款 Apple TV 硬件的发展进度。一旦新款硬件配置提升（特别是运行内存 RAM 扩大），我们将重新启动 WebKit 在 tvOS 上的定制编译、底层优化和内核性能调优工作，彻底突破系统限制！

---

## 🇬🇧 English Version

### 📌 Phase 1: System Stability & Experiential Polish (Focus: Core & Stability)
* **Core Goal**: Deliver a seamless, flawless, and ultra-smooth browsing experience on Apple TV.
* **Actionable Plans**:
  * **Deep Bug Fixes**: Investigate and systematically resolve remaining missed issues, rare edge-case crashes, and interactive glitches.
  * **Memory & Rendering Optimization**: Implement highly targeted optimizations for tvOS's unified memory architecture (shared RAM/VRAM) to minimize footprint and ensure butter-smooth 4K rendering.

### 🤖 Phase 2: Integrating Deep LLM Capabilities into Browser & Player
We believe AI is the future of TV human-computer interaction. We are designing two highly innovative integration pathways to empower our browser and media player with artificial intelligence:

#### ⚙️ Two LLM Integration Approaches:
1. **On-Device Local AI via Companion App**
   * **Architecture**: The companion mobile remote control application will load a lightweight LLM on-device. The tvOS app will communicate with the remote in real-time.
   * **Benefit**: Taps into the powerful AI hardware of modern smartphones to achieve instant responses and guarantee user privacy while entirely bypassing Apple TV hardware limitations.
   * **Open-Source Repository**: The companion remote control is fully open-sourced. Pull requests are warmly welcomed: 👉 [HSBRemoteBrowserTV](https://github.com/never88gone/HSBRemoteBrowserTV).
2. **Custom Cloud LLM APIs**
   * **Architecture**: Offer an in-app setup allowing users to configure standard custom endpoints (compatible with OpenAI-style APIs) and their API Keys.
   * **Benefit**: Grants users total freedom to leverage any cutting-edge commercial or open-source cloud-based LLM.

#### 🎯 Three Core AI Use Cases:
* **🎙️ Natural Voice-Controlled Browsing**: Go beyond remote controller button-clicks. Users can speak naturally (e.g., "like the first video", "scroll down half a page"), and our AI will translate the voice prompt into exact page navigation and tap events.
* **🌐 Smart Big-Screen Translation**: Utilize advanced LLM contextual capabilities to translate and adapt foreign-language sites into highly readable, beautifully formatted bilingual pages optimized for TV screens.
* **🎬 Real-Time Intelligent Player Subtitles**: Combine LLM power with Automatic Speech Recognition (ASR) to capture video audio, generating and translating highly accurate subtitles on the fly. Streaming untranslated foreign videos will be effortless.

### 🔬 Phase 3: Customized WebKit Kernel Compilation & Research (Deep Research)
* **Core Goal**: Bypass current tvOS WebView constraints by attempting to compile and run a fully customized WebKit engine on Apple TV.
* **Context & Outlook**:
  * We initiated local WebKit compilation but paused due to strict memory limits of existing Apple TV models (shared VRAM/RAM bottleneck).
  * **Next Steps**: We will closely monitor upcoming Apple TV releases. Once next-generation Apple TV models with upgraded hardware configurations (specifically expanded RAM) are released, we will resume WebKit compilation, integration, and kernel-level performance tuning on tvOS.
