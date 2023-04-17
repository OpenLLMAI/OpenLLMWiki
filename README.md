<div style="font-size: 1.5rem;">
  <a href="./README.md">中文</a> |
  <a href="./readme_en.md">English</a>
</div>


</br>

<h1 align="center">ChatPiXiu</h1>
<div align="center">
  <a href="https://github.com/catqaq/ChatPiXiu">
    <img src="https://github.com/catqaq/ChatPiXiu/tree/main/docs/imgs/pixiu.jpg" alt="Logo" height="210">
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

| 项目                                                         | 基础模型       | 机构                                              | 数据集                                                       | license                                                      | 介绍                                                         | 备注                                                         |
| ------------------------------------------------------------ | -------------- | ------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [stanford_alpaca](https://github.com/tatsu-lab/stanford_alpaca)<br>Alpaca | LLaMA          | stanford                                          | [alpaca_data](https://github.com/tatsu-lab/stanford_alpaca/blob/main/alpaca_data.json) | [Apache-2.0 license](https://github.com/tatsu-lab/stanford_alpaca/blob/main/LICENSE) | An Instruction-following LLaMA Model.<br>让 OpenAI 的 text-davinci-003 模型以 self-instruct 方式生成 52K 指令样本，SFT |                                                              |
| [ChatLLaMA](https://github.com/nebuly-ai/nebullvm/tree/main/apps/accelerate/chatllama) | LLaMA          | Nebuly+AI                                         | \-                                                           | [license](https://github.com/nebuly-ai/nebullvm/blob/main/apps/accelerate/chatllama/LICENSE) | 数据集创建、使用 RLHF 进行高效训练以及推理优化。             |                                                              |
| [Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca) | LLaMA          | [ymcui](https://github.com/ymcui)                 | \-                                                           | [Apache-2.0 license](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/LICENSE.md) | 中文LLaMA&Alpaca大语言模型+本地CPU/GPU部署 (Chinese LLaMA & Alpaca LLMs) |                                                              |
| [alpaca-lora](https://github.com/tloen/alpaca-lora)          | LLaMA          | stanford                                          | [LLaMA-GPT4 dataset](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM) | [Apache-2.0 license](https://github.com/tloen/alpaca-lora/blob/main/LICENSE) | [LoRA](https://zhuanlan.zhihu.com/p/620327907)               |                                                              |
| [Chinese-alpaca-lora<br/>](https://github.com/LC1332/Chinese-alpaca-lora)[Luotuo-Chinese-LLM](https://github.com/LC1332/Luotuo-Chinese-LLM) | LLaMA          | [LC1332](https://github.com/LC1332)               | -                                                            | [Apache-2.0 license](https://github.com/LC1332/Luotuo-Chinese-LLM/blob/main/LICENSE) | LoRA                                                         |                                                              |
| [ChatGLM](https://github.com/THUDM/ChatGLM-6B)               | GLM            | 清华                                              | 1T 标识符的中英双语数据                                      | [Apache-2.0 license](https://github.com/THUDM/ChatGLM-6B/blob/main/LICENSE) | 监督微调、反馈自助、人类反馈强化学习                         | [PROJECT.md](https://github.com/THUDM/ChatGLM-6B/blob/main/PROJECT.md) |
| [FastChat](https://github.com/lm-sys/FastChat)<br><br>Vicuna | LLaMA          | 斯坦福、CMU、UC伯克利                             | ShareGPT                                                     | [Apache-2.0 license](https://github.com/lm-sys/FastChat/blob/main/LICENSE) | SFT，使用GPT-4作为评判标准，结果显示Vicuna-13B在超过90%的情况下实现了与ChatGPT和Bard相匹敌的能力。 |                                                              |
| [Chinese-Vicuna](https://github.com/Facico/Chinese-Vicuna)   | LLaMA          | \-                                                | \-                                                           | [Apache-2.0 license](https://github.com/Facico/Chinese-Vicuna/blob/master/LICENSE) | LoRA                                                         |                                                              |
| [EasyLM](https://github.com/young-geng/EasyLM)<br>Koala考拉  | LLaMA<br>multi | UC伯克利                                          | ChatGPT数据和开源数据（Open Instruction Generalist (OIG)、斯坦福 Alpaca 模型使用的数据集、Anthropic HH、OpenAI WebGPT、OpenAI Summarization） | [Apache-2.0 license](https://github.com/Facico/Chinese-Vicuna/blob/master/LICENSE) | SFT                                                          |                                                              |
| [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) | LLaMA          | ColossalAI                                        | [](https://github.com/XueFuzhao/InstructionWild)[InstructionWild](https://github.com/XueFuzhao/InstructionWild):104K bilingual datasets | [LICENSE](https://github.com/hpcaitech/ColossalAI/blob/main/applications/Chat/LICENSE) | SFT-RM-RLHF                                                  |                                                              |
| [ChatRWKV](https://github.com/BlinkDL/ChatRWKV)              | RWKV           | [BlinkDL](https://github.com/BlinkDL)             | \-                                                           | [Apache-2.0 license](https://github.com/BlinkDL/ChatRWKV/blob/main/LICENSE) | ChatRWKV is like ChatGPT but powered by RWKV (100% RNN) language model, and open source. |                                                              |
| [ChatYuan](https://github.com/clue-ai/ChatYuan)              | T5             | 元语智能                                          | PromptClue                                                   | [LICENSE](https://github.com/clue-ai/ChatYuan/blob/main/LICENSE) | 基于PromptClue进行了监督微调                                 |                                                              |
| [OpenChatKit](https://github.com/togethercomputer/OpenChatKit) | GPT-NoX-20B    | Together+LAION+Ontocord.ai                        | OIG-43M                                                      | [Apache-2.0 license](https://github.com/togethercomputer/OpenChatKit/blob/main/LICENSE) | 60亿参数的审核模型，对不合适或者是有害的信息进行过滤         |                                                              |
| [BELLE](https://github.com/LianjiaTech/BELLE)                | Bloom<br>LLama | [LianjiaTech](https://github.com/LianjiaTech)     | 10M-ChatGPT生成的数据                                        | [Apache-2.0 license](https://github.com/LianjiaTech/BELLE/blob/main/LICENSE) | SFT                                                          |                                                              |
| [PaLM-rlhf-pytorch](https://github.com/lucidrains/PaLM-rlhf-pytorch) | PaLM           | [lucidrains](https://github.com/lucidrains)       | \-                                                           | [MIT license](https://github.com/lucidrains/PaLM-rlhf-pytorch/blob/main/LICENSE) | RLHF                                                         | PaLM太大了                                                   |
| [dolly](https://github.com/databrickslabs/dolly)             | GPT-J-6B       | \-                                                | \-                                                           | \-                                                           | 参考Alpaca                                                   |                                                              |
| [LMFlow](https://github.com/OptimalScale/LMFlow)             | LLaMA          | [OptimalScale](https://github.com/OptimalScale)   |                                                              |                                                              | An Extensible Toolkit for Finetuning and Inference of Large Foundation Models. Large Model for All.<br>LLaMA-7B，一张3090耗时 5 个小时 |                                                              |
| GPTrillion                                                   | \-             | \-                                                | \-                                                           | \-                                                           | 1.5万亿，多模态                                              |                                                              |
| [open_flamingo](https://github.com/mlfoundations/open_flamingo) | LLaMA<br>CLIP  | LAION                                             | [Multimodal C4](https://github.com/allenai/mmc4)             | [MIT license](https://github.com/mlfoundations/open_flamingo/blob/main/LICENSE) |                                                              |                                                              |
| [baize-chatbot](https://github.com/project-baize/baize-chatbot) | LLaMA          | [project-baize](https://github.com/project-baize) | 100k dialogs generated by letting ChatGPT chat with itself.  | [GPL-3.0 license](https://github.com/project-baize/baize-chatbot/blob/main/LICENSE) | LoRA                                                         |                                                              |
| [ChatPiXiu](https://github.com/catqaq/ChatPiXiu)             | multi          | 羡鱼智能                                          | \-                                                           | \-                                                           | LoRA                                                         | 筹备阶段                                                     |
| [stackllama](https://huggingface.co/blog/stackllama)         | LLaMA          | Hugging Face                                      | \-                                                           | \-                                                           | 用RLHF训练LLaMA的实践指南                                    |                                                              |
| [lit-llama](https://github.com/Lightning-AI/lit-llama)       | LLaMA          | lightening-ai                                     | \-                                                           | [Apache-2.0 license](https://github.com/Lightning-AI/lit-llama/blob/main/LICENSE) | **重写重训LLaMA,绕开license**                                | 概念阶段                                                     |
| [OPT](https://arxiv.org/abs/2205.01068)                      | OPT            | meta                                              | \-                                                           | [MIT license](https://github.com/facebookresearch/metaseq/blob/main/LICENSE) | 当年对标GPT3的模型                                           |                                                              |

### 2.基础模型

| model | 架构 | 机构 | 数据 | license                                                      | 介绍                                                         | 备注 |
| ----- | ---- | ---- | ---- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---- |
| LLaMA |      |      |      | [ GPL-3.0 license](https://github.com/facebookresearch/llama/blob/main/LICENSE) | [当前开源ChatGPT复现中使用最多的基础模型](https://zhuanlan.zhihu.com/p/622190021) |      |
| GLM   |      |      |      | [ Apache-2.0 license](https://github.com/THUDM/ChatGLM-6B/blob/main/LICENSE) | [GLM](https://zhuanlan.zhihu.com/p/622254367),中英双语，可能是当前开源的中文效果最好的基础模型； |      |
| GPT   |      |      |      |                                                              |                                                              |      |
| OPT   |      |      |      |                                                              |                                                              |      |

### 3.数据

| dataset                     | type        | 机构                                | 大小 | license | 介绍 | 备注 |
| --------------------------- | ----------- | ----------------------------------- | ---- | ------- | ---- | ---- |
| alpaca_data                 | Instruction | stanford                            |      |         |      |      |
| alpaca_chinese_dataset      | \-          | hikariming                          |      |         |      |      |
| Multilingual Instruction    |             | Guanaco                             |      |         |      |      |
| alpaca_chinese_dataset      |             | carbonz0                            |      |         |      |      |
| 0.5M+1M chinese instruction |             | LianjiaTech                         |      |         |      |      |
| shareGPT                    |             | [lm-sys](https://github.com/lm-sys) |      |         |      |      |

### 4.训练&部署

#### 4.1 训练

| 框架                                                         | type    | 机构                                      | 兼容性                       | license                                                      | 介绍                                                         | 备注 |
| ------------------------------------------------------------ | ------- | ----------------------------------------- | ---------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---- |
| [ColossalAI](https://github.com/hpcaitech/ColossalAI)        | general | [hpcaitech](https://github.com/hpcaitech) | 高                           | [Apache-2.0 license](https://github.com/hpcaitech/ColossalAI/blob/main/LICENSE) | Colossal-AI: Making large AI models cheaper, faster, and more accessible<br>支持ChatGPT完整复现 |      |
| [RLHF](https://github.com/sunzeyeah/RLHF)                    | RL      | [sunzeyeah](https://github.com/sunzeyeah) | 基于transformers库实现       | \-                                                           | Implementation of Chinese ChatGPT.<br>SFT、Reward Model和RLHF |      |
| trlx                                                         | RL      | [CarperAI](https://github.com/CarperAI)   | 强大的transformer 强化学习库 | [MIT license](https://github.com/CarperAI/trlx/blob/main/LICENSE) | A repo for distributed training of language models with Reinforcement Learning via Human Feedback (RLHF)<br>不支持自定义预训练模型。 |      |
| [trl](https://github.com/lvwerra/trl)                        | RL      | Hugging Face                              | 基于transformers             | [Apache-2.0 license](https://github.com/lvwerra/trl/blob/main/LICENSE) | 只要是基于ransformers 库开发的预训练库，均可适配，强烈推荐   |      |
| [DeepSpeed-Chat](https://github.com/microsoft/DeepSpeedExamples/tree/master/applications/DeepSpeed-Chat) | general | [microsoft](https://github.com/microsoft) | 基于DeepSpeed                | [Apache-2.0 license](https://github.com/microsoft/DeepSpeedExamples/blob/master/LICENSE) | **训练速度**大幅提升                                         |      |

#### 4.2 部署



## 使用步骤：TODO

1.克隆本项目

`git clone https://github.com/catqaq/ChatPiXiu.git`

2.准备数据



3.运行示例



## 结果展示




## 常见报错



## 参考资料&致谢

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