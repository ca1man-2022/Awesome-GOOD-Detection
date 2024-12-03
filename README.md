# Graph Out-Of-Distribution Detection

We collect and organize the approaches on the challenge of graph OOD, explain the difference between OOD detection and OOD generalization, and additionally present some insights that are intended to provide some key references for researchers in this emerging field.

1. We classify the existing methods for OOD detection into 4 categories: *Enhancement-based methods*, *Reconstruction-based methods*, *Propagation-based methods*, and *Classification-based methods*.


## Summary of GOOD detection methods

| Method         | Category  |                       Title                             |  Evaluation Metrics | Datasets   |Venue     | Paper Links  | Code Links  | 
| -------------- |-----------|-------------------------------------------------------- | ------------------- | -----------| -------- | ------------ | ----------- |
|GKDE            |Clas.      |Uncertainty Aware Semi-Supervised Learning on Graph Data |    AUROC, AUPR      |    Cora, Citeseer, Pubmed, Amazon-Photo, Amazon-Computer, Physics-CA   |  NeurIPS'20  |[GKDE](https://proceedings.neurips.cc/paper/2020/hash/968c9b4f09cbb7d7925f38aea3484111-Abstract.html)|   https://github.com/zxj32/uncertainty-GNN | 
|OpenWGL | Reco. | OpenWGL: Open-World Graph Learning| ACC., Macor F1 |Cora, Citeseer, DBLP|ICDM'20 | [OpenWGL](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9338284)| -|
|GPN | Prop. | Graph Posterior Network: Bayesian Predictive Uncertainty for Node Classification| ID-ACC., OOD-ACC., AUROC | CoraML, Amazon-Photos, OGBN-Arxiv |NeurIPS'21 |[GPN](https://proceedings.neurips.cc/paper_files/paper/2021/hash/95b431e51fc53692913da5263c214162-Abstract.html)| https://github.com/stadlmax/Graph-Posterior-Network |
|NGC  | Prop. | NGC: A Unified Framework for Learning with Open-World Noisy Data |ACC. | CIFAR-10, CIFAR-100, TinyImageNet, Places-365 |ICCV'21 | [NGC](https://openaccess.thecvf.com/content/ICCV2021/html/Wu_NGC_A_Unified_Framework_for_Learning_With_Open-World_Noisy_Data_ICCV_2021_paper.html)| -|
| S-BGCN-T-K|Clas. | Uncertainty-Aware Graph-Based Multimodal Remote Sensing Detection of Out-Of-Distribution Samples|  AUROC, AUPR    | 2018 IEEE GRSS Data Fusion Challenge dataset  |CIKM'21| [S-BGCN-T-K](https://ceur-ws.org/Vol-3052/short5.pdf) | -|
|OODGAT | Prop. |Learning on Graphs with Out-of-Distribution Nodes | ACC., AUROC, FPR@95, Macor F1  | Cora, Amazon-CS, Amazon-Photo, CS-CA, LastFMAsia, Wiki-CS |KDD'22|[OODGAT](https://dl.acm.org/doi/abs/10.1145/3534678.3539457) |https://github.com/SongYYYY/KDD22-OODGAT|
|LMN |Prop. |End-to-End Open-Set Semi-Supervised Node Classification with Out-of-Distribution Detection | ACC. |Cora, Citeseer,Pubmed, arVix |IJCAI'22 |[LMN](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=8482&context=sis_research)|-|
|GraphDE|Enha. |GraphDE: A Generative Framework for Debiased Learning and Out-of-Distribution Detection on Graphs| AUROC, AUPR, FPR@95 | Spurious-Motif, MNIST-75sp, Collab, DrugOOD |NeurIPS'22|[GraphDE](https://proceedings.neurips.cc/paper_files/paper/2022/hash/c34262c35aa5f8c1a091822cbb2020c2-Abstract-Conference.html)|https://github.com/Emiyalzn/GraphDE|
|OSSC|Reco.|A Dynamic Variational Framework for Open-World Node Classification in Structured Sequences|ACC., AUC, Macor F1| DBLP-5, DBLP-3, Reddit, Brain |ICDM'22|[OSSC](https://shiruipan.github.io/publication/icdm-22-zhang/icdm-22-zhang.pdf)|https://github.com/qinzhang11/OSSC|
|EL|Clas.|Well-Classified Examples are Underestimated in Classification with Deep Neural Networks| ACC. |  Proteins, NCI1|AAAI'22|[EL](https://arxiv.org/pdf/2110.06537)|https://github.com/lancopku/well-classified-examples-are-underestimated|
|AAGOD|Clas.| A Data-centric Framework to Endow Graph Neural Networks with Out-Of-Distribution Detection Ability|AUC, AUPR, FPR@95  | ENZYMES, PROTEIN, IMDBM, IMDBB, BZR, COX2, TOX21, SIDER, BBBP, BACE |KDD'23| [AAGOD](http://shichuan.org/doc/150.pdf) |https://github.com/BUPT-GAMMA/AAGOD |
|GNNSafe|Prop.|Energy-Based Out-of-Distribution Detection for Graph Neural Networks| ACC., AUROC, AUPR, FPR@95 | Twitch, Arxiv, Cora, Amazon, Coauthor |ICLR'23| [GNNSafe](https://arxiv.org/abs/2302.02914) | https://github.com/qitianwu/GraphOOD-GNNSafe |
|GOOD-D|Enha. | GOOD-D: On Unsupervised Graph Out-Of-Distribution Detection | AUC|ENZYMES, PROTEIN, IMDBM, IMDBB, BZR, COX2, TOX21, SIDER, BBBP, BACE | WSDM'23|[GOOD-D](https://dl.acm.org/doi/abs/10.1145/3539597.3570446)|https://github.com/yixinliu233/G-OOD-D|










|ML-GOOD|Prop.|ML-GOOD: Towards Multi-Label Graph Out-Of-Distribution Detection |ACC., AUROC, AUPR, FPR@95|OGB-Proteins, PPI, DBLP, PCG, HumLoc, EukLoc|ML-GOOD|-|-|
