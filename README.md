# 李嘉宇 · Li Jiayu

武汉大学 · 网络空间安全 · 本科在读（2023–2027）

关注大模型智能体系统的工程可靠性与应用安全。

📧 2728288049@qq.com　·　📍 武汉

---

## 研究方向

- **大模型智能体系统的工程可靠性** —— 多 Agent 架构、配置与代码解耦、上下文管理与降级容错
- **大模型可信与应用安全** —— 群体偏见量化与归因分析、企业资产测绘与漏洞检测

## 精选项目

### 天命：AI 君主模拟器 —— 六部 Multi-Agent 系统

腾讯游戏引擎技术远程课题。基于大语言模型的古风策略游戏，本人参与 Multi-Agent 系统设计
与 Agent 层开发：六部（吏 / 户 / 礼 / 兵 / 刑 / 工）各由独立 JSON 配置驱使人设、职责、
部门协作关系与 Prompt 模板，实现**配置与代码分离**；实现按世界数值阈值与概率触发的事件
系统、由 LLM 动态排序的群聊发言调度，以及模型不可用时的**关键词匹配降级方案**。
系统最终落地 **9 个** Agent、**11 项**世界指标与 **22 个**后端接口。

`Node.js` `Express` `豆包（火山方舟）API` `Multi-Agent` `Prompt 工程`

### 大模型情感分析公平性与偏见量化复现

复现 Knowledge-Based Systems 2025 论文
《Fairness and Social Bias Quantification in Large Language Models for Sentiment Analysis》。
将面向多卡环境的上游流水线收敛为单卡可跑的 BERT 路径，覆盖偏见量化与 SHAP 分析脚本；
复现出通用推文 18 例、核能推文 2 例 BERT 偏见实例，计数与论文报告一致。

`Python` `PyTorch` `Transformers` `SHAP` → [仓库](https://github.com/Samdy-L/SA-Reproducing-the-experiment)

### 动态社区发现与社区级虚假信息检测

在 CoDÆN 动态社区检测基准框架下，横向评估 GMA / αGMA / sGMA / NeGMA 四种算法
（覆盖 9 种社区演化变换）；NeGMA 在**社区分裂**场景 Modularity 0.5118，为四者最高。
该基准对比属课程课题，代码未开源。

另自研约 870 行社区级检测链路（8 维社区特征 + 逻辑回归 + 规则融合决策），已开源：

> 该链路数据为 ER 随机图模拟生成，社区系随机划分、标签与图结构相互独立，
> 该设定下指标不具参考意义——局限已在仓库 README 中逐条说明。

`Python` `NetworkX` `scikit-learn` `Matplotlib` → [仓库](https://github.com/Samdy-L/NeGMA-)

### CarePal 康伴 —— 帕金森病智能康复伴侣

uni-app + Vue3 跨端前端工程（Varlet 组件库 / Vite 构建），以「单页多模块」结构承载
智能对话、服药日程、周报问卷、OCR 识别与跌倒监控五个模块；通过 Vite 开发代理转发
两套后端服务，并实现统一鉴权封装与语音交互双通道回退。

药品识别模块基于**豆包视觉模型**：多图 base64 拼装为多模态消息，以结构化 Prompt 约束
输出「专业分析 / 患者可读说明」双块结果与 JSON 用药字段；针对模型不按格式输出的情况，
实现标签解析失败后按中文标题切分、再退化为全文的**三级解析策略**。另参与
ASR → LLM → TTS 语音链路与 **RAG 检索**模块的实现。

跌倒检测以预训练 YOLO-Pose 提取骨骼关键点，训练 **ST-GCN** 时空图卷积网络完成二分类，
在 GMDCSA24 与 Le2i 上训练、UR-Fall 上做**跨数据集留出评估**，采用 8 折交叉验证。

`uni-app` `Vue3` `Varlet` `Vite` `Python` `FastAPI` `豆包视觉模型` `ST-GCN` → [仓库](https://github.com/Samdy-L/CarePal)

## 技术栈

Python · PyTorch · Transformers · scikit-learn · NetworkX · Node.js / Express
Vue3 / uni-app · Git · MySQL · LaTeX
