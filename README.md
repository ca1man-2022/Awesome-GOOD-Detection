# Graph Out-of-Distribution Detection (GOOD-D) 

This repository provides a **comprehensive and structured catalogue** of existing
Graph Out-of-Distribution (GOOD) detection methods.

⭐The paper is available on arXiv: [Out-of-Distribution Detection on Graphs: A Survey](https://arxiv.org/pdf/2502.08105).

## Abstract
Graph machine learning has witnessed rapid growth, driving advancements across diverse domains. However, the in-distribution assumption, where training and testing data share the same distribution, often breaks in real-world scenarios, leading to degraded model performance under distribution shifts. This challenge has catalyzed interest in graph out-of-distribution (GOOD) detection, which focuses on identifying graph data that deviates from the distribution seen during training, thereby enhancing model robustness. In this paper, we provide a rigorous definition of GOOD detection and systematically categorize existing methods into four types: enhancement-based, reconstruction-based, information propagation-based, and classification-based approaches. We analyze the principles and mechanisms of each approach and clarify the distinctions between GOOD detection and related fields, such as graph anomaly detection, outlier detection, and GOOD generalization. Beyond methodology, we discuss practical applications and theoretical foundations, highlighting the unique challenges posed by graph data. Finally, we discuss the primary challenges and propose future directions to advance this emerging field. 

---

## Taxonomy

We categorize GOOD detection methods into four classes:

- **Enhancement-based**  
- **Reconstruction-based**  
- **Information Propagation-based**  
- **Classification-based**

---

## Enhancement-based Methods 

| # | Method | Title | Metrics | Datasets | Venue | Paper | Code | Keywords | Task |
|---|--------|-------|---------|----------|-------|-------|------|----------|------|
| 1 | GraphDE | GraphDE: A Generative Framework for Debiased Learning and OOD Detection on Graphs | AUROC, AUPR, FPR@95 | Spurious-Motif, MNIST-75sp, DrugOOD | NeurIPS’22 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/c34262c35aa5f8c1a091822cbb2020c2-Abstract-Conference.html) | https://github.com/Emiyalzn/GraphDE | Generative Model | Graph |
|2 | GOOD-D | On Unsupervised Graph Out-of-Distribution Detection | AUC | Molecule datasets | WSDM’23 | [Paper](https://dl.acm.org/doi/abs/10.1145/3539597.3570446) | https://github.com/yixinliu233/G-OOD-D | Contrastive Learning | Graph |
|3 | GPN-CE-GD | Improvements on Uncertainty Quantification via Distance Regularization | AUROC, AUPR | CoraML, Citeseer, PubMed | NeurIPS’23 | [Paper](https://arxiv.org/abs/2311.05795) | https://github.com/neoques/Graph-Posterior-Network | Bayesian Posterior | Node |
|4 | SGOOD | Substructure-enhanced Graph-level OOD Detection | AUROC, AUPR, FPR@95 | ENZYMES, IMDB, DrugOOD | CIKM’24 | [Paper](https://dl.acm.org/doi/abs/10.1145/3627673.3679710) | https://github.com/TommyDzh/SGOOD | Self-supervised | Graph |
|5 | GOODAT | Towards Test-time Graph OOD Detection | AUC | Molecule datasets | AAAI’24 | [Paper](https://arxiv.org/abs/2401.06176) | – | Information Bottleneck | Graph |
|6 | HGOE | Hybrid External & Internal Graph Outlier Exposure | AUC | Molecule datasets | MM’24 | [Paper](https://dl.acm.org/doi/abs/10.1145/3664647.3681118) | – | Outlier Exposure | Graph |
|7 | SMUG | Sand Mixing for Unobserved Class Detection | AUROC | Cora, DBLP, Amazon | WWW’24 | [Paper](https://dl.acm.org/doi/abs/10.1145/3589334.3645466) | – | Few-shot Learning | Node |
|8| GOLD | Implicit Adversarial Latent Generation for GOOD | AUROC, FPR@95 | Twitch, Cora, Amazon | ICLR’25 | [Paper](https://openreview.net/pdf?id=y5einmJ0Yx) | https://github.com/DannyW618/GOLD | Generative Model | Node |
|9| DeGEM | Decoupled Graph Energy-based Model | AUROC, FPR@95 | Heterophilic graphs | ICLR’25 | [Paper](https://openreview.net/pdf?id=NuVBI4wPMm) | – | Energy-based | Node |

---

## Reconstruction-based Methods 

| # | Method | Title | Metrics | Datasets | Venue | Paper | Code | Keywords | Task |
|---|--------|-------|---------|----------|-------|-------|------|----------|------|
| 1 | OpenWGL | OpenWGL: Open-World Graph Learning | ACC, Macro-F1 | Cora, Citeseer, DBLP | ICDM’20 | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9338284) | – | Graph Autoencoder | Node |
| 2 | OSSC | Dynamic Variational Framework for Open-World Node Classification | ACC, AUC | DBLP, Reddit | ICDM’22 | [Paper](https://shiruipan.github.io/publication/icdm-22-zhang/icdm-22-zhang.pdf) | https://github.com/qinzhang11/OSSC | Graph Autoencoder | Node |
|3 | PGR-MOOD | Optimizing OOD Detection in Molecular Graphs with Diffusion | AUROC, AUPR | DrugOOD, GOOD-HIV | KDD’24 | [Paper](https://arxiv.org/abs/2404.15625) | https://github.com/se7esx/PGR-MOOD | Diffusion Model | Graph |

---

## Information Propagation-based Methods 

| # | Method | Title | Metrics | Datasets | Venue | Paper | Code | Keywords | Task |
|---|--------|-------|---------|----------|-------|-------|------|----------|------|
|1  | GPN | Graph Posterior Network | AUROC | CoraML, ogbn-arxiv | NeurIPS’21 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2021/hash/95b431e51fc53692913da5263c214162-Abstract.html) | https://github.com/stadlmax/Graph-Posterior-Network | Bayesian | Node |
| 2 | OODGAT | Learning on Graphs with OOD Nodes | AUROC | Cora, Amazon | KDD’22 | [Paper](https://dl.acm.org/doi/abs/10.1145/3534678.3539457) | https://github.com/SongYYYY/KDD22-OODGAT | Semi-supervised | Node |
|3  | GNNSafe | Energy-Based OOD Detection for GNNs | AUROC, FPR@95 | Twitch, Arxiv | ICLR’23 | [Paper](https://arxiv.org/abs/2302.02914) | https://github.com/qitianwu/GraphOOD-GNNSafe | Energy | Node |
|4  | GERDQ | Calibrate GNNs via Deep Q-learning | ACC, ECE | Cora, Amazon | CIKM’23 | [Paper](https://dl.acm.org/doi/pdf/10.1145/3583780.3614797) | https://github.com/DamoSWL/Calibration-of-GNN-with-OOD-nodes | Q-learning | Node |
|5  | TopoOOD | Neighborhood Shaping for GOOD | AUROC | Cora, Amazon | ICML’24 | [Paper](https://openreview.net/forum?id=pmcusTywXO) | – | Dirichlet Energy | Node |
|6  | NODESAFE | Bounded Energy-based GOOD | AUROC | Twitch, Arxiv | ICML’24 | [Paper](https://openreview.net/forum?id=mjh7AOWozN) | https://github.com/ShenzhiYang2000/NODESAFE | Energy | Node |
|7  | GNSD | Graph Neural Stochastic Diffusion | AUROC | Cora, Pubmed | ICML’24 | [Paper](https://openreview.net/pdf?id=xJUhgvM2u8) | – | Diffusion | Node |
|8  | EnergyDef | Category-free Energy OOD Detection | AUROC | Yelp, Amazon | KDD’24 | [Paper](https://dl.acm.org/doi/abs/10.1145/3637528.3671939) | https://github.com/KellyGong/EnergyDef | Energy | Node |
|9  | ML-GOOD | Multi-label GOOD Detection | AUROC | OGB-Proteins, PPI | AAAI’25 | – | https://github.com/ca1man-2022/ML-GOOD | Energy | Node |
|10 | GRASP | Revisiting Score Propagation in GOOD | AUROC | ogbn-products, Arxiv | NeurIPS’24 | [Paper](https://openreview.net/forum?id=jb5qN3212b) | https://github.com/longfei-ma/GRASP | Score Propagation | Node |
|11 | EDBD | Spreading GOOD on Graphs | AUROC | Cora, Amazon | ICLR’25 | [Paper](https://openreview.net/pdf?id=p1TBYyqy8v) | – | Energy Diffusion | Node |

---

## Classification-based Methods 

| # | Method | Title | Metrics | Datasets | Venue | Paper | Code | Keywords | Task |
|---|--------|-------|---------|----------|-------|-------|------|----------|------|
| 1 | GKDE | Uncertainty Aware Semi-Supervised Learning | AUROC, AUPR | Cora, Pubmed | NeurIPS’20 | [Paper](https://proceedings.neurips.cc/paper/2020/hash/968c9b4f09cbb7d7925f38aea3484111-Abstract.html) | https://github.com/zxj32/uncertainty-GNN | Dirichlet | Node |
| 2 | S-BGCN-T-K | Uncertainty-Aware Multimodal OOD Detection | AUROC | Remote Sensing | CIKM’21 | [Paper](https://ceur-ws.org/Vol-3052/short5.pdf) | – | Knowledge Distillation | Node |
|3  | EL | Well-Classified Examples are Underestimated | ACC | Proteins, NCI1 | AAAI’22 | [Paper](https://arxiv.org/pdf/2110.06537) | https://github.com/lancopku/well-classified-examples-are-underestimated | Self-supervised | Node/Graph |
|4  | AAGOD | Data-centric GOOD Framework | AUROC | Molecule datasets | KDD’23 | [Paper](http://shichuan.org/doc/150.pdf) | https://github.com/BUPT-GAMMA/AAGOD | Self-supervised | Graph |
|5  | Relation | Neural Relation Graph | AP, TNR95 | ImageNet, SUN | NeurIPS’23 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/886ed40d7882c9f891824e42a452c228-Abstract-Conference.html) | https://github.com/snu-mllab/Neural-Relation-Graph | Semi-supervised | Graph |
|6  | UGNN | Universal Graph Classification | ACC | COIL, CIFAR | TKDE’23 | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10138449) | – | Open-set | Graph |

---


🚩
We will keep this repository updated. If we have missed any relevant work, please feel free to contact us by email tingyicai@zjnu.edu.cn.

Last updated on Jan. 2025.

## Citation

If you find this repository useful, please consider citing it:

```bibtex
@article{cai2025good-d,
  title   = {Out-of-Distribution Detection on Graphs: A Survey},
  author  = {Tingyi Cai and Yunliang Jiang and Yixin Liu and Ming Li and Changqin Huang and Shirui Pan},
  journal = {arXiv preprint arXiv:2502.08105},
  year    = {2025}
}
