---
title: Generative design of programmable asymmetric β-barrel nanopores
title_zh: 可编程非对称β-桶纳米孔的生成式设计
authors: "Philomin, A., Sonigra, R., Majumder, S., Lin, H.-J., Li, Y., Xue, F., Kibler, R. D., Baldus, C., Trapido, E., Medeiros, A., Coventry, B., Bera, A., Kang, A., Mendoza, J., Kumar, M., Yang, Y., Baker, D."
date: 2026-07-15
pdf: "https://www.biorxiv.org/content/10.64898/2026.06.04.729630v2.full.pdf"
tags: ["query:aimat-mlpot"]
score: 6.0
evidence: 生成式AI框架设计跨膜β-桶纳米孔
tldr: 蛋白质纳米孔在分子传感等领域至关重要，但设计功能性纳米孔极具挑战。现有方法依赖天然对称结构或手工设计，限制了可编程性。本文提出生成式AI框架，通过蒸馏集训练主链和序列设计模型，实现了非对称β-桶纳米孔的自动化设计。实验表征48种设计，直径0.7-1.5nm，晶体结构验证准确性。该方法可按需定制离子传感、DNA易位等功能，拓展了纳米孔的应用空间。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-04-729630-v2/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1661, \"height\": 1826, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-04-729630-v2/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1642, \"height\": 2228, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-04-729630-v2/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1686, \"height\": 1118, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-04-729630-v2/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1684, \"height\": 1826, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-06-04-729630-v2/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1700, \"height\": 1230, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-06-04-729630-v2/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1550, \"height\": 724, \"label\": \"Table\"}]"
motivation: 现有纳米孔设计局限于对称结构或手工操作，难以实现可编程功能，亟需自动化设计方法。
method: 提出生成式AI框架，基于蒸馏集训练主链和序列设计模型，自动生成非对称β-桶纳米孔。
result: 48种设计直径0.7-1.5nm，晶体结构与模型高度匹配，实现离子传感和DNA易位功能。
conclusion: 该AI方法实现了纳米孔的可编程设计，为分子传感和膜输送提供新工具。
---

## 摘要
蛋白质纳米孔是分子传感、测序和分离的强大工具，但设计具有可编程功能的孔洞仍具挑战性。天然的同源寡聚跨膜β-桶（TMBs）被用于这些应用，但其均匀的管腔限制了空间分辨率和分析物区分能力。尽管基于能量的方法可以设计单体TMBs，但这些方法仍然高度依赖人工操作，且仅限于结构设计而非功能设计。在此，我们提出了一种用于TMB设计的生成式AI框架，其骨架和序列设计模型基于精心策划的蒸馏集进行训练。我们表征了48种设计，直径范围为0.7-1.5 nm，具有多样化的管腔化学性质和疏水厚度。晶体结构与设计模型高度吻合。我们证明，我们的方法可产生可定制的纳米孔，用于离子传感、DNA易位以及跨聚合物膜的运输。

## Abstract
Protein nanopores are powerful tools for molecular sensing, sequencing, and separation, but designing pores with programmable function remains challenging. Native homo-oligomeric transmembrane {beta} barrels (TMBs) are used for these applications, but their uniform lumens limit spatial resolution and analyte discrimination. Although monomeric TMBs can be designed using energy-based methods, these approaches remain highly manual and limited to structural design rather than function. Here, we present a generative AI framework for TMB design, with backbone and sequence design models trained on a curated distillation set. We characterized 48 designs spanning 0.7-1.5 nm in diameter, diverse lumen chemistries, and hydrophobic thicknesses. Crystal structures closely match the design models. We demonstrate that our method produces customizable nanopores for ion sensing, DNA translocation, and transport across polymer membranes.