# 年货：24年最火的RAG论文都在这了

## 1. LLM核心应用领域：RAG

2024年，检索增强生成（Retrieval-Augmented Generation, RAG）技术迎来了爆发式的技术发展。无论是学术研究还是产业落地，RAG均以“现象级”姿态重塑了生成式AI的格局。


![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737887079743-3d81b58a-37b2-46a8-9691-b65da9529c53.png)

仅Arxiv平台全年以“Retrieval Augmented Generation”为关键词的论文便高达1223篇，较2023年的92篇，增长将近1229%，其中既有对基础架构的革新，也有面向多模态、检索性能、知识图谱等细分领域的突破性探索。

这种热度源于RAG本身的技术潜力，并且随着模型性能的提高（特别是开源模型）、长上下文窗口技术的成熟，凭借其**实时性**、**灵活性**和**低成本**优势，成为企业、细分领域应对动态知识更新与复杂场景的首选方案。而23年广泛提出的基于大模型Finetune提出的所谓行业大模型却逐渐消失在大家视野。

论文这么多，哪些才值得认真读呢？快过年了，给大家梳理一下，大家过年带回家仔细研究一下。

![加入社群，+v: iamxxn886](assets/qrcode.png)

## 2. 哪些RAG综述值得一读

可以先读这两篇今年早期的RAG综述，系统性了解RAG的历史缘由、技术框架原理

### 第一篇

第一篇综述是来自北大团队，系统性介绍了检索增强生成（RAG）在AI生成内容（AIGC）中的应用：如何通过结合信息检索与生成模型解决知识更新、长尾数据处理等挑战。提出了RAG技术分类框架，分析检索与生成组件的协同机制，总结性能增强方法及跨模态应用场景，并建立评估基准，为优化生成质量、降低计算成本提供理论参考，同时指出未来研究方向。

- 标题：Retrieval-Augmented Generation for AI-Generated Content: A Survey

	- 原文链接：https://arxiv.org/abs/2402.19473
    
    - Github：https://github.com/PKU-DAIR/RAG-Survey
    
    - Google Scholar引用量：166

    - [查看论文](/survey/2402.19473v6.pdf)
    

![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737892434868-211ae002-c052-4ad5-b4d0-b7edb4dabfc1.png)


![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737892303002-c895f73e-527e-45f4-971e-c949fee20e63.png)


![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737892334577-f67d2a7c-9ba2-4f50-abb4-2c9b153ed663.png)

    
--- 

### 第二篇

第二篇综述由香港理工大学、百度公司与新加坡国立大学的联合研究团队共同完成。可相对全面的了解RAG的技术演进脉络、RAG生成质量的关键方法（如检索优化策略）。

- 标题：A Survey on RAG Meeting LLMs: Towards Retrieval-Augmented Large Language Models

	- 原文链接：https://arxiv.org/pdf/2405.06211
    
    - Github：https://advanced-recommender-systems.github.io/RAG-Meets-LLMs/
    
    - Google Scholar引用量：154

    - [查看论文](/survey/2405.06211v3.pdf)

    
    
![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737893675177-3be5e353-bbab-4c45-90f4-3f294970115c.png)


![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737893682493-2726e6aa-0eec-4b5d-8b16-458eb888b757.png)


![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737893688796-1d2ed646-13c1-47bf-89fe-42831d807b90.png)


--- 

### 第三篇

第三篇是由同济大学上海智能自主系统研究院、复旦大学数据科学重点实验室及同济大学设计创意学院团队合作完成。针对传统检索增强生成（RAG）系统"检索-生成"线性架构的局限性，提出模块化RAG框架，通过解耦系统为独立模块和专用算子，实现路由调度、流程融合等动态重组能力。该研究系统梳理了线性、条件、分支、循环四种RAG模式，为构建可重构AI系统提供理论支撑与实践路径。通讯作者为同济大学王昊奋教授。

这篇文章本质上不是一篇综述，但是他梳理了整个RAG的技术路线，给出了各个模块清晰定义，可以视为综述。

