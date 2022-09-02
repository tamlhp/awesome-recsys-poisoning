# Posion attacks against Recommender Systems
A repository of poison attacks against recommender systems, as well as their countermeasures.

Our systematic review **Manipulating Recommender Systems: A Survey of Poisoning Attacks and Countermeasures** is available on arxiv: [link](https://github.com/adamnguyenitvn/RS_posion_attacks)

Please cite our survey paper if this repository is helpful.

# Table of Contents

- [Poison Attacks](#Poison-Attacks)
   - [Model-agnostic](#Model-agnostic)
   - [Model-intrinsic](#Model-intrinsic)
- [Detection Methods](#Detection-Methods)
   - [Supervised](#Supervised)
   - [Semi Supervised](#Semi-Supervised)
   - [Unsupervised](#Unsupervised)
## Poison Attacks
### Model-agnostic
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| MA-1 | [Shyong K Lam and John Riedl. (2004). Shilling recommender systems for fun and profit. In Proceedings of the 13th
international conference on World Wide Web. 393–402.](https://dl.acm.org/doi/10.1145/988672.988726) | WWW | 2004 | [Python](#) |
| Pin-Sage | [Ying, R., He, R., Chen, K., Eksombatchai, P., Hamilton, W. L., & Leskovec, J. (2018, July). Graph convolutional neural networks for web-scale recommender systems. In Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining (pp. 974-983).](https://arxiv.org/pdf/1806.01973) | KDD | 2018 | [Python](https://paperswithcode.com/paper/graph-convolutional-neural-networks-for-web) |
| NGCF | [Wang, X., He, X., Wang, M., Feng, F., & Chua, T. S. (2019, July). Neural graph collaborative filtering. In _Proceedings of the 42nd international ACM SIGIR conference on Research and development in Information Retrieval_ (pp. 165-174).](https://arxiv.org/pdf/1905.08108.pdf) | SIGIR | 2019 | [Python](https://paperswithcode.com/paper/neural-graph-collaborative-filtering) |
| DGCF | [Wang, X., Jin, H., Zhang, A., He, X., Xu, T., & Chua, T. S. (2020, July). Disentangled graph collaborative filtering. In _Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 1001-1010).](https://arxiv.org/pdf/2007.01764) | SIGIR | 2020 | [Python](https://paperswithcode.com/paper/disentangled-graph-collaborative-filtering) |
| LightGCN | [He, X., Deng, K., Wang, X., Li, Y., Zhang, Y., & Wang, M. (2020, July). Lightgcn: Simplifying and powering graph convolution network for recommendation. In _Proceedings of the 43rd International ACM SIGIR conference on research and development in Information Retrieval_ (pp. 639-648).](https://arxiv.org/pdf/2002.02126.pdf) | SIGIR | 2020 | [Python](https://paperswithcode.com/paper/lightgcn-simplifying-and-powering-graph) |
| NIA-GCN | [Sun, J., Zhang, Y., Guo, W., Guo, H., Tang, R., He, X., ... & Coates, M. (2020, July). Neighbor interaction aware graph convolution networks for recommendation. In Proceedings of the 43rd International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 1289-1298).](https://dl.acm.org/doi/abs/10.1145/3397271.3401123) | SIGIR | 2020 | NA |
| SGL | [Wu, J., Wang, X., Feng, F., He, X., Chen, L., Lian, J., & Xie, X. (2021, July). Self-supervised graph learning for recommendation. In _Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. 726-735).](https://arxiv.org/pdf/2010.10783) | SIGIR | 2021 | [Python](https://github.com/wujcan/SGL) |

### Model-intrinsic
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| Fi-GNN | [Li, Z., Cui, Z., Wu, S., Zhang, X., & Wang, L. (2019, November). Fi-gnn: Modeling feature interactions via graph neural networks for ctr prediction. In _Proceedings of the 28th ACM International Conference on Information and Knowledge Management_ (pp. 539-548).](https://arxiv.org/pdf/1910.05552.pdf) | CIKM | 2019 | [Python](https://paperswithcode.com/paper/fi-gnn-modeling-feature-interactions-via) |
| PUP | [Zheng, Y., Gao, C., He, X., Li, Y., & Jin, D. (2020, April). Price-aware recommendation with graph convolutional networks. In _2020 IEEE 36th International Conference on Data Engineering (ICDE)_ (pp. 133-144). IEEE.](https://arxiv.org/pdf/2003.03975.pdf) | ICDE | 2020 | [Python](https://github.com/DavyMorgan/ICDE20-PUP) |
| L0-SIGN | [Su, Y., Zhang, R., Erfani, S., & Xu, Z. (2021, May). Detecting Beneficial Feature Interactions for Recommender Systems. In _Proceedings of the 34th AAAI Conference on Artificial Intelligence (AAAI)_.](https://arxiv.org/pdf/2008.00404.pdf) | AAAI | 2021 | [Python](https://github.com/ruizhang-ai/SIGN-Detecting-Beneficial-Feature-Interactions-for-Recommender-Systems) |
| DG-ENN | [Guo, W., Su, R., Tan, R., Guo, H., Zhang, Y., Liu, Z., ... & He, X. (2021). Dual Graph enhanced Embedding Neural Network for CTRPrediction. _arXiv preprint arXiv:2106.00314_.](https://arxiv.org/pdf/2106.00314.pdf) | KDD | 2021 | NA |
| SHCF | [Li, C., Hu, L., Shi, C., Song, G., & Lu, Y. (2021). Sequence-aware Heterogeneous Graph Neural Collaborative Filtering. In _Proceedings of the 2021 SIAM International Conference on Data Mining (SDM)_ (pp. 64-72). Society for Industrial and Applied Mathematics.](http://www.shichuan.org/doc/98.pdf) | SDM | 2021 | [Python](http://www.shichuan.org/dataset/SHCF.zip) |
| GCM | [Wu, J., He, X., Wang, X., Wang, Q., Chen, W., Lian, J., & Xie, X. (2020). Graph Convolution Machine for Context-aware Recommender System. _arXiv preprint arXiv:2001.11402_.](https://arxiv.org/pdf/2001.11402.pdf) | Frontiers of Computer Science | 2021 | [Python](https://github.com/wujcan/GCM) |

## Detection Methods
### Supervised
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| IRGPR | [Liu, W., Liu, Q., Tang, R., Chen, J., He, X., & Heng, P. A. (2020, October). Personalized Re-ranking with Item Relationships for E-commerce. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 925-934).](https://dl.acm.org/doi/abs/10.1145/3340531.3412332) | CIKM | 2020 | NA |

### Semi Supervised
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| IRGPR | [Liu, W., Liu, Q., Tang, R., Chen, J., He, X., & Heng, P. A. (2020, October). Personalized Re-ranking with Item Relationships for E-commerce. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 925-934).](https://dl.acm.org/doi/abs/10.1145/3340531.3412332) | CIKM | 2020 | NA |

### UnSupervised
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| IRGPR | [Liu, W., Liu, Q., Tang, R., Chen, J., He, X., & Heng, P. A. (2020, October). Personalized Re-ranking with Item Relationships for E-commerce. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 925-934).](https://dl.acm.org/doi/abs/10.1145/3340531.3412332) | CIKM | 2020 | NA |

Thank you for your reading.


