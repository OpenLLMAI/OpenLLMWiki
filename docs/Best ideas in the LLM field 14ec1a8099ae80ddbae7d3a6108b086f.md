# Best ideas in the LLM field

# 写在前面：

## 更新日志：

20241201：初稿，时间关系，先强行停在这里了，本文不定期更新，大家感兴趣的可以留言补充。

## 转载及引用事宜：

转载请注明出处：[https://openllmai.notion.site/Best-ideas-in-the-LLM-field-14ec1a8099ae80ddbae7d3a6108b086f](https://www.notion.so/Best-ideas-in-the-LLM-field-14ec1a8099ae80ddbae7d3a6108b086f?pvs=21)

引用：

xianyu. (Nov. 01, 2024). 《Best ideas in the LLM field》[Blog post]. [https://openllmai.notion.site/Best-ideas-in-the-LLM-field-14ec1a8099ae80ddbae7d3a6108b086f](https://www.notion.so/Best-ideas-in-the-LLM-field-14ec1a8099ae80ddbae7d3a6108b086f?pvs=21)

@online{xianyu-LLMIdeas,

title={Best ideas in the LLM field},

author={xianyu},

year={2024},

month={Dec},

org={OpenLLMAI},

url={\url{[https://openllmai.notion.site/Best-ideas-in-the-LLM-field-14ec1a8099ae80ddbae7d3a6108b086f](https://www.notion.so/Best-ideas-in-the-LLM-field-14ec1a8099ae80ddbae7d3a6108b086f?pvs=21)}},

}

## 背景：

去年笔者总结了[深度学习领域最令人惊艳&最重要的想法和论文](https://www.zhihu.com/question/440729199/answer/2629696353)，这两天刚好看到一个镜像问题-[大模型领域，你心目中 idea 最惊艳的论文是哪篇？ - 知乎](https://www.zhihu.com/question/665735775)，有感而作此文，想和大家一起聊聊大模型领域一些最好的ideas，总结过去也展望未来。

本文侧重于讨论LLM领域中一些惊艳的、有趣的idea，同时兼顾重要性，全面性暂时无法保证；结构上会以ChatGPT为界分成3个阶段：LLM之前、ChatGPT时代和未来展望。

# 1.LLM之前：

*AGI不是一日建成的，况且现在离AGI还很远。*

## 思想基石：

1.压缩即智能

预训练的本质在做什么？什么是智能？怎么达成智能？

老实说，在ChatGPT火爆之前，本人对这些星辰大海的终极问题基本上是缺乏深度思考的。但是，总有人要去想呀！

**压缩即智能**，这个观点给我的感觉有点像**捅破了智能之神身前的迷雾**，让智能不再遥不可及、高不可攀，这一点甚至比观点本身更为重要。

在这个观点下，MLM也好，NTP也罢，只是实现压缩的一种训练方式罢了，对于AGI可能不一定够，而通往AGI的路或许也不止一条。我们也许不一定走在完全正确的路上，但重要的是永远有人在路上！

- Jack Rae 分享视频：[**Compression for AGI - Jack Rae | Stanford MLSys #76**](https://www.youtube.com/watch?v=dO4TPJkeaaU)
- 北京大学分享：【Compression For AGI：压缩即智慧，大语言模型LLM是最好的无损压缩器-哔哩哔哩】 [https://b23.tv/RwEARtr](https://link.zhihu.com/?target=https%3A//b23.tv/RwEARtr)
- [**Why next-token prediction is enough for AGI - Ilya Sutskever (OpenAI Chief Scientist)**](https://www.youtube.com/watch?v=YEUclZdj_Sc)

2.scaling law：

*OpenAI早期的工作：Scaling Laws for Neural Language Models:* [https://arxiv.org/abs/2001.08361](https://arxiv.org/abs/2001.08361)

[关于scaling law 的正确认识 - 曾冠奇的文章 - 知乎](https://zhuanlan.zhihu.com/p/684955373)，评论区有一些总结可以看看。另外需要特别注意的是，scaling law不是一个固定的东西，其实一直在变化，和具体的任务也有关系，可以借鉴思想，但不要生搬硬套。

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image.png)

推荐阅读：

survey：[https://openreview.net/pdf?id=xI71dsS3o4](https://openreview.net/pdf?id=xI71dsS3o4)

解析大模型中的Scaling Law - nghuyong的文章 - 知乎
[https://zhuanlan.zhihu.com/p/667489780](https://zhuanlan.zhihu.com/p/667489780)

最近，随着O1的发布，也有一些关于**inference scaling law的讨论了。**

o1 系列：inference scaling law - 周波的文章 - 知乎
[https://zhuanlan.zhihu.com/p/839046978](https://zhuanlan.zhihu.com/p/839046978)

3.涌现能力：可能不是做不到，只是模型还不够大

**Emergent Abilities of Large Language Models，能力的出现不是平滑的，这一点倒是很合理，看看武侠小说里面的主角就知道了哈哈。**

## 结构基石：

1.transformers：开启大规模预训练时代，[attention is all you need](https://arxiv.org/abs/1706.03762)!

**没什么好说的，深度学习模型结构的开创性工作，彻底抛开CNN和RNN，建立以self-attention机制为核心的transformers网络，成为后来LLM领域的奠基性工作。**

后来统治NLP领域长达4年的Bert类模型，就是基于transformer-encoder架构的模型，虽然比不上当今ChatGPT的影响力，但证明了预训练模型的强大能力。现在bert有些out了，说起来真是时代的眼泪，毕竟曾经带着NLPer走过黑暗岁月，至今也依然在发挥余热，有些思想还是可以借鉴的。

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%201.png)

2.word2vec：NLP预训练的奠基之作

词嵌入领域的经典之作，也是NLP预训练的奠基性工作，思想简单（由中心词预测上下文skip-gram或者由上下文预测中心词CBOW），效果很好，两个训练的优化算法negative sampling和分层softmax也很有启发。其实个人认为，现今LLM的embedding技术也并没有逃出word2vec的思想，无法是训练方式和使用方式有点儿变化而已。

- 训练目标：由由中心词预测上下文/由上下文预测中心词 -》以bert为代表的MLM/以GPT为代表的NTP
- 使用方式：offline → online

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%202.png)

3.dropout：**preventing co-adaptation**

通过随机丢掉一些神经元来**preventing co-adaptation以缓解过拟合。**

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%203.png)

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%204.png)

4.resnet：解锁更深的模型

在知乎上有个关于resnet的讨论，Resnet是否只是一个深度学习的trick？ - 知乎，个人认为当然不是，resnet堪称大道至简的典范，通过简单的shortcut/skip connection极大的改善了深度网络的过拟合问题，我们可以开始训练更深的模型。
[https://www.zhihu.com/question/459892388](https://www.zhihu.com/question/459892388)

paper：[https://arxiv.org/abs/1512.03385](https://arxiv.org/abs/1512.03385)

5.position encoding：弥补attention机制之缺陷

self-attention好是好，但是有个致命的缺陷，这玩意儿是对称的、是位置无关的，而文本或者说序列数据天生就是位置敏感的。这里必须提到苏神的[RoPE](https://arxiv.org/abs/2104.09864)，位置编码领域非常优雅的工作，同时也是当前最常用的选择。从原始transformer的sin正弦位置编码到bert时代的learned 位置编码，再到后面的ROPE、alibi等等，位置编码技术逐步从绝对位置建模走向相对位置建模和可扩展性技术，尤其在追求long context和long generation的时代，位置编码发挥着非常重要的作用。

## 训练基石：

分布式训练领域其实有很多绝妙的想法，感兴趣的可以去看看细节，本人在infra方面经验有限就不展开了。

- deepspeed的zero系列：alignment阶段的主流
    - [https://github.com/microsoft/DeepSpeed](https://github.com/microsoft/DeepSpeed)
- Megatron-LM的TP、PP系列：预训练阶段的主流
    - https://github.com/NVIDIA/Megatron-LM
    - 【Megatron LM 论文精读【论文精读】】 [https://www.bilibili.com/video/BV1nB4y1R7Yz/?share_source=copy_web&vd_source=9e7882f0ef2735e23d66a6f128612943](https://www.bilibili.com/video/BV1nB4y1R7Yz/?share_source=copy_web&vd_source=9e7882f0ef2735e23d66a6f128612943)
- pytorch原生的FSDP系列：发展迅速，llama系列原生应该用的是FSDP，所谓人生苦短，我用torch；
    - [https://github.com/OpenRLHF/OpenRLHF/issues/530](https://github.com/OpenRLHF/OpenRLHF/issues/530)

# 2.ChatGPT时代

## 算法层

相比各种各样的模型和数据，算法层本身的进展不算多，但也绝不算少，不过真正能让人眼前一亮的确实不多。

1.RLHF：

- [**InstructGPT: Training language models to follow instructions with human feedback (OpenAI Alignment Team 2022)**](https://openai.com/blog/instruction-following/)
- 框架（私货，但确实不错hh）：[https://github.com/OpenRLHF/OpenRLHF](https://github.com/OpenRLHF/OpenRLHF)

到了2024年年末，RLHF至今已觉不新鲜了。但是时间倒回去，在22年年末，这个东西还是非常有趣的。其实RLHF中RL部分的PPO算法是更老的东西，OpenAI 2017年的工作，所以这里重要的是如何设计一个优雅的框架把RL引入到LM建模并且把它做work。后者是个更Open的问题了，这里按下不表。

我记得之前知乎上有个蛮热门的问题，为什么RL领域没有预训练模型？个人观点是，数据和通用性问题导致没有预训练的必要。随着预训练LM的能力增长，让RM+LM开始变得可能。我们为什么不训练一个语言模型来给语言模型打分呢？实际上，这就是RLHF的核心观点（当然了，这肯定是事后诸葛亮了）。

PT model → SFT model，获得指令遵循的能力；随后在SFT模型基础上训练一个reward model（一般是判别式的，但是生成式的也OK，可能效果还更好），最后采用RL算法利用RM信号来对policy model（可以从SFT模型初始化）进行优化。在实际的训练中会涉及到4个模型，其中actor和critic需要训练，而RM和reference则不需要。

那么怎么理解这个架子？通俗的来说（此比喻最早应该是从何枝佬那儿看到的），actor就是你，RM是个考官或者裁判，critic是你的私教（可以指点细节），而reference model是过去的你（避免步子迈的太大了）。

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%205.png)

具体的原理和代码，推荐阅读猛猿小姐姐的文章，上图也来自于文1的封面：

- 图解大模型RLHF系列之：人人都能看懂的PPO原理与源码解读 - 猛猿的文章 - 知乎
[https://zhuanlan.zhihu.com/p/677607581](https://zhuanlan.zhihu.com/p/677607581)
- 人人都能看懂的RL-PPO理论知识 - 猛猿的文章 - 知乎
[https://zhuanlan.zhihu.com/p/7461863937](https://zhuanlan.zhihu.com/p/7461863937)
- [https://huggingface.co/blog/zh/rlhf](https://huggingface.co/blog/zh/rlhf)

2.DPO：

DPO可以看做是RLHF的一个比较优雅的简化，当然你也可以认为和RL没啥关系，这并不重要，重要的是隐式奖励模型的观点。DPO由于简单有效，目前可能是学姐和业界都研究的比较多的算法了。

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%206.png)

推荐阅读，推导不算复杂，实现也不难，重要的是实践，DPO在实践中并没有理论上那么美好：

- DPO 是如何简化 RLHF 的 - 朱小霖的文章 - 知乎
[https://zhuanlan.zhihu.com/p/671780768](https://zhuanlan.zhihu.com/p/671780768)
- **Direct Preference Optimization: Your Language Model is Secretly a Reward Model**

        [https://arxiv.org/abs/2305.18290](https://arxiv.org/abs/2305.18290)

- **From r to Q∗: Your Language Model is Secretly a Q-Function**

        [https://arxiv.org/abs/2404.12358](https://arxiv.org/abs/2404.12358)

3.MOE相关：暂不展开

MOE在算法设计和分布式训练上都带来了更大的挑战，我们以后有机会再聊。

## 数据/应用层：

数据层有一些通用的方法，也有一些和应用息息相关的方法，这里放到一起说了。

1.COT

COT可以提升LLM的推理和思维能力，简单有效。

**Chain-of-Thought Prompting Elicits Reasoning in Large Language Models：**[https://arxiv.org/abs/2201.11903](https://arxiv.org/abs/2201.11903)

2.MCTS构建推理数据：

MCTS本身不算什么新东西，这波火主要是因为o1带来的，作为主流的复现路径之一受到了不小的关注，但如何提高搜索效率、如何获得可靠的奖励信号才是关键。

大模型领域，你心目中 idea 最惊艳的论文是哪篇？ - Trisimo崔思莫的回答 - 知乎
[https://www.zhihu.com/question/665735775/answer/3611179773](https://www.zhihu.com/question/665735775/answer/3611179773)

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%207.png)

3.执行反馈：

human feedback/AI feedback之外，执行反馈是代码、计算相关任务的应有之义，倒谈不上惊艳，只是以前谈的少，在这儿提一嘴。

4.复杂指令

比如指令进化：**WizardLM: Evol-Instruct，思路是比较简单朴素、可扩展的。**

- 原文链接: [https://arxiv.org/pdf/2304.12244.pdf](https://arxiv.org/pdf/2304.12244.pdf)
- github链接: [https://github.com/nlpxucan/WizardLM](https://github.com/nlpxucan/WizardLM)

5.**SynopGround：视频定位**

根据文字需求找视频画面，真的很有用好不好，尤其对于当今的短视频行业。

“**SynopGround是一个大规模的数据集，开启了一种新的研究方向，叫做多段落视频定位。这个研究是关于怎么在很长的视频里，根据一些详细的段落文字描述找到对应的画面。”**

大模型领域，你心目中 idea 最惊艳的论文是哪篇？ - 数据猎手小K的回答 - 知乎
[https://www.zhihu.com/question/665735775/answer/3616819759](https://www.zhihu.com/question/665735775/answer/3616819759)

6.使用电脑

如何评价 Claude 的新功能 Computer use? - 知乎
[https://www.zhihu.com/question/1791732928](https://www.zhihu.com/question/1791732928)

## critic/评估层：

1.不确定性度量

![image.png](https://xianyunlp.oss-cn-hangzhou.aliyuncs.com/uPic/image%208.png)

from：大模型领域，你心目中 idea 最惊艳的论文是哪篇？ - Beyond Hsueh的回答 - 知乎
[https://www.zhihu.com/question/665735775/answer/3611972970](https://www.zhihu.com/question/665735775/answer/3611972970)

2.LLM-as-a-judge：

很简单的想法，大家也一直在这么干，不过这东西可以套娃，要做好并不容易。

比如：[**Meta-Rewarding Language Models: Self-Improving Alignment with LLM-as-a-Meta-Judge**](https://arxiv.org/abs/2407.19594)

3.GenRM：暂不展开

4.PRM：暂不展开

# 3.展望未来

这里大部分为纯个人看法，请谨慎参考~

- 有趣的AI：有个观点是只有用大部分情况是真没用，挣不到钱。和人一样，有用之上，还得有趣，不然出不了好的应用。
- world RM and efficient RLHF：
    - discriminative RM
    - GenRM
    - PRM
    - efficient RLHF
- 高级能力：
    - 推理：math、code…
    - 情感
    - 幽默感
- MOE：暂不展开
- agent：不好说，上限很高，但是真的不好搞，纯prompt工程肯定是不太行的。
- 应用层：
    - 生成式搜索：两年过去，道理都懂，但做好真的不容易
    - 生成式广告：据我所知，这里有朋友做了一些很骚的东西了，大家可以开开脑洞，如果能让广告变得有趣一些、自然一些，也算是一件功德了。
    - 情感陪伴：海外市场还不错，情感和长文记忆很关键。
    - 办公场景：算是目前落地做的比较好的领域了。

# 参考资料：

1. [https://www.cnblogs.com/lsgsanxiao/p/18159871](https://www.cnblogs.com/lsgsanxiao/p/18159871) | 压缩即智能：为什么 ChatGPT 拥有智能？（转） - 三小 - 博客园 
2. [https://blog.csdn.net/weixin_65514978/article/details/140587617](https://blog.csdn.net/weixin_65514978/article/details/140587617) | 【大模型理论篇】压缩泛化-对大语言模型智能涌现的理解_compression for agi-CSDN博客
3. [https://www.reddit.com/r/LocalLLaMA/comments/1c60h88/relationship_between_intelligence_and_compression/](https://www.reddit.com/r/LocalLLaMA/comments/1c60h88/relationship_between_intelligence_and_compression/) | Relationship Between Intelligence and Compression in Large Language Models : r/LocalLLaMA
4. [https://www.youtube.com/watch?v=dO4TPJkeaaU](https://www.youtube.com/watch?v=dO4TPJkeaaU) | Compression for AGI - Jack Rae | Stanford MLSys #76 - YouTube
5. [https://www.reddit.com/r/singularity/comments/18hl2l9/why_nexttoken_prediction_is_enough_for_agi_ilya/](https://www.reddit.com/r/singularity/comments/18hl2l9/why_nexttoken_prediction_is_enough_for_agi_ilya/) | Why next-token prediction is enough for AGI - Ilya Sutskever : r/singularity
6. [https://www.youtube.com/watch?v=YEUclZdj_Sc](https://www.youtube.com/watch?v=YEUclZdj_Sc) | Why next-token prediction is enough for AGI - Ilya Sutskever (OpenAI Chief Scientist) - YouTube
7. [https://www.google.com/searchq=scaling+law+survey&sca_esv=c568a49474654ded&sxsrf=ADLYWIIQ7xx_JTn1SNlOwZoVdLq22IgdrQ%3A1733044493425&ei=DSlMZ7bSGcek0-kPq6eskAk&ved=0ahUKEwj2jKTrnYaKAxVH0jQHHasTC5IQ4dUDCA8&uact=5&oq=scaling+law+survey&gs_lp=Egxnd3Mtd2l6LXNlcnAiEnNjYWxpbmcgbGF3IHN1cnZleTIFEAAYgAQyCBAAGIAEGKIEMggQABiABBiiBDIIEAAYgAQYogQyCBAAGIAEGKIESOMhUN4EWM0ecAF4AZABAJgB-gGgAbQNqgEFMC4yLja4AQPIAQD4AQGYAgmgAsoNwgIKEAAYsAMY1gQYR8ICBxAjGLECGCfCAgoQABiABBhDGIoFwgIJEAAYgAQYChgMwgIEEAAYHsICBhAAGAgYHpgDAIgGAZAGCpIHBTEuMi42oAe7Eg&sclient=gws-wiz-serp](https://www.google.com/search?q=scaling+law+survey&sca_esv=c568a49474654ded&sxsrf=ADLYWIIQ7xx_JTn1SNlOwZoVdLq22IgdrQ%3A1733044493425&ei=DSlMZ7bSGcek0-kPq6eskAk&ved=0ahUKEwj2jKTrnYaKAxVH0jQHHasTC5IQ4dUDCA8&uact=5&oq=scaling+law+survey&gs_lp=Egxnd3Mtd2l6LXNlcnAiEnNjYWxpbmcgbGF3IHN1cnZleTIFEAAYgAQyCBAAGIAEGKIEMggQABiABBiiBDIIEAAYgAQYogQyCBAAGIAEGKIESOMhUN4EWM0ecAF4AZABAJgB-gGgAbQNqgEFMC4yLja4AQPIAQD4AQGYAgmgAsoNwgIKEAAYsAMY1gQYR8ICBxAjGLECGCfCAgoQABiABBhDGIoFwgIJEAAYgAQYChgMwgIEEAAYHsICBhAAGAgYHpgDAIgGAZAGCpIHBTEuMi42oAe7Eg&sclient=gws-wiz-serp) | scaling law survey
8. [https://axk51013.medium.com/llm專欄-迎接2024年-10個必須要搞懂的llm概念-1-scaling-law-5f6a409d35c5](https://axk51013.medium.com/llm%E5%B0%88%E6%AC%84-%E8%BF%8E%E6%8E%A52024%E5%B9%B4-10%E5%80%8B%E5%BF%85%E9%A0%88%E8%A6%81%E6%90%9E%E6%87%82%E7%9A%84llm%E6%A6%82%E5%BF%B5-1-scaling-law-5f6a409d35c5) | 【LLM 10大觀念-1】Scaling Law. 迎接2024年：10個必須要搞懂的LLM概念-1 | by 倢愷 Oscar | Medium
9. [https://arxiv.org/abs/2001.08361](https://arxiv.org/abs/2001.08361) | [2001.08361] Scaling Laws for Neural Language Models
10. [https://openreview.net/forum?id=xI71dsS3o4](https://openreview.net/forum?id=xI71dsS3o4) | (Mis)Fitting Scaling Laws: A Survey of Scaling Law Fitting Techniques in Deep Learning | OpenReview
11. [https://openreview.net/pdf?id=xI71dsS3o4](https://openreview.net/pdf?id=xI71dsS3o4) | pdf
12. [https://epoch.ai/blog/scaling-laws-literature-review](https://epoch.ai/blog/scaling-laws-literature-review) | Scaling Laws Literature Review | Epoch AI
13. [https://www.zhihu.com/search?type=content&q=scaling law综述最新](https://www.zhihu.com/search?type=content&q=scaling%20law%E7%BB%BC%E8%BF%B0%E6%9C%80%E6%96%B0) | scaling law综述最新 - 搜索结果 - 知乎
14. [https://zhuanlan.zhihu.com/p/684955373](https://zhuanlan.zhihu.com/p/684955373) | 关于scaling law 的正确认识 - 知乎
15. [https://zhuanlan.zhihu.com/p/667489780](https://zhuanlan.zhihu.com/p/667489780) | 解析大模型中的Scaling Law - 知乎
16. [https://zhuanlan.zhihu.com/p/839046978](https://zhuanlan.zhihu.com/p/839046978) | o1 系列：inference scaling law - 知乎
17. [https://www.zhihu.com/search?type=content&q=RLHF](https://www.zhihu.com/search?type=content&q=RLHF) | (76 条消息) RLHF - 搜索结果 - 知乎
18. [https://zhuanlan.zhihu.com/p/677607581](https://zhuanlan.zhihu.com/p/677607581) | 图解大模型RLHF系列之：人人都能看懂的PPO原理与源码解读 - 知乎
19. [https://zhuanlan.zhihu.com/p/7461863937](https://zhuanlan.zhihu.com/p/7461863937) | 人人都能看懂的RL-PPO理论知识 - 知乎
20. [https://zhuanlan.zhihu.com/p/624589622](https://zhuanlan.zhihu.com/p/624589622) | 详解大模型RLHF过程（配代码解读） - 知乎
21. [https://huggingface.co/blog/zh/rlhf](https://huggingface.co/blog/zh/rlhf) | ChatGPT 背后的“功臣”——RLHF 技术详解
22. [https://zhuanlan.zhihu.com/p/671780768](https://zhuanlan.zhihu.com/p/671780768) | DPO 是如何简化 RLHF 的 - 知乎
23. [https://arxiv.org/abs/2305.18290](https://arxiv.org/abs/2305.18290) | [2305.18290] Direct Preference Optimization: Your Language Model is Secretly a Reward Model
24. [https://arxiv.org/abs/2404.12358](https://arxiv.org/abs/2404.12358) | [2404.12358] From $r$ to $Q^*$: Your Language Model is Secretly a Q-Function
25. [https://github.com/OpenRLHF/OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) | OpenRLHF/OpenRLHF: An Easy-to-use, Scalable and High-performance RLHF Framework (70B+ PPO Full Tuning & Iterative DPO & LoRA & RingAttention)
26. [https://www.zhihu.com/search?type=content&q=LLM 最好的idea](https://www.zhihu.com/search?type=content&q=LLM%20%E6%9C%80%E5%A5%BD%E7%9A%84idea) | (75 条消息) LLM 最好的idea - 搜索结果 - 知乎
27. [https://www.zhihu.com/question/665735775/answer/3617148056](https://www.zhihu.com/question/665735775/answer/3617148056) | (75 条消息) 大模型领域，你心目中 idea 最惊艳的论文是哪篇？ - 知乎
28. [https://arxiv.org/abs/2201.11903](https://arxiv.org/abs/2201.11903) | [2201.11903] Chain-of-Thought Prompting Elicits Reasoning in Large Language Models
29. [https://www.zhihu.com/search?type=content&q=Claude computer use](https://www.zhihu.com/search?type=content&q=Claude%20computer%20use) | (1 封私信 / 77 条消息) Claude computer use - 搜索结果 - 知乎
30. [https://www.zhihu.com/question/1791732928/answer/12845008970](https://www.zhihu.com/question/1791732928/answer/12845008970) | (1 封私信 / 77 条消息) 如何评价 Claude 的新功能 Computer use? - 知乎
31. [https://www.zhihu.com/question/637595961/answer/3414267874](https://www.zhihu.com/question/637595961/answer/3414267874) | (75 条消息) 2024年大模型LLM还有哪些可研究的方向？ - 知乎
32. [https://www.zhihu.com/question/642440575/answer/3400886291](https://www.zhihu.com/question/642440575/answer/3400886291) | (75 条消息) 研究课题是LLM和推荐系统结合，有没有好的idea？ - 知乎
33. [https://zhuanlan.zhihu.com/p/708492953](https://zhuanlan.zhihu.com/p/708492953) | LLM---代码大模型(Code LLM)优秀工作解读 - 知乎
34. [https://www.zhihu.com/question/440729199/answer/2629696353](https://www.zhihu.com/question/440729199/answer/2629696353) | (1 封私信 / 77 条消息) 深度学习领域，你心目中 idea 最惊艳的论文是哪篇？ - 知乎
35. [https://www.zhihu.com/question/459892388](https://www.zhihu.com/question/459892388) | (1 封私信 / 77 条消息) Resnet是否只是一个深度学习的trick？ - 知乎
36. [https://arxiv.org/abs/1706.03762](https://arxiv.org/abs/1706.03762) | [1706.03762] Attention Is All You Need
37. [https://arxiv.org/pdf/1310.4546](https://arxiv.org/pdf/1310.4546) | countries.capitals.projections.eps
38. [https://arxiv.org/abs/1512.03385](https://arxiv.org/abs/1512.03385) | [1512.03385] Deep Residual Learning for Image Recognition
39. [https://arxiv.org/abs/2104.09864](https://arxiv.org/abs/2104.09864) | [2104.09864] RoFormer: Enhanced Transformer with Rotary Position Embedding
40. [https://arxiv.org/abs/1207.0580](https://arxiv.org/abs/1207.0580) | [1207.0580] Improving neural networks by preventing co-adaptation of feature detectors
41. [https://www.cs.toronto.edu/~rsalakhu/papers/srivastava14a.pdf](https://www.cs.toronto.edu/~rsalakhu/papers/srivastava14a.pdf) | srivastava14a.pdf
42. [https://arxiv.org/abs/2407.19594](https://arxiv.org/abs/2407.19594) | [2407.19594] Meta-Rewarding Language Models: Self-Improving Alignment with LLM-as-a-Meta-Judge
43. [https://mingchao.wang/LO8uep9D/](https://mingchao.wang/LO8uep9D/) | Index - 笔记
44. [https://github.com/OpenRLHF/OpenRLHF/issues/530](https://github.com/OpenRLHF/OpenRLHF/issues/530) | 训练引擎支持 pytorch FSDP · Issue #530 · OpenRLHF/OpenRLHF
45. [https://github.com/microsoft/DeepSpeed](https://github.com/microsoft/DeepSpeed) | microsoft/DeepSpeed: DeepSpeed is a deep learning optimization library that makes distributed training and inference easy, efficient, and effective.
46. [https://github.com/NVIDIA/Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | NVIDIA/Megatron-LM: Ongoing research training transformer models at scale