- 标题：Modular RAG: Transforming RAG Systems into LEGO-like Reconfigurable Frameworks

	- 原文链接：https://arxiv.org/pdf/2407.21059
    - [查看论文](/survey/2407.21059v1.pdf)

    
![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737894129470-fe1f28ab-20c5-4010-93a2-62f96a0a301b.png)

---

### 第四篇

第四篇由卡内基梅隆大学撰写，系统梳理了RAG技术演进与前沿发展。研究深入解析RAG融合检索机制与生成模型的核心架构，讨论其在问答、摘要等知识密集型任务中的应用突破，并评述检索效率优化等关键技术进展。剖析了当前面临的扩展性、伦理偏差等挑战，更提出增强模型鲁棒性、拓展应用边界等未来研究方向，为自然语言处理领域研究者提供重要参考框架。

- 标题：A Comprehensive Survey of Retrieval-Augmented Generation (RAG): Evolution, Current Landscape and Future Directions

	- 原文链接：https://arxiv.org/pdf/2410.12837

    - [查看论文](/survey/2410.12837v1.pdf)

 
![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737894530981-c41e02fa-40ea-4122-a473-bb436bc46043.png)

---

### 第五篇：GraphRAG

第五篇由北京大学、浙江大学、蚂蚁集团、中国人民大学和罗格斯大学的多学科团队联合撰写，系统综述GraphRAG技术。研究团队提出GraphRAG的三阶段框架——基于图的索引构建、图引导知识检索和图增强内容生成，重点解决大语言模型的知识幻觉、领域适应性不足和动态更新难题。

- 标题：Graph Retrieval-Augmented Generation: A Survey

	- 原文链接：https://arxiv.org/pdf/2408.08921
    
    - Github：https://github.com/pengboci/GraphRAG-Survey
    
    - Github：https://github.com/circlemind-ai/fast-graphrag

    - [查看论文](/survey/2408.08921v2.pdf)

   
![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737895062281-e7a14ccc-fa71-4b71-952c-fe3bd977b835.png)

---

### 第六篇：AgenticRAG

第六篇针对传统检索增强生成（RAG）系统静态工作流的局限性，提出了Agentic RAG创新框架。系统阐述了如何通过自主AI代理的反思、规划、工具调用与多智能体协作机制，实现动态数据检索与上下文迭代优化，显著提升了LLM在医疗、金融和教育等领域的复杂任务处理能力，同时探讨了系统扩展性、伦理决策与性能优化等核心挑战，为下一代上下文感知AI系统提供了理论框架与实践指南。

- 标题：Agentic Retrieval-Augmented Generation: A Survey on Agentic RAG

	- 原文标题：https://arxiv.org/pdf/2501.09136
    
    - Github：https://github.com/asinghcsu/AgenticRAG-Survey

    - [查看论文](/survey/2501.09136v1.pdf)

    
![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737897706872-6af86e21-e8a8-479c-8ecb-a30092189582.png)

![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737897714563-1418277d-8dfb-4d1c-98c8-6cc7f8282541.png)


## 2. 架构创新

第二部分，我们来看看在架构创新这块，有哪些值得大家一读的论文。

### 第一篇：混合检索，Blended RAG

第一篇论文是来自IBM团队的，通过融合语义搜索中的密集向量索引与稀疏编码器索引，结合混合查询策略优化检索增强生成（RAG）系统的准确性。

- 标题：Blended RAG: Improving RAG (Retriever-Augmented Generation) Accuracy with Semantic Search and Hybrid Query-Based Retrievers

	- 原文链接：https://arxiv.org/pdf/2404.07220

    - [查看论文](/arch/2404.07220v2.pdf)

   
![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737895480311-56193b4e-f1e0-47a5-8927-03243250a931.png)

---

### 第二篇：Self-RAG

