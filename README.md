# 李嘉宇 · Li Jiayu

武汉大学 · 网络空间安全 · 本科在读（2023–2027）

关注大模型的可信与安全——偏见量化、公平性评估与虚假信息检测。

📧 2728288049@qq.com　·　📍 武汉

---

## 研究方向

- **大模型公平性与社会偏见量化** —— 情感分析模型中的群体偏见度量与归因分析
- **虚假信息与协同传播检测** —— 动态网络中的组织化传播群体识别

## 精选项目

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
智能对话、服药日程、周报问卷、OCR 识别与跌倒监控五个模块。
通过 Vite 开发代理转发两套后端服务，并实现统一鉴权封装与语音交互双通道回退。

`uni-app` `Vue3` `Varlet` `Vite` → [仓库](https://github.com/Samdy-L/CarePal)

## 其他

腾讯游戏引擎技术远程课题《天命：AI 君主模拟器》—— 参与 Multi-Agent 系统设计与
Agent 层开发，系统落地 9 个 Agent（其中六部由独立 JSON 配置驱动）、11 项世界指标
与 22 个后端接口。

## 技术栈

Python · PyTorch · Transformers · scikit-learn · NetworkX · Node.js / Express
Vue3 / uni-app · Git · MySQL · LaTeX
