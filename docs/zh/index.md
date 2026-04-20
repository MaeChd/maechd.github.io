# 昌 达（Da Chang）

**鹏城实验室** (*2025.7-至今*)

**中国科学院深圳先进技术研究院** (*2024.9-至今*)

模式识别与智能系统 (PRIS) 博士

**中南大学**自动化学院2020级

智能科学与技术 工学学士

**深度学习研究 — 优化 • 预训练基础设施 • 参数高效微调**

![Da Chang](../img/me_v2.jpg){ .avatar-left }

我2024年毕业于<a href="https://www.csu.edu.cn/">中南大学</a><a href="https://soa.csu.edu.cn/">自动化学院</a>智能科学与技术专业。  
目前在中国科学院深圳先进技术研究院（<a href="https://www.siat.ac.cn/">SIAT</a>）与鹏城实验室（<a href="https://www.pcl.ac.cn/">PCL</a>）联合培养攻读博士学位。  
我的专业方向为模式识别与智能系统，研究兴趣主要聚焦于**深度学习的优化与泛化**，以及深度模型在各类应用场景中的实践。  
我对**深度学习的理论与应用**都非常感兴趣，欢迎与我交流神经网络训练技巧、应用场景与优化理论。

- 📄 **[简历（PDF）](../pdf/cv_zh.pdf)**
- 🧪 **[GitHub](https://github.com/MaeChd)**
- 🎓 **[学术主页](https://scholar.google.com/citations?user=glTBszIAAAAJ&hl=zh-CN)**
- ✉️ **changda24@mails.ucas.ac.cn**


---

## 动态 / News {#news}
- **2026-03*** — 预印本 *MuonEq: Balancing Before Orthogonalization with Lightweight Equilibration* 发布。
- **2026-01** — *KG-SAM: Injecting Anatomical Knowledge into Segment Anything Models via Conditional Random Fields* 入选 **ICASSP 2026 Oral**。
- **2025-11** — *Calibrating and Rotating: A Unified Framework for Weight Conditioning in PEFT* 入选 **AAAI 2026**。 
- **2025-09** — 预印本 *On the Convergence of Muon and Beyond* 发布。  
- **2025-09** — *MGUP: A Momentum-Gradient Alignment Update Policy for Stochastic Optimization* 入选 **NeurIPS 2025 Spotlight**。
- **2025-07** — 我开始了博士第二年在鹏城实验室的学习。
- **2024-09** — 我开启了博士第一年在中国科学院大学雁栖湖校区的学习。  
- **2024-08** — 本科毕业设计*Mixed Text Recognition with Efficient Parameter Fine-Tuning and Transformer* 入选 **ICONIP 2024**。
- **2024-06** — 我从中南大学自动化学院毕业.
- **2024-06** — 我的本科毕业论文获得优秀论文评价。
---

## 项目经验
<div class="pub-list">

<div class="pub-item">
  <strong>Distributed Muon-based MoE Training on 64 NPUs</strong>
  <div class="authors">
    <span class="author-me">Da Chang</span>
  </div>
  <div>
    <span class="meta">Project · Systems for LLM Training</span>
  </div>
  <span class="meta">
    <span class="text-blue"><i>Megatron & MindSpeed</i></span> ·
    <span class="text-yellow"><i>MoE / Distributed Training</i></span>
  </span>
  <div>
    在基于 Megatron 和 MindSpeed 的 64 卡 NPU MoE 大模型训练框架上，完成了 Muon 与 Distributed Muon（ZeRO 风格）的集成与训练落地，并支持 TP、CP、EP、PP 等并行策略。通过对优化器与训练系统的联合调优，Muon 在训练中稳定优于 AdamW，Distributed Muon 则以额外通信开销换取了更低显存占用；同时定位了 MoE expert 与 Muon 冗余引发的损失尖峰故障。项目最终提升了训练吞吐、稳定性与资源利用率，并支持更大规模模型训练。
  </div>
  <div class="chips">
    <span class="chip">MoE</span><span class="chip">Muon</span><span class="chip">ZeRO</span><span class="chip">Megatron</span><span class="chip">MindSpeed</span><span class="chip">64 NPUs</span>
  </div>
</div>

</div>
## 代表论文

<div class="pub-list">

<div class="pub-item">
  <strong>MuonEq: Balancing Before Orthogonalization with Lightweight Equilibration</strong>
  <div class="authors">
    <span class="author-me">Da Chang</span>, Qiankun Shi, Lvgang Zhang, Yu Li, Ruijie Zhang, Yao Lu, Yongxiang Liu, Ganzhao Yuan
  </div>
  <span class="meta">
    Preprint 2026.3 ·
    <a href="https://arxiv.org/pdf/2603.28254" target="_blank" rel="noopener">PDF</a> ·
    <a href="https://github.com/MaeChd/muon-eq" target="_blank" rel="noopener">Code</a>
  </span>
  <div class="summary">
    MuonEq 在 Muon 的正交化更新之前加入轻量级的行/列平衡改善有限步 Newton–Schulz 的输入矩阵几何。
  </div>
  <div class="chips">
    <span class="chip">Muon</span>
    <span class="chip">Row/Col Equilibration</span>
    <span class="chip">Stochastic Optimization</span>
  </div>
</div>

<div class="pub-item">
  <strong>KG-SAM: Injecting Anatomical Knowledge into Segment Anything Models via Conditional Random Fields</strong>
  <div class="authors">
    Yu Li*, <span class="author-me">Da Chang*</span>, Xi Xiao
  </div>
  <span class="meta">(*: Equal contribution)</span>
  <span class="meta">
    <span class="text-blue"><i>ICASSP 2026 Oral</i></span> ·
    <span class="text-yellow"><i>CCF B</i></span> ·
    <a href="https://arxiv.org/abs/2509.21750" target="_blank" rel="noopener">PDF</a>
  </span>
  <div class="summary">
    提出了一个知识引导的医学图像分割框架，该框架集成了用于解剖先验的医学知识图谱、用于边界细化的基于能量的CRF和基于不确定性感知的融合模块，在多位点前列腺分割中取得了82.69%的Dice分割效果。
  </div>
  <div class="chips">
    <span class="chip">SAM</span>
    <span class="chip">Medical Segmentation</span>
    <span class="chip">Knowledge Graph</span>
    <span class="chip">CRF</span>
  </div>
</div>

<div class="pub-item">
  <strong>On the Convergence of Muon and Beyond</strong>
  <div class="authors">
    <span class="author-me">Da Chang</span>, Yongxiang Liu, Ganzhao Yuan
  </div>
  <span class="meta">
    Preprint 2025.9 ·
    <a href="https://arxiv.org/pdf/2509.15816" target="_blank" rel="noopener">PDF</a> ·
    <a href="https://github.com/MaeChd/MUON-MVR" target="_blank" rel="noopener">Code</a>
  </span>
  <div class="summary">
    提供了统一的衰减步长分析框架，完整地分析Muon-type优化器在随机非凸优化设置下的非遍历收敛性质与遍历收敛性质；讨论方差缩减带来的最优复杂度性质。
  </div>
  <div class="chips">
    <span class="chip">Muon</span>
    <span class="chip">Convergence</span>
    <span class="chip">Stochastic Optimization</span>
  </div>
</div>

<div class="pub-item">
  <strong>Calibrating and Rotating: A Unified Framework for Weight Conditioning in PEFT</strong>
  <div class="authors">
    <span class="author-me">Da Chang</span>, Peng Xue, Yu Li, Yongxiang Liu, Pengxiang Xu, Shixun Zhang
  </div>
  <span class="meta">
    <span class="text-blue"><i>AAAI 2026</i></span> ·
    <span class="text-red"><i>CCF A</i></span> ·
    <a href="https://arxiv.org/pdf/2511.00051" target="_blank" rel="noopener">PDF</a> ·
    <a href="https://github.com/MaeChd/SORA" target="_blank" rel="noopener">Code</a>
  </span>
  <div class="summary">
    分析DoRA与LoRA的性质，并统一“校准 + 旋转”的权重条件化策略，提升 PEFT 的性能与训练推理效率。
  </div>
  <div class="chips">
    <span class="chip">LLMs PEFT</span>
    <span class="chip">Weight Conditioning</span>
  </div>
</div>

<div class="pub-item">
  <strong>MGUP: A Momentum-Gradient Alignment Update Policy for Stochastic Optimization</strong>
  <div class="authors">
    <span class="author-me">Da Chang</span>, Ganzhao Yuan
  </div>
  <span class="meta">
    <span class="text-blue"><i>NeurIPS 2025</i></span> ·
    <span class="text-red"><i>Spotlight (Top 3%)</i></span> ·
    <span class="text-red"><i>CCF A</i></span> ·
    <a href="https://openreview.net/pdf?id=TDFSKAspoQ" target="_blank" rel="noopener">PDF</a> ·
    <a href="https://github.com/MaeChd/MGUP" target="_blank" rel="noopener">Code</a>
  </span>
  <div class="summary">
    通过动量-梯度的对齐策略提供随机非凸优化遍历收敛性保证并加速训练
  </div>
  <div class="chips">
    <span class="chip">Stochastic Optimization</span>
    <span class="chip">Momentum</span>
    <span class="chip">Alignment</span>
  </div>
</div>

<div class="pub-item">
  <strong>Mixed Text Recognition with Efficient Parameter Fine-Tuning and Transformer</strong>
  <div class="authors">
    <span class="author-me">Da Chang*</span>, Yu Li*
  </div>
  <span class="meta">(*: Equal contribution)</span>
  <span class="meta">
    <strong>Undergraduate Graduation Project</strong> /
    <span class="text-blue"><i>ICONIP 2024</i></span> ·
    <span class="text-green"><i>CCF C</i></span> ·
    <a href="https://arxiv.org/pdf/2404.12734" target="_blank" rel="noopener">PDF</a> ·
    <a href="https://github.com/MaeChd/DLoRA-TrOCR" target="_blank" rel="noopener">Code</a>
  </span>
  <div class="summary">
    基于 TrOCR 的 OCR 管线，结合高效 PEFT 以处理混合文本；提供可复现实验与评测。
  </div>
  <div class="chips">
    <span class="chip">OCR</span>
    <span class="chip">TrOCR</span>
    <span class="chip">PEFT</span>
  </div>
</div>

</div>

---
## 学术服务
*TPAMI'25*, *ICML'26*, *NeurIPS'26*审稿人。

---

## 荣誉与奖励

- 第八届全国大学生生物医学工程创新设计竞赛 **二等奖**，2023  
- 第九届全国大学生统计建模竞赛 **三等奖**，2023  
- **中南大学二等优秀奖学金（前 15%）**，2023  
- **“山河智能奖学金”二等奖学金（前 5%）**，2022  
- **中南大学一等奖学金（前 5%）**，2022

---

## 技能

- **编程语言:** Python, C/C++, MATLAB, LaTeX
- **机器学习框架:** PyTorch, scikit-learn, Megatron, MindSpeed
- **分布式训练:** TP, PP, EP, CP; MoE training on NPU clusters
- **AI助手编程:** Claude Code, Codex

---

## 访客

<!-- <div id="visit-map"></div> -->
<!-- <a href="https://mapmyvisitors.com/web/1c0fh"  title="Visit tracker"><img src="https://mapmyvisitors.com/map.png?d=GJ-YeVhSXGG7UloYgc5FBWrsxNV1Nq0n-gAWy_7wmvU&cl=ffffff" /></a> -->
<figure class="vis-center">
  <a href="https://mapmyvisitors.com/web/1c0fh" title="Visit tracker">
    <img src="https://mapmyvisitors.com/map.png?d=GJ-YeVhSXGG7UloYgc5FBWrsxNV1Nq0n-gAWy_7wmvU&cl=ffffff" alt="Visitors map">
  </a>
  <figcaption style="opacity:.75; font-size:.9em; margin-top:.25rem;">
    Visitors map (powered by mapmyvisitors.com)
  </figcaption>
</figure>