第二篇论文由华盛顿大学、艾伦人工智能研究所和IBM Research AI团队联合开发的SELF-RAG（自反思RAG）通过自我反思机制提升语言模型的生成质量与事实性。训练单一模型动态决策检索需求，利用特殊标记评估检索段落相关性并批判生成内容，实现按需检索和输出优化。在开放域问答、推理等任务中优于ChatGPT及检索增强的Llama2-chat，显著提高了长文本生成的事实准确性和引用可靠性。

- 标题：Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection

	- 原文链接：https://openreview.net/pdf?id=hSyW5go0v8

    - [查看论文](/arch/6283_Self_RAG_Learning_to_Retr.pdf)

![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737896140861-723733ed-da65-489b-9568-7593013b6693.png)

---

### 第三篇：GraphRAG

第三篇就是本年度最火的新RAG框架 - GraphRAG。本篇论文由微软团队贡献，通过两阶段图索引构建：首先从文档中提取实体知识图谱，进而生成紧密关联实体的社区摘要。查询时，系统对各社区生成局部响应，再综合形成全局回答。

- 标题：From Local to Global: A Graph RAG Approach to Query-Focused Summarization

	- 原文链接：https://arxiv.org/pdf/2404.16130
    
    - Github：https://github.com/microsoft/graphrag
    
    - [查看论文](/arch/2404.16130v1.pdf)

![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737896756170-ec0e17d1-ce70-4904-b76d-3590d7935882.png)

---

### 第四篇：LightRAG

第四篇是比GraphRAG更火、更快的LightRAG。由北京邮电大学与香港大学团队联合提出，将图结构引入检索增强生成框架，通过双层次检索机制（低阶实体与高阶语义关系）解决传统RAG的上下文割裂问题。结合图结构与向量表示，实现高效关联检索，响应速度提升显著，并设计增量更新算法动态适应数据变化。检索准确率与效率优于现有方案，已开源为动态知识场景提供轻量解决方案。

- 标题：LightRAG: Simple and Fast Retrieval-Augmented Generation

	- 原文链接：https://arxiv.org/pdf/2410.05779
    
    - Github：https://github.com/HKUDS/LightRAG
    
    - [查看论文](/arch/2410.05779v2.pdf)

![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737897783089-a299268d-d373-40a1-bd8a-909af4809a36.png)

---

### 第五篇：KAG

第五篇是由蚂蚁集团知识图谱团队与浙江大学合作研发的知识增强生成框架KAG，针对专业领域RAG技术在逻辑推理和知识关联性上的不足，提出知识图谱与向量检索协同增强方案。

- 标题：KAG: Boosting LLMs in Professional Domains via Knowledge Augmented Generation

	- 原文链接：https://arxiv.org/pdf/2409.13731
    
    - Github：https://github.com/OpenSPG/KAG

    - [查看论文](/arch/2409.13731v3.pdf)

![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2025/01/26/1737898011935-98b21bf2-fcdd-44d4-a4bc-c028d8c03e51.png)

    
---

### 第六篇：HybridRAG

第六篇是由BlackRock与NVIDIA团队联合完成，介绍了HybridRAG方法，融合知识图谱（GraphRAG）与向量检索（VectorRAG）技术，以解决金融领域复杂非结构化文本（如财报电话会议记录）的信息抽取难题。通过结合图数据库的结构化语义关系和向量检索的语义相似性，该方法在真实问答对测试中，检索准确率和生成答案质量均优于单一技术，为跨领域知识密集型任务提供了高效解决方案。

- 标题：HybridRAG: Integrating Knowledge Graphs and Vector Retrieval Augmented Generation for Efficient Information Extraction

	- 原文链接：https://arxiv.org/pdf/2408.04948

    - [查看论文](/arch/2408.04948v1.pdf)



<hr />

- 获取更多最新 Arxiv 论文更新: [https://github.com/HuggingAGI/HuggingArxivLLM](https://github.com/HuggingAGI/HuggingArxivLLM)!
- 加入社群，+v: iamxxn886
- 点击公众号菜单加入讨论
  ![](https://raw.githubusercontent.com/HuggingAGI/wx_assets/main/2024/07/31/1722434818326-94339e92-22f1-4472-9d27-fed232f70b5d.jpeg)
