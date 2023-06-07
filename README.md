<div style="font-size: 1.5rem;">
  <a href="./README.md">中文</a> |
  <a href="./readme_en.md">English</a>
</div>



</br>

<h1 align="center">ChatPiXiu</h1>
<div align="center">
  <a href="https://github.com/catqaq/ChatPiXiu">
    <img src="docs/imgs/pixiu.jpg" alt="Logo" height="210">
  </a>


  <p align="center">
    <h3>ChatPiXiu: Eat every ChatGPT - Output your own chatbot.</h3>
      <a href="https://github.com/catqaq/ChatPiXiu/graphs/contributors">
        <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/catqaq/ChatPiXiu" />
      </a>
      <a href="https://github.com/catqaq/ChatPiXiu/issues">
        <img alt="Issues" src="https://img.shields.io/github/issues/catqaq/ChatPiXiu?color=0088ff" />
      </a>
      <a href="https://github.com/catqaq/ChatPiXiu/discussions">
        <img alt="Issues" src="https://img.shields.io/github/discussions/catqaq/ChatPiXiu?color=0088ff" />
      </a>
      <a href="https://github.com/catqaq/ChatPiXiu/pulls">
        <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/catqaq/ChatPiXiu?color=0088ff" />
      <a href="https://github.com/catqaq/ChatPiXiu/stargazers">
        <img alt="GitHub stars" src="https://img.shields.io/github/stars/catqaq/ChatPiXiu?color=ccf" />
      </a>
      <br/>
      <em>开源ChatGPT / 全面 / 轻量 / 易用 </em>
      <br/>
      <a href="https://zhuanlan.zhihu.com/p/622065348/"><strong>文章解读</strong></a>
        ·
      <a href="https://zhuanlan.zhihu.com/p/622065348"><strong>视频解读</strong></a>
    </p>






 </p>
</div>

> **代码开源，大家放心使用，欢迎贡献! 注意：模型的license取决于模型提供方**


