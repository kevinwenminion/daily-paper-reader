---
title: "UniFlow: Unifying protein conformational ensemble generation and machine-learned force fields with a scalable normalizing Flow"
title_zh: "UniFlow: 统一蛋白质构象系综生成与机器学习力场通过可扩展的归一化流"
authors: "Liu, Y., Chen, M., Lin, G."
date: 2026-07-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.17.739266v1.full.pdf"
tags: ["query:aimat-mlpot"]
score: 7.0
evidence: 机器学习粗粒化力场用于蛋白质分子动力学
tldr: 分子动力学模拟计算成本高，现有生成式模型和机器学习力场虽能加速采样但通常各自独立发展。UniFlow首次将蛋白质构象系综生成与粗粒化力场统一在归一化流框架内，支持高效独立同分布采样、精确似然计算及可微能量力计算。在多种蛋白质上生成的系综接近参考MD，且可泛化至未见蛋白质，采样速度显著快于扩散模型。该统一模型还能进行稳定的长时域MD模拟，架起了生成式系综建模与物理模拟之间的桥梁。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739266-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1395, \"height\": 623, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-17-739266-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1463, \"height\": 473, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-17-739266-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1398, \"height\": 351, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-17-739266-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1345, \"height\": 565, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-17-739266-v1/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1370, \"height\": 242, \"label\": \"Table\"}]"
motivation: 分子动力学模拟计算成本高，而现有的生成式系综模型与机器学习力场各自独立发展，未能统一建模同一平衡分布。
method: 提出UniFlow，基于内坐标归一化流实现蛋白质构象生成与可微能量力计算，支持高效i.i.d.采样与精确似然评估。
result: 在多个蛋白质系统上生成的系综与参考MD高度吻合，并泛化到训练集外蛋白，采样速度远超扩散模型基线。
conclusion: UniFlow首次统一了生成式系综建模与机器学习力场，为桥接物理模拟与生成模型开辟了新路径。
---

## 摘要
分子动力学（MD）提供了建模平衡蛋白质构象能量景观的基本方法，但其计算成本限制了对长时间尺度和更大蛋白质系统的访问。近年来，生成式蛋白质系综模型和机器学习粗粒化力场作为加速构象采样的补充方法出现。然而，它们通常是分别开发的，尽管建模的是相同的平衡分布。我们引入UniFlow，第一个可扩展的生成模型，在单一框架内统一了蛋白质系综生成和用于分子动力学模拟的机器学习粗粒化力场。UniFlow采用内坐标归一化流，支持高效的独立同分布采样、精确的似然评估以及可微的能量和力计算。在多种蛋白质系统中，UniFlow生成的系综与参考MD模拟高度匹配，能够泛化到训练数据集之外的蛋白质，并且采样速度显著快于基于扩散的系综生成基线。相同的学习密度还可实现稳定的长时间尺度分子动力学模拟。总之，UniFlow为连接生成式系综建模与基于物理的分子模拟的统一模型类别铺平了道路。

## Abstract
Molecular dynamics (MD) provides a principled method for modeling equilibrium protein conformational energy landscapes, but its computational cost limits access to long timescales and larger protein systems. Recently, generative protein ensemble models and machine-learned coarse-grained force fields have emerged as complementary approaches for accelerating conformational sampling. However, they are typically developed separately despite modeling the same underlying equilibrium distribution. We introduce UniFlow, the first scalable generative model that unifies protein ensemble generation and machine-learned coarse-grained force fields for molecular dynamics simulation within a single framework. UniFlow employs an internal-coordinate normalizing flow that supports efficient i.i.d. sampling, exact likelihood evaluation, and differentiable energy and force computation. Across diverse protein systems, UniFlow generates ensembles that closely match reference MD simulations, generalizes to proteins beyond its training dataset, and samples substantially faster than diffusion-based ensemble-generation baselines. The same learned density further enables stable long-timescale molecular dynamics simulations. Together, UniFlow paves the way for a unified class of models that bridges generative ensemble modeling with physics-based molecular simulation.