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
| MA-1 | [Shyong K Lam and John Riedl. 2004. Shilling recommender systems for fun and profit. In Proceedings of the 13th international conference on World Wide Web. 393–402.](https://dl.acm.org/doi/10.1145/988672.988726) | WWW | 2004 | [Python](#) |
| MA-2 | [Junshuai Song, Zhao Li, Zehong Hu, Yucheng Wu, Zhenpeng Li, Jian Li, and Jun Gao. 2020. Poisonrec: an adaptive data poisoning framework for attacking black-box recommender systems. In 2020 IEEE 36th International Conference on Data Engineering (ICDE). IEEE, 157–168.](https://ieeexplore.ieee.org/document/9101655/) | ICDE | 2020 | NA |
| MA-3 | [Jiaxi Tang, Hongyi Wen, and Ke Wang. 2020. Revisiting adversarially learned injection attacks against recommender systems. In Fourteenth ACM Conference on Recommender Systems. 318–327.](https://dl.acm.org/doi/10.1145/3383313.3412243) | RecSys | 2020 | [Python](#) |
| MA-4 | [Chen Lin, Si Chen, Hui Li, Yanghua Xiao, Lianyun Li, and Qian Yang. 2020. Attacking recommender systems with augmented user profiles. In Proceedings of the 29th ACM International Conference on Information & Knowledge Management. 855–864.](https://dl.acm.org/doi/10.1145/3340531.3411884) | CIKM | 2020 | [Python](#) |
| MA-5 | [Chenwang Wu, Defu Lian, Yong Ge, Zhihao Zhu, and Enhong Chen. 2021. Triple Adversarial Learning for Influence based Poisoning Attack in Recommender Systems. In Proceedings of the 27th ACM SIGKDD Conference on Knowledge Discovery & Data Mining. 1830–1840.](https://dl.acm.org/doi/10.1145/3447548.3467335) | KDD | 2021 | [Python](#) |
| MA-6 | [Yihe Zhang, Xu Yuan, Jin Li, Jiadong Lou, Li Chen, and Nian-Feng Tzeng. 2021. Reverse Attack: Black-box Attacks on Collaborative Recommendation. In Proceedings of the 2021 ACM SIGSAC Conference on Computer and Communications Security. 51–68.](https://dl.acm.org/doi/10.1145/3460120.3484805) | CSS | 2021 | NA |
| MA-7 | [Wenqi Fan, Tyler Derr, Xiangyu Zhao, Yao Ma, Hui Liu, Jianping Wang, Jiliang Tang, and Qing Li. 2021. Attacking Black-box Recommendations via Copying Cross-domain User Profiles. In 2021 IEEE 37th International Conference on Data Engineering (ICDE). IEEE, 1583–1594.](https://ieeexplore.ieee.org/document/9458627) | ICDE | 2021 | [Python](#) |
| MA-8 | [Julio Barbieri, Leandro GM Alvim, Filipe Braida, and Geraldo Zimbrão. 2021. Simulating real profiles for shilling attacks: A generative approach. Knowledge-Based Systems 230 (2021), 107390.](https://www.sciencedirect.com/science/article/pii/S0950705121006523) | KBS | 2021 | [Python](#) |
| MA-9 | [Fan Wu, Min Gao, Junliang Yu, Zongwei Wang, Kecheng Liu, and Xu Wang. 2021. Ready for emerging threats to recommender systems? A graph convolution-based generative shilling attack. Information Sciences 578 (2021), 683–701.](https://www.sciencedirect.com/science/article/pii/S0020025521007313) | IS | 2021 | [Python](#) |


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


