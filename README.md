# Graph Out-Of-Distribution Detection

We classify the existing methods for GOOD detection into 4 categories: **Enhancement-based methods**, **Reconstruction-based methods**, **Propagation-based methods**, and **Classification-based methods**.

## Summary of GOOD detection methods

|  | Method         | Category  |                       Title                             |  Evaluation Metrics | Datasets   |Venue     | Paper Links  | Code Links  | 
|--| -------------- |-----------|-------------------------------------------------------- | ------------------- | -----------| -------- | ------------ | ----------- |
|1|GKDE            |Clas.      |Uncertainty Aware Semi-Supervised Learning on Graph Data |    AUROC, AUPR      |    Cora, Citeseer, Pubmed, Amazon-Photo, Amazon-Computer, Physics-CA   |  NeurIPS'20  |[GKDE](https://proceedings.neurips.cc/paper/2020/hash/968c9b4f09cbb7d7925f38aea3484111-Abstract.html)|   https://github.com/zxj32/uncertainty-GNN | 
|2|OpenWGL | Reco. | OpenWGL: Open-World Graph Learning| ACC., Macor F1 |Cora, Citeseer, DBLP|ICDM'20 | [OpenWGL](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9338284)| -|
|3|GPN | Prop. | Graph Posterior Network: Bayesian Predictive Uncertainty for Node Classification| ID-ACC., OOD-ACC., AUROC | CoraML, Amazon-Photos, OGBN-Arxiv |NeurIPS'21 |[GPN](https://proceedings.neurips.cc/paper_files/paper/2021/hash/95b431e51fc53692913da5263c214162-Abstract.html)| https://github.com/stadlmax/Graph-Posterior-Network |
|4|NGC  | Prop. | NGC: A Unified Framework for Learning with Open-World Noisy Data |ACC. | CIFAR-10, CIFAR-100, TinyImageNet, Places-365 |ICCV'21 | [NGC](https://openaccess.thecvf.com/content/ICCV2021/html/Wu_NGC_A_Unified_Framework_for_Learning_With_Open-World_Noisy_Data_ICCV_2021_paper.html)| -|
|5| S-BGCN-T-K|Clas. | Uncertainty-Aware Graph-Based Multimodal Remote Sensing Detection of Out-Of-Distribution Samples|  AUROC, AUPR    | 2018 IEEE GRSS Data Fusion Challenge dataset  |CIKM'21| [S-BGCN-T-K](https://ceur-ws.org/Vol-3052/short5.pdf) | -|
|6|OODGAT | Prop. |Learning on Graphs with Out-of-Distribution Nodes | ACC., AUROC, FPR@95, Macor F1  | Cora, Amazon-CS, Amazon-Photo, CS-CA, LastFMAsia, Wiki-CS |KDD'22|[OODGAT](https://dl.acm.org/doi/abs/10.1145/3534678.3539457) |https://github.com/SongYYYY/KDD22-OODGAT|
|7|LMN |Prop. |End-to-End Open-Set Semi-Supervised Node Classification with Out-of-Distribution Detection | ACC. |Cora, Citeseer,Pubmed, arVix |IJCAI'22 |[LMN](https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=8482&context=sis_research)|-|
|8|GraphDE|Enha. |GraphDE: A Generative Framework for Debiased Learning and Out-of-Distribution Detection on Graphs| AUROC, AUPR, FPR@95 | Spurious-Motif, MNIST-75sp, Collab, DrugOOD |NeurIPS'22|[GraphDE](https://proceedings.neurips.cc/paper_files/paper/2022/hash/c34262c35aa5f8c1a091822cbb2020c2-Abstract-Conference.html)|https://github.com/Emiyalzn/GraphDE|
|9|OSSC|Reco.|A Dynamic Variational Framework for Open-World Node Classification in Structured Sequences|ACC., AUC, Macor F1| DBLP-5, DBLP-3, Reddit, Brain |ICDM'22|[OSSC](https://shiruipan.github.io/publication/icdm-22-zhang/icdm-22-zhang.pdf)|https://github.com/qinzhang11/OSSC|
|10|EL|Clas.|Well-Classified Examples are Underestimated in Classification with Deep Neural Networks| ACC. |  Proteins, NCI1|AAAI'22|[EL](https://arxiv.org/pdf/2110.06537)|https://github.com/lancopku/well-classified-examples-are-underestimated|
|11|AAGOD|Clas.| A Data-centric Framework to Endow Graph Neural Networks with Out-Of-Distribution Detection Ability|AUC, AUPR, FPR@95  | ENZYMES, PROTEIN, IMDBM, IMDBB, BZR, COX2, TOX21, SIDER, BBBP, BACE |KDD'23| [AAGOD](http://shichuan.org/doc/150.pdf) |https://github.com/BUPT-GAMMA/AAGOD |
|12|GNNSafe|Prop.|Energy-Based Out-of-Distribution Detection for Graph Neural Networks| ACC., AUROC, AUPR, FPR@95 | Twitch, Arxiv, Cora, Amazon, Coauthor |ICLR'23| [GNNSafe](https://arxiv.org/abs/2302.02914) | https://github.com/qitianwu/GraphOOD-GNNSafe |
|13|GOOD-D|Enha. | GOOD-D: On Unsupervised Graph Out-Of-Distribution Detection | AUC|BZR, PTC-MR, AIDS, ENZYMES, IMDB-M, Tox21, FreeSolv, BBBP, ClinTox, Esol, COX2, MUTAG, DHFR, PROTEIN, IMDB-B, SIDER, ToxCast, BACE, LIPO, MUV | WSDM'23|[GOOD-D](https://dl.acm.org/doi/abs/10.1145/3539597.3570446)|https://github.com/yixinliu233/G-OOD-D|
|14|Relation| Clas. |Neural Relation Graph: A Unified Framework for Identifying Label Noise and Outlier Data| AP, TNR95| ImageNet, Places, SUN, iNatualist, Textures |NeurIPS'23|[Relation](https://proceedings.neurips.cc/paper_files/paper/2023/hash/886ed40d7882c9f891824e42a452c228-Abstract-Conference.html) |https://github.com/snu-mllab/Neural-Relation-Graph |
|15|GPN-CE-GD|Enha. |Improvements on Uncertainty Quantification for Node Classification via Distance-Based Regularization| ID-ACC., AUROC, AUPR | CoralML, Citeseer, PubMed | NeurIPS'23 |[GPN-CE-GD](https://arxiv.org/abs/2311.05795)| https://github.com/neoques/Graph-Posterior-Network|
|16|Open-WRF|Prop.| Open-World Lifelong Graph Learning| ACC., AUROC  | Cora, Citeseer, Pubmed, OGB-arXiv, DBLP-easy, DBLP-hard | IJCNN'23| [Open-WRF](https://arxiv.org/pdf/2310.12565) |https://github.com/Bobowner/Open-World-LGL |
|17|UGNN|Clas.|Towards Semi-Supervised Universal Graph Classification |ACC.  | COIL-DEL, Letter-High, MNIST, CIFAR10, Reddit-Mutil-12k, Colors-3  |TKDE'23 |[UGNN](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10138449)|- |
|18|GERDQ|Prop.|Calibrate Graph Neural Networks under Out-of-Distribution Nodes via Deep Q-learning| ACC., ECE| Cora, Citeseer, Pubmed, Amazon-Photo, Amazon-Computer, Physics-CA |CIKM'23|[GERDQ](https://dl.acm.org/doi/pdf/10.1145/3583780.3614797)|https://github.com/DamoSWL/Calibration-of-GNN-with-OOD-nodes|
|19|SGOOD|Enha.|SGOOD: Substructure-enhanced Graph-Level Out-of-Distribution Detection| AUROC, AUPR, FPR@95| ENZYMES, IMDB-M, IMDB-B, Reddit-12k, BACE, BBBP, DrugOOD, HIV|CIKM'24|[SGOOD](https://dl.acm.org/doi/abs/10.1145/3627673.3679710)|https://github.com/TommyDzh/SGOOD|
|20|GOODAT|Enha.|GOODAT: Towards Test-time Graph Out-of-Distribution Detection| AUC | BZR, PTC-MR, AIDS, ENZYMES, IMDB-M, Tox21, FreeSolv, BBBP, ClinTox, Esol, COX2, MUTAG, DHFR, PROTEIN, IMDB-B, SIDER, ToxCast, BACE, LIPO, MUV  |AAAI'24|[GOODAT](https://arxiv.org/abs/2401.06176)|- |
|21|TopoOOD|Prop.|Graph Out-of-Distribution Detection Goes Neighborhood Shaping|ACC., AUROC, AUPR, FPR@95 | Twitch, Arxiv, Cora, Amazon, Coauthor | ICML'24|[TopoOOD](https://openreview.net/forum?id=pmcusTywXO)|-|
|22|NODESAFE|Prop.|Bounded and Uniform Energy-based Out-of-distribution Detection for Graphs|ACC., AUROC, AUPR, FPR@95 | Twitch, Arxiv, Cora, Amazon, Coauthor |ICML'24|[NODESAFE](https://openreview.net/forum?id=mjh7AOWozN)|https://github.com/ShenzhiYang2000/NODESAFE|
|23|GNSD|Prop.|Graph Neural Stochastic Diffusion for Estimating Uncertainty in Node Classification| ACC., AUROC, AUPR, FPR@95| Amazon-Computers, Cora, Citeseer, Pubmed, OGBN-Arxiv| ICML'24|[GNSD](https://openreview.net/pdf?id=xJUhgvM2u8)|-|
|24|PGR-MOOD|Reco.|Optimizing OOD Detection in Molecular Graphs: A Novel Approach with Diffusion Models |AUROC, AUPR, FPR@95 | GOOD-HIV, GOOD-PCBA, DrugOOD-IC50, DrugOOD-EC50|KDD'24|[PGR-MOOD](https://arxiv.org/abs/2404.15625)|https://github.com/se7esx/PGR-MOOD|
|25|EnergyDef|Prop.| An Energy-centric Framework for Category-free Out-of-distribution Node Detection in Graphs| | |KDD'24|[EnergyDef](https://dl.acm.org/doi/abs/10.1145/3637528.3671939)|-|
|26|HGOE|Enha.|HGOE: Hybrid External and Internal Graph Outlier Exposure for Graph Out-of-Distribution Detection| AUC |AIDS, DHFR, ENZYMES, PROTEIN, IMDB-M, IMDB-B, Tox21, SIDER, FreeSolv, ToxCast, BBBP, BACE, ClinTox, LIPO, Esol, MUV, BZR, COX2, PTC_MR, MUTAG |MM'24|[HGOE](https://dl.acm.org/doi/abs/10.1145/3664647.3681118)|-|
|27|HGIF|Enha.|Heterophilic Graph Invariant Learning for Out-of-Distribution of Fraud Detection| AUC, Macor F1 |YelpChi, Amazon, T-Finance, T-Social |MM'24|[HGIF](https://openreview.net/forum?id=JnG3wI5E5P)|https://github.com/Ling-Fei-Ren/HGIF|
|28|SMUG|Enha.|SMUG: Sand Mixing for Unobserved Class Detection in Graph Few-Shot Learning| AUROC |Cora, DBLP, Amazon-Clothing, Amazon-Electronics |WWW'24|[SMUG](https://dl.acm.org/doi/abs/10.1145/3589334.3645466)|-|
|29|ML-GOOD|Prop.|ML-GOOD: Towards Multi-Label Graph Out-Of-Distribution Detection |ACC., AUROC, AUPR, FPR@95|OGB-Proteins, PPI, DBLP, PCG, HumLoc, EukLoc|'25|ML-GOOD|https://github.com/ca1man-2022/ML-GOOD |