- [💥最新讯息](#最新讯息)
- [💫OpenNLP计划](#OpenNLP计划)
- [💫OpenChat-PiXiu](#ChatPiXiu项目)
- [🌟开源ChatGPT调研](#开源ChatGPT调研)
- [⛏️使用步骤](#使用步骤)
- [📄运行示例](#运行示例)
- [📄结果展示](#结果展示)
- [🛠️常见报错](#常见报错)
- [💐参考资料&致谢](#参考资料&致谢)
- [🌟赞助我们](#赞助我们)
- [🌈Starchart](#Starchart)
- [🏆Contributors](#Contributors)




## 最新讯息

- 2023/04/14：ChatPiXiu项目正式启动：
  - 开源ChatGPT平替调研汇总
  - 

## OpenNLP计划

我们是谁？

我们是**羡鱼智能**【xianyu.ai】，主要成员是一群来自老和山下、西湖边上的咸鱼们，塘主叫作羡鱼，想在LLMs时代做点有意义的事！我们的口号是：**做OpenNLP和OpenX！希望在CloseAI卷死我们之前退出江湖！**

也许有一天，等到GPT-X发布的时候，有人会说NLP不存在了，但是我们想证明有人曾经来过、热爱过！在以ChatGPT/GPT4为代表的LLMs时代，在被CloseAI卷死之前，我们发起了OpenNLP计划，宗旨是OpenNLP for everyone! 

- 【P0】[OpenTextClassification](https://github.com/catqaq/OpenTextClassification)：打造一流的文本分类项目，已开源
  - 综述：done
  - 开源项目：done
  - papers解读：doing
  - 炼丹术：done
- 【P0】OpenSE：句嵌入，自然语言处理的核心问题之一，doing
- 【P0】[ChatPiXiu](https://github.com/catqaq/ChatPiXiu)：ChatGPT开源平替及领域适应，doing
- 【P1】OpenLLMs：大语言模型，doing
- 【P2】OpenTextTagger：文本标注，分词、NER、词性标注等
- OpenX：任重而道远

## ChatPiXiu项目

ChatPiXiu项目为OpenNLP计划的第2个正式的开源项目，旨在Open ChatGPT for everyone！在以ChatGPT/GPT4为代表的LLMs时代，在被OpenAI卷死之前，做一点有意义的事情！未来有一天，等到GPT-X发布的时候，或许有人会说NLP不存在了，但是我们想证明有人曾来过！

### 1.开发计划

本项目的开发宗旨，打造全面且实用的ChatGPT模型库和文档库。**Eat every ChatGPT - Output your own chatbot!**

目前我们正在启动V1版本的开发，整体的开发计划如下，主要包括了文档和代码两类任务，数据的部分我们暂时将其分散到了各个子任务中。

**V1版本：资料调研+通用最小实现+领域/任务适配**

#### 1.1 文档分支

文档分支主要负责项目文档的建设，包括通用技术文档和项目相关文档。

**dev_for_docs**：文档分支，主要负责资料调研（算力有限，有调查才有训练权）：

1. 【P0】开源ChatGPT调研：持续更新，doing
2. 【P0】训练技术调研：持续更新，doing
3. 【P0】数据调研：doing
4. 【P1】部署技术调研：TODO
5. 【P2】基础模型调研：目前以LLaMA和GLM为主，doing
6. 【P3】技术解读/教程：doing



#### 1.2 代码分支

代码分支，负责具体的开发工作，包括数据处理、算法开发、算法评测等，分成通用最小实现和领域/任务适应两种，具体的：

**dev_for_chatmini**：通用最小实现分支，尽可能支持不同的基础模型和训练方式，提供可比较的实现。

1. 【P0】ChatGPT最小复现：完整的RLHF复现SFT-RM-PPO，doing
2. 【P0】适配不同的基座模型
3. 适配不同的PEFT算法
4. 【P2】探索新的训练方式
5. 【P3】探索知识迁移：比如蒸馏



**dev_for_chatzhihu**：知乎及问答领域适配，主要想解决一些知乎使用过程中的痛点，比如问题冗余、回答太多等等。

1. 【P0】收集知乎数据收集及处理
   1. SFT数据
   2. RLHF数据：答案打分
   3. 摘要数据：答案/观点汇总、摘要
2. 【P0】基于知乎数据做SFT
3. 【P1】基于知乎数据做RLHF
4. 【P2】输出知乎LoRA
5. 【P3】和知乎热榜聊天的demo



**dev_for_chatzhangsan**：法律领域适配，张三犯了什么罪？

1. 【P0】法律领域数据收集及处理
2. 法律条文解释
3. 【P1】罪名判定：张三犯了什么罪？



更多领域，敬请期待！

ChatPiXiu-Eat every ChatGPT - Output your own chatbot!

### 2.加入我们

OpenNLP计划的其他内容尚在筹备中，暂时只开源了本项目和[OpenTextClassification](https://github.com/catqaq/OpenTextClassification)项目。欢迎大家积极参与ChatPiXiu的建设和讨论，一起变得更强！

加入方式：

- **项目建设**：可以在前面列出的开发计划中选择自己感兴趣的部分进行开发，建议优先选择高优先级的任务。包括资料调研和算法开发等工作。
- OpenLLM技术交流群：知识在讨论中发展，QQ群：740679327
- 技术分享和讨论：输出倒逼输入，欢迎投稿，稿件会同步到本项目的docs目录和知乎专栏OpenNLP. 同时也欢迎大家积极的参与本项目的讨论https://github.com/catqaq/ChatPiXiu/discussions。

## 开源ChatGPT调研

### 1.开源ChatGTP平替

注：开源类ChatGPT/LLM汇总，持续更新中，欢迎贡献! 现已超过60+！

| 项目                                                         | 基础模型                                      | lang        | 机构                                                         | 数据集                                                       | license                                                      | 介绍                                                         | 备注                                                         |
| ------------------------------------------------------------ | --------------------------------------------- | ----------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [LLaMA](https://github.com/facebookresearch/llama)           | LLaMA                                         | Multi       | meta                                                         | CCNet [67%], C4 [15%], GitHub [4.5%], Wikipedia [4.5%], Books [4.5%], ArXiv [2.5%], Stack Exchange[2%]. | [Apache-2.0 license](https://github.com/tatsu-lab/stanford_alpaca/blob/main/LICENSE) | 可能是目前开源ChatGPT用的最多的基础模型                      | 支持多语言，但以英文为主                                     |
| [stanford_alpaca](https://github.com/tatsu-lab/stanford_alpaca) Alpaca | LLaMA                                         | eng         | stanford                                                     | [alpaca_data](https://github.com/tatsu-lab/stanford_alpaca/blob/main/alpaca_data.json) | [Apache-2.0 license](https://github.com/tatsu-lab/stanford_alpaca/blob/main/LICENSE) | 指令调优的 LLaMA 模型: An Instruction-following LLaMA Model. 让 OpenAI 的 text-davinci-003 模型以 self-instruct 方式生成 52K 指令样本，SFT | FT模型语言以数据为准                                         |
| [ChatLLaMA](https://github.com/nebuly-ai/nebullvm/tree/main/apps/accelerate/chatllama) | LLaMA                                         |             | Nebuly+AI                                                    | -                                                            | [license](https://github.com/nebuly-ai/nebullvm/blob/main/apps/accelerate/chatllama/LICENSE) | 数据集创建、使用 RLHF 进行高效训练以及推理优化。             |                                                              |
| [Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca) | LLaMA                                         | mutli       | [ymcui](https://github.com/ymcui)                            | -                                                            | [Apache-2.0 license](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/LICENSE.md) | Chinese LLaMA & Alpaca LLMs; 中文词表扩充                    |                                                              |
| [alpaca-lora](https://github.com/tloen/alpaca-lora)          | LLaMA                                         |             | stanford                                                     | [LLaMA-GPT4 dataset](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM) | [Apache-2.0 license](https://github.com/tloen/alpaca-lora/blob/main/LICENSE) | [LoRA](https://zhuanlan.zhihu.com/p/620327907)               |                                                              |
| Chinese-alpaca-lora Luotuo-Chinese-LLM                       | LLaMA                                         |             | -                                                            |                                                              |                                                              | LoRA                                                         |                                                              |
| [ChatGLM](https://github.com/THUDM/ChatGLM-6B)               | GLM                                           | cn/eng      | 清华                                                         | 1T 标识符的中英双语数据                                      | [Apache-2.0 license](https://github.com/THUDM/ChatGLM-6B/blob/main/LICENSE) | 监督微调、反馈自助、人类反馈强化学习                         | [PROJECT.md](https://github.com/THUDM/ChatGLM-6B/blob/main/PROJECT.md) |
| [FastChat](https://github.com/lm-sys/FastChat)  Vicuna       | LLaMA                                         | eng         | UC Berkeley, CMU, Stanford, UCSD and MBZUAI                  | ShareGPT, 70k问答指令数据                                    | [Apache-2.0 license](https://github.com/lm-sys/FastChat/blob/main/LICENSE) | SFT，使用GPT-4作为评判标准，结果显示Vicuna-13B在超过90%的情况下实现了与ChatGPT和Bard相匹敌的能力。 |                                                              |
| Chinese-Vicuna                                               | LLaMA                                         | cn          | -                                                            | -                                                            | [Apache-2.0 license](https://github.com/Facico/Chinese-Vicuna/blob/master/LICENSE) | LoRA                                                         |                                                              |
| [EasyLM](https://github.com/young-geng/EasyLM) Koala考拉     | LLaMA multi                                   | eng         | UC伯克利                                                     | ChatGPT数据和开源数据（Open Instruction Generalist (OIG)、斯坦福 Alpaca 模型使用的数据集、Anthropic HH、OpenAI WebGPT、OpenAI Summarization） | [Apache-2.0 license](https://github.com/Facico/Chinese-Vicuna/blob/master/LICENSE) | SFT/13B/500k条数据                                           |                                                              |
| [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) | LLaMA                                         |             | ColossalAI                                                   | [InstructionWild](https://github.com/XueFuzhao/InstructionWild):104K bilingual datasets | [LICENSE](https://github.com/hpcaitech/ColossalAI/blob/main/applications/Chat/LICENSE) | SFT-RM-RLHF                                                  |                                                              |
| [ChatRWKV](https://github.com/BlinkDL/ChatRWKV)              | RWKV                                          |             | [BlinkDL](https://github.com/BlinkDL)                        | -                                                            | [Apache-2.0 license](https://github.com/BlinkDL/ChatRWKV/blob/main/LICENSE) | ChatRWKV is like ChatGPT but powered by RWKV (100% RNN) language model, and open source. |                                                              |
| [ChatYuan](https://github.com/clue-ai/ChatYuan)              | T5                                            | eng/cn      | 元语智能                                                     | PromptClue                                                   | [LICENSE](https://github.com/clue-ai/ChatYuan/blob/main/LICENSE) | 基于PromptClue进行了监督微调                                 |                                                              |
| [OpenChatKit](https://github.com/togethercomputer/OpenChatKit) | GPT-NoX-20B                                   |             | Together+LAION+Ontocord.ai                                   | OIG-43M                                                      | [Apache-2.0 license](https://github.com/togethercomputer/OpenChatKit/blob/main/LICENSE) | 60亿参数的审核模型，对不合适或者是有害的信息进行过滤         |                                                              |
| BELLE                                                        | Bloom LLama                                   | cn          | [LianjiaTech](https://github.com/LianjiaTech)                | 10M-ChatGPT生成的数据                                        | [Apache-2.0 license](https://github.com/LianjiaTech/BELLE/blob/main/LICENSE) | SFT                                                          |                                                              |
| PaLM-rlhf-pytorch                                            | PaLM                                          |             | [lucidrains](https://github.com/lucidrains)                  | -                                                            | [MIT license](https://github.com/lucidrains/PaLM-rlhf-pytorch/blob/main/LICENSE) | RLHF                                                         | PaLM太大了                                                   |
| [dolly](https://github.com/databrickslabs/dolly)             | v1:GPT-J-6B v2:pythia                         | eng         | Databricks                                                   | The Pile+databricks-dolly-15k                                | [MIT license](https://github.com/lucidrains/PaLM-rlhf-pytorch/blob/main/LICENSE) | 参考Alpaca; dolly-v2-12b based on pythia-12b                 |                                                              |
| LMFlow                                                       | LLaMA                                         |             | [OptimalScale](https://github.com/OptimalScale)              |                                                              |                                                              | An Extensible Toolkit for Finetuning and Inference of Large Foundation Models. Large Model for All. LLaMA-7B，一张3090耗时 5 个小时 |                                                              |
| GPTrillion                                                   | -                                             |             | -                                                            | -                                                            | -                                                            | 1.5万亿，多模态                                              |                                                              |
| [open_flamingo](https://github.com/mlfoundations/open_flamingo) | LLaMA CLIP                                    |             | LAION                                                        | [Multimodal C4](https://github.com/allenai/mmc4)             | [MIT license](https://github.com/mlfoundations/open_flamingo/blob/main/LICENSE) |                                                              |                                                              |
| [baize-chatbot](https://github.com/project-baize/baize-chatbot) | LLaMA                                         | eng         | [project-baize](https://github.com/project-baize)            | 100k dialogs generated by letting ChatGPT chat with itself.  | [GPL-3.0 license](https://github.com/project-baize/baize-chatbot/blob/main/LICENSE) | LoRA                                                         |                                                              |
| [ChatPiXiu](https://github.com/catqaq/ChatPiXiu)             | multi                                         |             | 羡鱼智能                                                     | -                                                            | -                                                            | LoRA                                                         | 筹备阶段                                                     |
| [stackllama](https://huggingface.co/blog/stackllama)         | LLaMA                                         |             | Hugging Face                                                 | -                                                            | -                                                            | 用RLHF训练LLaMA的实践指南                                    |                                                              |
| [Lit-LLaMA](https://github.com/Lightning-AI/lit-llama)       | LLaMA                                         | multi       | lightening-ai                                                | -                                                            | [Apache-2.0 license](https://github.com/Lightning-AI/lit-llama/blob/main/LICENSE) | 重写重训LLaMA,绕开license: Implementation of the LLaMA language model based on nanoGPT. | 可商用版LLaMA                                                |
| [OPT](https://arxiv.org/abs/2205.01068)                      | OPT                                           | eng         | meta                                                         | -                                                            | [MIT license](https://github.com/facebookresearch/metaseq/blob/main/LICENSE) | 当年对标GPT3的模型                                           |                                                              |
| [Cerebras-GPT](https://huggingface.co/cerebras/Cerebras-GPT-13B) | Cerebras-GPT                                  | eng         | Cerebras                                                     | The Pile                                                     | [Apache-2.0 license](https://github.com/Cerebras/modelzoo/blob/main/LICENSE) | GPT-3 style; 最小 1.11 亿，最大 130 亿，共 7 个模型          |                                                              |
| BLOOM                                                        | BLOOM                                         | multi       | [bigscience](https://huggingface.co/bigscience)              | Total seen tokens: 366B                                      | 代码：[Apache-2.0 license ](https://github.com/huggingface/transformers-bloom-inference/blob/main/LICENSE)模型：RAIL License v1.0 | 176B；46 种自然语言（包括中文）和 13 种编程语言              |                                                              |
| GPT-J                                                        | GPT-3                                         | multi       | EleutherAI                                                   | The Pile                                                     | [apache-2.0](https://huggingface.co/models?license=license:apache-2.0) | based on GPT-3;                                              |                                                              |
| GPT-2                                                        |                                               |             |                                                              |                                                              |                                                              |                                                              |                                                              |
| [RWKV](https://github.com/BlinkDL/RWKV-LM)                   | [RWKV-LM](https://github.com/BlinkDL/RWKV-LM) | cn/eng      | [BlinkDL](https://github.com/BlinkDL)                        |                                                              |                                                              |                                                              | 纯RNN                                                        |
| [鹏程・盘古 α](https://www.oschina.net/p/pangu-alpha)        |                                               | cn          | 鹏城                                                         | 2TB                                                          | [Apache License 2.0](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha/src/branch/master/LICENSE) |                                                              |                                                              |
| [鹏程・盘古对话](https://www.oschina.net/p/pangu-dialog)     |                                               | cn          | 鹏城                                                         |                                                              |                                                              |                                                              |                                                              |
| [悟道](https://www.oschina.net/p/wudao-model)                |                                               | cn/eng      | BAAI(智源)                                                   |                                                              |                                                              | 多模态; 1.75 万亿参数; 图文：CogView、BriVL；文本：GLM、CPM、Transformer-XL、EVA、Lawformer；生物：ProtTrans |                                                              |
| [MOSS](https://www.oschina.net/p/moss)                       | MOSS                                          | cn/eng      | [OpenLMLab](https://github.com/OpenLMLab)                    | 700B tokens                                                  | 代码Apache 2.0，数据CC BY-NC 4.0，模型权重GNU AGPL 3.0       | 支持中英双语和多种插件; 基座moss-moon-003-base               |                                                              |
| [伶荔 (Linly)](https://www.oschina.net/p/linly)              | LLaMA                                         | cn          | [CVI-SZU](https://github.com/CVI-SZU)                        |                                                              | Apache Licence 2.0                                           | 33B 的 Linly-Chinese-LLAMA 是目前最大的中文 LLaMA 模型       |                                                              |
| [华驼 (HuaTuo)](https://www.oschina.net/p/huatuo-llama)      | LLaMA                                         | cn/eng      | [SCIR-HI](https://github.com/SCIR-HI)                        |                                                              | [Apache-2.0 license](https://github.com/SCIR-HI/Huatuo-Llama-Med-Chinese/blob/main/LICENSE) |                                                              | 医学                                                         |
| [BBT-2](https://www.oschina.net/p/bbt-2)                     |                                               | cn/eng      |                                                              |                                                              |                                                              | 120 亿参数的通用大语言模型                                   |                                                              |
| [CodeGeeX](https://www.oschina.net/p/codegeex)               | -                                             | code        | 鹏城                                                         |                                                              |                                                              | 130 亿参数的多编程语言代码生成预训练模型                     | code                                                         |
| [RedPajama](https://www.oschina.net/p/redpajama)             | gpt-neox                                      | eng         | Together、Ontocord.ai、ETH DS3Lab、斯坦福大学 CRFM、Hazy Research 和 MILA 魁北克 AI 研究所 | 800B/1T                                                      | Apache-2.0                                                   | 开源地全面对齐LLaMA的训练数据集                              |                                                              |
| [OpenAssistant](https://www.oschina.net/p/open-assistant)    |                                               | eng         | [LAION-AI](https://github.com/LAION-AI)                      |                                                              | [Apache-2.0 license](https://github.com/LAION-AI/Open-Assistant/blob/main/LICENSE) | OpenAssistant is a chat-based assistant that understands tasks, can interact with third-party systems, and retrieve information dynamically to do so. |                                                              |
| [StableLM](https://www.oschina.net/p/stablelm)               | pythia                                        | eng         | [Stability-AI](https://github.com/Stability-AI)              |                                                              | [Apache-2.0 license](https://github.com/Stability-AI/StableLM/blob/main/LICENSE) | Stability AI Language Models; max len 4096                   |                                                              |
| [StarCoder](https://www.oschina.net/p/starcoder)             |                                               | code        | [bigcode-project](https://github.com/bigcode-project)        |                                                              | [Apache-2.0 license](https://github.com/bigcode-project/starcoder/blob/main/LICENSE) |                                                              | code                                                         |
| [SantaCoder](https://www.oschina.net/p/santacoder)           |                                               | code        | [bigcode](https://huggingface.co/bigcode)                    | The Stack（v1.1）                                            | the BigCode OpenRAIL-M v1 license                            | 轻量级 AI 编程模型，1.1B                                     | code                                                         |
| [MLC LLM](https://www.oschina.net/p/mlc-llm)                 |                                               | -           | [mlc-ai](https://github.com/mlc-ai)                          | -                                                            | [Apache-2.0 license](https://github.com/mlc-ai/mlc-llm/blob/main/LICENSE) | 本地大语言模型部署；Enable everyone to develop, optimize and deploy AI models natively on everyone's devices. |                                                              |
| [Web LLM](https://www.oschina.net/p/web-llm)                 |                                               |             | [mlc-ai](https://github.com/mlc-ai)                          |                                                              | [Apache-2.0 license](https://github.com/mlc-ai/web-llm/blob/main/LICENSE) | Bringing large-language models and chat to web browsers.     |                                                              |
| [WizardLM](https://www.oschina.net/p/wizardlm)               | LLaMA                                         | eng         | [nlpxucan](https://github.com/nlpxucan)                      |                                                              |                                                              | Evol-Instruct                                                |                                                              |
| [YaLM 100B](https://www.oschina.net/p/yalm-100b)             |                                               | eng/russian | [yandex](https://github.com/yandex)                          |                                                              | [Apache-2.0 license](https://github.com/yandex/YaLM-100B/blob/main/LICENSE) |                                                              |                                                              |
| [OpenLLaMA](https://www.oschina.net/p/openllama)             |                                               | multi       | [s-JoL](https://github.com/s-JoL)                            |                                                              | [MIT license](https://github.com/s-JoL/Open-Llama/blob/main/LICENSE) | LLaMA 开源复现版                                             |                                                              |
| BiLLa                                                        | LLaMA                                         | cn/eng      | [Neutralzz](https://github.com/Neutralzz)                    |                                                              |                                                              | A Bilingual LLaMA with Enhanced Reasoning Ability            |                                                              |
| pandallm                                                     | LLaMA                                         | cn/eng      | [dandelionsllm](https://github.com/dandelionsllm)            |                                                              | Apache-2.0 license                                           |                                                              |                                                              |
| pandalm                                                      |                                               |             | [WeOpenML](https://github.com/WeOpenML)                      |                                                              | [Apache-2.0 license](https://github.com/WeOpenML/PandaLM/blob/main/LICENSE) | PandaLM：可重现和自动化的语言模型评估                        |                                                              |
| [gpt4all](https://github.com/nomic-ai/gpt4all)               |                                               |             | [nomic-ai](https://github.com/nomic-ai)                      |                                                              | [MIT license](https://github.com/nomic-ai/gpt4all/blob/main/LICENSE.txt) | gpt4all: an ecosystem of open-source chatbots trained on a massive collections of clean assistant data including code, stories and dialogue |                                                              |
| [stable-vicuna](https://huggingface.co/CarperAI/stable-vicuna-13b-delta) |                                               | eng         | [CarperAI](https://huggingface.co/CarperAI)                  |                                                              | [CC-BY-NC-SA-4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) | StableVicuna-13B is a Vicuna-13B v0 model fine-tuned         |                                                              |
| [MPT](https://huggingface.co/mosaicml/mpt-7b)                | MPT                                           | eng         | [mosaicml](https://huggingface.co/mosaicml)                  | 1T tokens of English text and code                           | Apache-2.0                                                   | ALiBi保证了良好的长度外推性                                  |                                                              |
| ImageBind                                                    |                                               | 多模态      | meta                                                         |                                                              |                                                              | One embedding space to bind them all.                        |                                                              |
| [Phoenix](https://github.com/FreedomIntelligence/LLMZoo)     |                                               | multi       | CUHK                                                         |                                                              |                                                              | 7B/BLOOMZ + 微调                                             |                                                              |
| [ChatPLUG](https://github.com/X-PLUG/ChatPLUG)               |                                               |             | Alibaba                                                      |                                                              |                                                              | Encoder-Decoder/3.7B                                         |                                                              |
| [BLOOMZ](https://github.com/bigscience-workshop/xmtf)        |                                               | multi       | BigScience                                                   |                                                              |                                                              | BLOOM + 多任务微调                                           |                                                              |
| [CPM-Ant+](https://github.com/OpenBMB/CPM-Live/tree/cpm-ant-plus/cpm-live) |                                               | cn/eng      | OpenBMB                                                      |                                                              |                                                              | 10B/Decoder-only(UniLM)                                      |                                                              |
| [PaLM](https://ai.googleblog.com/2022/04/pathways-language-model-palm-scaling-to.html) |                                               | multi       | Google                                                       |                                                              | -                                                            | pathways/540B                                                | 未开源                                                       |
| [PaLM 2](https://blog.google/technology/ai/google-palm-2-ai-large-language-model/) |                                               | multi       | Google                                                       |                                                              | -                                                            | pathways; 改进的多语言、推理和编码能力                       | 未开源                                                       |
|                                                              |                                               |             |                                                              |                                                              |                                                              |                                                              |                                                              |



### 2.基础模型

注：基础LLM汇总，持续更新中，欢迎贡献! 现已超过15+！个人的工作和研究兴趣会更关注基础模型相关技术及其应用！

| model                                                        | Architecture/task           | lang   | tokenizer | vocab                                    | PE                   | max len                        | size                                    | org                                           | data                                                         | license                                                      | intro                                                        | notes                                                        |
| ------------------------------------------------------------ | --------------------------- | ------ | --------- | ---------------------------------------- | -------------------- | ------------------------------ | --------------------------------------- | --------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [LLaMA](https://huggingface.co/decapoda-research/llama-7b-hf) | decoder/LM                  | multi  | BBPE      | 32K                                      | RoPE                 | 2048                           | 7B/13B/33B/65B                          | meta                                          | 1.4万亿 tokens                                               | [GPL-3.0 license](https://github.com/facebookresearch/llama/blob/main/LICENSE) | Meta 大语言模型: The model comes in different sizes: 7B, 13B, 33B and 65B parameters. |                                                              |
| GLM                                                          | mix/自回归式填空，prefix LM | cn/eng | multi     | multi                                    | RoPE                 | 2048 for 130B 1024 for ChatGLM | 6B/10B/130B                             | 智谱                                          | 中英文token各2000亿                                          | [Apache-2.0 license](https://github.com/THUDM/ChatGLM-6B/blob/main/LICENSE) | ChatGLM-6B: 1T data                                          |                                                              |
| GPT1                                                         | decoder/LM                  | eng    | BPE       | 40478                                    | learned              | 512                            |                                         | OpenAI                                        | BooksCorpus/5 G                                              | [MIT License](https://github.com/openai/finetune-transformer-lm/blob/master/LICENSE) | GPT系列的起源                                                | 分词部分有特殊处理，详见tokenization_openai.py： - lowercases all inputs,     - uses `SpaCy` tokenizer and `ftfy` for pre-BPE tokenization if they are installed, fallback to BERT's       `BasicTokenizer` if not. |
| [GPT2](https://huggingface.co/gpt2-xl)                       | decoder/LM                  | multi  | BBPE      | 50257                                    | learned              | 1024                           | 124M/355M/774M/1.5B                     | OpenAI                                        | WebText/ 40G                                                 | [Modified MIT License](https://github.com/openai/gpt-2/blob/master/LICENSE) | 主打zero-shot                                                | GPT系列开源的最后一舞                                        |
| GPT3                                                         | decoder/LM                  | multi  | BBPE      | 50257/davinci                            | learned              | 2048                           | 175B                                    | OpenAI                                        | 570G                                                         |                                                              | sparse attention；主打few-shot/in-context learning           | 关上了GPT系列的大门                                          |
| GPT3.5                                                       | decoder/LM                  | multi  | BBPE      | 100256                                   | ~learned             | 4096                           |                                         | OpenAI                                        | -                                                            | -                                                            | InstructGPT等一系列模型                                      | 未开源                                                       |
| GPT4                                                         | decoder/LM                  | multi  | BBPE      | 100256                                   | ~learned             | 32768                          |                                         | OpenAI                                        | -                                                            | -                                                            | 多模态                                                       | 未开源                                                       |
| [BLOOM](https://huggingface.co/bigscience/bloom)             | decoder/LM                  | multi  | BBPE      | 250,680                                  | ALiBi                | 2048                           | 176B                                    | bigscience                                    | [Data Cards](https://huggingface.co/spaces/bigscience/BigScienceCorpus) | RAIL License v1.0                                            | Modified from Megatron-LM GPT2; StableEmbedding              | 包括Training logs                                            |
| PaLM                                                         |                             |        |           |                                          | RoPE                 |                                |                                         |                                               |                                                              |                                                              |                                                              |                                                              |
| Chinchilla                                                   |                             |        |           |                                          | transformer-XL style |                                |                                         |                                               |                                                              |                                                              |                                                              |                                                              |
| OPT                                                          |                             | eng    |           |                                          | learned              |                                |                                         |                                               |                                                              |                                                              |                                                              |                                                              |
| [GPT-J](https://huggingface.co/EleutherAI/gpt-j-6b)          | decoder/LM                  | multi  | BBPE      | 50257/50400† (same tokenizer as GPT-2/3) | RoPE                 | 2048                           | 6B                                      | EleutherAI                                    | The Pile                                                     | [apache-2.0](https://huggingface.co/models?license=license:apache-2.0) | based on GPT-3;                                              |                                                              |
| [Lit-LLaMA](https://github.com/Lightning-AI/lit-llama)       |                             |        |           |                                          |                      |                                |                                         |                                               |                                                              |                                                              | Implementation of the LLaMA language model based on nanoGPT. |                                                              |
| [Cerebras-GPT](https://huggingface.co/cerebras/Cerebras-GPT-13B) | decoder                     | eng    | BPE       | 50257                                    | Learned              | 2048                           |                                         | [Cerebras Systems](https://www.cerebras.net/) | The Pile                                                     | Apache 2.0                                                   | The family includes 111M, 256M, 590M, 1.3B, 2.7B, 6.7B, and 13B models. All models in the Cerebras-GPT family have been trained in accordance with Chinchilla scaling laws (20 tokens per model parameter) which is compute-optimal. |                                                              |
| [RWKV](https://github.com/BlinkDL/RWKV-LM)                   | RNN                         | eng/cn |           |                                          | None(pure RNN)       | 1024/4096/8192                 | [multi](https://huggingface.co/BlinkDL) |                                               | the Pile                                                     |                                                              | 结合了 RNN 和 Transformer 的语言模型，适合长文本，运行速度较快，拟合性能较好，占用显存较少，训练用时较少。RWKV 整体结构依然采用 Transformer Block 的思路，相较于原始 Transformer Block 的结构，RWKV 将 self-attention 替换为 Position Encoding 和 TimeMix，将 FFN 替换为 ChannelMix。其余部分与 Transfomer 一致。 |                                                              |
| CoLT5                                                        |                             |        |           |                                          | T5 bias style        |                                |                                         |                                               |                                                              |                                                              |                                                              |                                                              |
| MOSS                                                         | decoder/LM                  | cn/eng |           |                                          |                      | 2048                           | 16B                                     | [OpenLMLab](https://github.com/OpenLMLab)     | 700B tokens                                                  | 代码Apache 2.0，数据CC BY-NC 4.0，模型权重GNU AGPL 3.0       | 支持中英双语和多种插件                                       |                                                              |
| [MPT](https://huggingface.co/mosaicml/mpt-7b)                | decoder/LM                  | eng    | BBPE      | 50432                                    | ALiBi                | 2048/65k/84k                   | 7B                                      | [mosaicml](https://huggingface.co/mosaicml)   | 1T tokens+各种FT数据                                         | Apache-2.0                                                   | Although the model was trained with a sequence length of 2048, ALiBi enables users to increase the maximum sequence length during finetuning and/or inference.  The model vocabulary size of 50432 was set to be a multiple of 128 (as in MEGATRON-LM) |                                                              |
| [mt5](https://huggingface.co/google/mt5-xxl)                 | encoder-decoder             | multi  |           |                                          |                      |                                | 1.2B/3.7B/13B                           | Google                                        | mC4                                                          |                                                              |                                                              |                                                              |
| [Wenzhong2.0-GPT2-3.5B-chinese](https://huggingface.co/IDEA-CCNL/Wenzhong2.0-GPT2-3.5B-chinese) | decoder/LM                  | cn     |           |                                          |                      |                                | 3.5B                                    | IDEA-CCNL                                     |                                                              |                                                              |                                                              |                                                              |
| CPM-Generate                                                 |                             | cn     |           |                                          |                      |                                | 2.6B                                    | TsinghuaAI                                    | 100GB Chinese training data                                  |                                                              |                                                              |                                                              |
| [bloom-zh](https://huggingface.co/Langboat/bloom-1b4-zh)     | decoder/LM                  | cn     | BBPE      | 46145                                    | ALiBi                | 2048                           | 1.4B/2.5B/6.4B                          | Langboat                                      | -                                                            |                                                              | 词表裁剪，保留中文: 250880 to 46145                          |                                                              |
| [GPT-2B](https://huggingface.co/nvidia/GPT-2B-001)           | decoder/LM                  | eng    | BBPE      |                                          | RoPE                 | 4096                           |                                         | HuggingFace+Nvidia                            | 1.1T tokens                                                  |                                                              |                                                              |                                                              |
|                                                              |                             |        |           |                                          |                      |                                |                                         |                                               |                                                              |                                                              |                                                              |                                                              |



### 3.数据

| dataset                     | type        | 机构                                | 大小 | license | 介绍 | 备注 |
| --------------------------- | ----------- | ----------------------------------- | ---- | ------- | ---- | ---- |
| alpaca_data                 | Instruction | stanford                            |      |         |      |      |
| alpaca_chinese_dataset      | \-          | hikariming                          |      |         |      |      |
| Multilingual Instruction    |             | Guanaco                             |      |         |      |      |
| alpaca_chinese_dataset      |             | carbonz0                            |      |         |      |      |
| 0.5M+1M chinese instruction |             | LianjiaTech                         |      |         |      |      |
| shareGPT                    |             | [lm-sys](https://github.com/lm-sys) |      |         |      |      |
|                             |             |                                     |      |         |      |      |



### 4.产品

注：为了文档的完整性，将工业界的ChatGPT也进行了汇总，只做介绍不做比较，以免争议!

| model                                             | org       | intro | notes |
| ------------------------------------------------- | --------- | ----- | ----- |
| [ChatGPT-GPT-3.5-turbo](https://chat.openai.com/) | OpenAI    |       |       |
| [ChatGPT-GPT-4](https://chat.openai.com/)         | OpenAI    |       |       |
| Claude                                            | Anthropic |       |       |
| 文心一言                                          | 百度      |       |       |
| 星火人知大模型                                    | 讯飞      |       |       |
| ChatGLM                                           | 清华/智谱 |       |       |
| MiniMax                                           | MiniMax   |       |       |
| 通义千问                                          | 阿里      |       |       |
| Bard                                              | Google    |       |       |
|                                                   |           |       |       |



### 5.训练&部署

#### 5.1 训练

| 框架                                                         | type    | 机构                                      | 兼容性                       | license                                                      | 介绍                                                         | 备注 |
| ------------------------------------------------------------ | ------- | ----------------------------------------- | ---------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---- |
| [ColossalAI](https://github.com/hpcaitech/ColossalAI)        | general | [hpcaitech](https://github.com/hpcaitech) | 高                           | [Apache-2.0 license](https://github.com/hpcaitech/ColossalAI/blob/main/LICENSE) | Colossal-AI: Making large AI models cheaper, faster, and more accessible<br>支持ChatGPT完整复现 |      |
| [RLHF](https://github.com/sunzeyeah/RLHF)                    | RL      | [sunzeyeah](https://github.com/sunzeyeah) | 基于transformers库实现       | \-                                                           | Implementation of Chinese ChatGPT.<br>SFT、Reward Model和RLHF |      |
| trlx                                                         | RL      | [CarperAI](https://github.com/CarperAI)   | 强大的transformer 强化学习库 | [MIT license](https://github.com/CarperAI/trlx/blob/main/LICENSE) | A repo for distributed training of language models with Reinforcement Learning via Human Feedback (RLHF)<br>不支持自定义预训练模型。 |      |
| [trl](https://github.com/lvwerra/trl)                        | RL      | Hugging Face                              | 基于transformers             | [Apache-2.0 license](https://github.com/lvwerra/trl/blob/main/LICENSE) | 只要是基于ransformers 库开发的预训练库，均可适配，强烈推荐   |      |
| [DeepSpeed-Chat](https://github.com/microsoft/DeepSpeedExamples/tree/master/applications/DeepSpeed-Chat) | general | [microsoft](https://github.com/microsoft) | 基于DeepSpeed                | [Apache-2.0 license](https://github.com/microsoft/DeepSpeedExamples/blob/master/LICENSE) | **训练速度**大幅提升                                         |      |
| [nanoGPT](https://github.com/karpathy/nanoGPT)               | GPT     | [karpathy](https://github.com/karpathy)   |                              | [MIT license](https://github.com/karpathy/nanoGPT/blob/master/LICENSE) | The simplest, fastest repository for training/finetuning medium-sized GPTs. |      |
|                                                              |         |                                           |                              |                                                              |                                                              |      |



#### 5.2 部署



## 使用步骤：TODO

1.克隆本项目

`git clone https://github.com/catqaq/ChatPiXiu.git`

2.准备数据



3.运行示例



## 结果展示




## 常见报错



## 参考资料&致谢

【OpenLLM 011】ChatPiXiu项目-可能是全网最全的ChatGPT复现调研：54+开源ChatGPT平替项目，15+基础模型，8+ ChatGPT产品！ - 羡鱼智能的文章 - 知乎 https://zhuanlan.zhihu.com/p/629364056 

开源ChatGPT替代模型项目整理https://zhuanlan.zhihu.com/p/618790279

平替chatGPT的开源方案 https://zhuanlan.zhihu.com/p/618926239ChatGPT/GPT4

开源“平替”汇总https://zhuanlan.zhihu.com/p/621324917

完整版 ChatGPT 克隆方案，开源了！https://zhuanlan.zhihu.com/p/617996976

ColossalChat：完整RLHF平替ChatGPT的开源方案 https://zhuanlan.zhihu.com/p/618048558ChatGPT

开源平替来了，开箱即用！前OpenAI团队打造，GitHub刚发布就揽获800+星https://zhuanlan.zhihu.com/p/613556853

LoRA:大模型的低秩适配-最近大火的lora到底是什么东西？为啥stable diffusion和开源ChatGPT复现都在用？https://zhuanlan.zhihu.com/p/620327907? 

成本不到100美元！UC伯克利再开源类ChatGPT模型「考拉」：数据量大没有用，高质量才是王道https://zhuanlan.zhihu.com/p/621078208

ChatGPT平替方案汇总https://zhuanlan.zhihu.com/p/618839784

微软宣布开源 Deep Speed Chat，可将训练速度提升 15 倍以上，哪些信息值得关注？https://www.zhihu.com/question/595311294 

总结当下可用的大模型LLMshttps://zhuanlan.zhihu.com/p/611403556

可能是最全的开源 LLM （大语言模型）整理

https://my.oschina.net/oscpyaqxylk/blog/8727824

[资源整理]2023-05-11比较全的LLMs的资源整理 - 迷途小书僮的文章 - 知乎 https://zhuanlan.zhihu.com/p/628637821

中文开源1B以上大模型汇总 - nghuyong的文章 - 知乎 https://zhuanlan.zhihu.com/p/613239726

https://github.com/CLUEbenchmark/SuperCLUE

https://github.com/THUDM/ChatGLM-6B

一文汇总开源大语言模型，人人都可以拥有自己的ChatGPT - 无忌的文章 - 知乎 https://zhuanlan.zhihu.com/p/622370602

新发布的一些开源商用模型 - LokLok的文章 - 知乎 https://zhuanlan.zhihu.com/p/627785493

最新发布！截止目前最强大的最高支持65k输入的开源可商用AI大模型：MPT-7B！ - 数据学习的文章 - 知乎 https://zhuanlan.zhihu.com/p/627420365

复旦团队大模型 MOSS 开源了，有哪些技术亮点值得关注？ - 孙天祥的回答 - 知乎 https://www.zhihu.com/question/596908242/answer/2994534005

暴击专家模型！Meta最新多模态大模型ImageBind已开源 - 新智元的文章 - 知乎 https://zhuanlan.zhihu.com/p/628370318

整理开源可用的中文大模型LLMs - 罗胤的文章 - 知乎 https://zhuanlan.zhihu.com/p/616812772

大模型热点论文：谷歌推出 PaLM 2、Meta 开源 ImageBind - MegEngine Bot的文章 - 知乎 https://zhuanlan.zhihu.com/p/628941792

如何评价Google最新发布的PaLM2，效果反超GPT4？ - 一堆废纸的回答 - 知乎 https://www.zhihu.com/question/600311066/answer/3022625910

两大可商用开源大模型同时发布！性能不输LLaMA，羊驼家族名字都不够用了 - 量子位的文章 - 知乎 https://zhuanlan.zhihu.com/p/627454901





## 赞助我们

我们是谁？

我们是羡鱼智能【xianyu.ai】，主要成员是一群来自老和山下、西湖边上的咸鱼们，塘主叫作羡鱼，想在LLMs做点有意义的事！我们的口号是：做OpenNLP和OpenX！希望在OpenAI卷死我们之前退出江湖！

ChatPiXiu项目为羡鱼智能【xianyu.ai】发起的OpenNLP计划的第2个正式的开源项目，旨在Open ChatGPT for everyone！在以ChatGPT/GPT4为代表的LLMs时代，在被OpenAI卷死之前，做一点有意义的事情！未来有一天，等到GPT-X发布的时候，或许有人会说NLP不存在了，但是我们想证明有人曾来过！

本项目第一版由本羡鱼利用业务时间（熬夜）独立完成，受限于精力和算力，拖延至今，好在顺利完成了。如果大家觉得本项目对你的NLP学习/研究/工作有所帮助的话，求一个免费的star! 富哥富姐们可以考虑赞助一下！尤其是算力，**租卡的费用已经让本不富裕的鱼塘快要无鱼可摸了**！

<img src="https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image-20230324010955205.png" alt="image-20230324010955205" style="zoom: 25%;" />

## Starchart

[![Star History Chart](https://api.star-history.com/svg?repos=catqaq/ChatPiXiu&type=Date)](https://star-history.com/#catqaq/ChatPiXiu&Date)

## Contributors

<a href="https://github.com/catqaq/ChatPiXiu/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=catqaq/ChatPiXiu" />
</a>
