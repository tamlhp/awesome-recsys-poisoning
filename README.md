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
| MI-1 | [Bo Li, Yining Wang, Aarti Singh, and Yevgeniy Vorobeychik. 2016. Data poisoning attacks on factorization-based collaborative filtering. Advances in neural information processing systems 29 (2016), 1885–1893.](https://proceedings.neurips.cc/paper/2016/hash/83fa5a432ae55c253d0e60dbfa716723-Abstract.html) | NIPS | 2016 | [Python](#) |
| MI-2 | [Guolei Yang, Neil Zhenqiang Gong, and Ying Cai. 2017. Fake Co-visitation Injection Attacks to Recommender Systems. In NDSS.](https://people.duke.edu/~zg70/papers/ndss17-attackRS.pdf) | NDSS | 2017 | [Python](#) |
| MI-3 | [Minghong Fang, Guolei Yang, Neil Zhenqiang Gong, and Jia Liu. 2018. Poisoning attacks to graph-based recommender systems. In Proceedings of the 34th Annual Computer Security Applications Conference. 381–392.](https://dl.acm.org/doi/10.1145/3274694.3274706) | ACSAC | 2018 | [Python](#) |
| MI-4 | [Konstantina Christakopoulou and Arindam Banerjee. 2019. Adversarial attacks on an oblivious recommender. In Proceedings of the 13th ACM Conference on Recommender Systems. 322–330.](https://dl.acm.org/doi/10.1145/3298689.3347031) | RecSys | 2019 | NA |
| MI-5 | [Rui Hu, Yuanxiong Guo, Miao Pan, and Yanmin Gong. 2019. Targeted poisoning attacks on social recommender systems. In 2019 IEEE Global Communications Conference (GLOBECOM). IEEE, 1–6.](https://ieeexplore.ieee.org/document/9013539) | GLOBECOM | 2019 | [Python](#) |
| MI-6 | [Huiyuan Chen and Jing Li. 2019. Data poisoning attacks on cross-domain recommendation. In Proceedings of the 28th ACM International Conference on Information and Knowledge Management. 2177–2180.](https://dl.acm.org/doi/10.1145/3357384.3358116) | CIKM | 2019 | [Python](#) |
| MI-7 | [Hengtong Zhang, Yaliang Li, Bolin Ding, and Jing Gao. 2020. Practical data poisoning attack against next-item recommendation. In Proceedings of The Web Conference 2020. 2458–2464.](https://dl.acm.org/doi/10.1145/3366423.3379992) | WWW | 2020 | [Python](#) |
| MI-8 | [Minghong Fang, Neil Zhenqiang Gong, and Jia Liu. 2020. Influence function based data poisoning attacks to top-n recommender systems. In Proceedings of The Web Conference 2020. 3019–3025.](https://dl.acm.org/doi/10.1145/3366423.3380072) | WWW | 2020 | [Python](#) |
| MI-9 | [Liang Chen, Yangjun Xu, Fenfang Xie, Min Huang, and Zibin Zheng. 2021. Data poisoning attacks on neighborhoodbased recommender systems. Transactions on Emerging Telecommunications Technologies 32, 6 (2021), e3872.](https://onlinelibrary.wiley.com/doi/full/10.1002/ett.3872) | ETT | 2021 | [Python](#) |
| MI-10 | [Hengtong Zhang, Changxin Tian, Yaliang Li, Lu Su, Nan Yang, Wayne Xin Zhao, and Jing Gao. 2021. Data Poisoning Attack against Recommender System Using Incomplete and Perturbed Data. In Proceedings of the 27th ACM SIGKDD Conference on Knowledge Discovery & Data Mining. 2154–2164.](https://dl.acm.org/doi/10.1145/3447548.3467233) | KDD | 2021 | [Python](#) |
| MI-11 | [Zhenrui Yue, Zhankui He, Huimin Zeng, and Julian McAuley. 2021. Black-Box Attacks on Sequential Recommenders via Data-Free Model Extraction. In Fifteenth ACM Conference on Recommender Systems. 44–54.](https://dl.acm.org/doi/10.1145/3460231.3474275) | RecSys | 2021 | [Python](#) |
| MI-12 | [Zih-Wun Wu, Chiao-Ting Chen, and Szu-Hao Huang. 2021. Poisoning attacks against knowledge graph-based recommendation systems using deep reinforcement learning. Neural Computing and Applications (2021), 1–19.](https://dl.acm.org/doi/abs/10.1007/s00521-021-06573-8) | Neural. Comput. Appl. | 2021 | [Python](#) |
| MI-13 | [Zhuoran Liu and Martha Larson. 2021. Adversarial Item Promotion: Vulnerabilities at the Core of Top-N Recommenders that Use Images to Address Cold Start. In Proceedings of the Web Conference 2021. 3590–3602.](https://dl.acm.org/doi/10.1145/3442381.3449891) | WWW | 2021 | [Python](#) |
| MI-14 | [Hai Huang, Jiaming Mu, Neil Zhenqiang Gong, Qi Li, Bin Liu, and Mingwei Xu. 2021. Data poisoning attacks to deep learning based recommender systems. arXiv preprint arXiv:2101.02644 (2021). [60] Keman Huang, Michael Siegel, and Stuart Madnick. 2018. Systematically underst](https://arxiv.org/pdf/2012.10544.pdf) | arXiv | 2021 | [Python](#) |
| MI-15 | [Shijie Zhang, Hongzhi Yin, Tong Chen, Zi Huang, Quoc Viet Hung Nguyen, and Lizhen Cui. 2021. PipAttack: Poisoning Federated Recommender Systems forManipulating Item Promotion. arXiv preprint arXiv:2110.10926 (2021).](https://dl.acm.org/doi/10.1145/3488560.3498386) | WSDM | 2022 | [Python](#) |

## Detection Methods
### Supervised
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| CM-1 | [Paul-Alexandru Chirita, Wolfgang Nejdl, and Cristian Zamfir. 2005. Preventing shilling attacks in online recommender systems. In Proceedings of the 7th annual ACM international workshop on Web information and data management. 67–74.](https://dl.acm.org/doi/10.1145/1097047.1097061) | WIDM | 2005 | NA |
| CM-2 | [Robin Burke, Bamshad Mobasher, Chad Williams, and Runa Bhaumik. 2006. Classification features for attack detection in collaborative recommender systems. In Proceedings of the 12th ACM SIGKDD international conference on Knowledge discovery and data mining. 542–547.](https://dl.acm.org/doi/10.1145/1150402.1150465) | KDD | 2006 | NA |
| CM-3 | [Robin Burke, Bamshad Mobasher, Chad Williams, and Runa Bhaumik. 2006. Detecting profile injection attacks in collaborative recommender systems. In The 8th IEEE International Conference on E-Commerce Technology and The 3rd IEEE International Conference on Enterprise Computing, E-Commerce, and E-Services (CEC/EEE’06). IEEE, 23–23.](https://dl.acm.org/doi/10.1109/CEC-EEE.2006.34) | CEC-EEE | 2006 | NA |
| CM-4 | [Bamshad Mobasher, Robin Burke, Runa Bhaumik, and Chad Williams. 2007. Toward trustworthy recommender systems: An analysis of attack models and algorithm robustness. ACM Transactions on Internet Technology (TOIT) 7, 4 (2007), 23–es.](https://dl.acm.org/doi/10.1145/1278366.1278372) | TOIT | 2007 | NA |
| CM-5 | [Fuzhi Zhang and Quanqiang Zhou. 2012. A Meta-learning-based Approach for Detecting Profile Injection Attacks in Collaborative Recommender Systems. J. Comput. 7, 1 (2012), 226–234](http://www.jcomputers.us/vol7/jcp0701-26.pdf) | J. Comput. | 2012 | NA |
| CM-6 | [Fuzhi Zhang and Quanqiang Zhou. 2014. HHT–SVM: An online method for detecting profile injection attacks in collaborative recommender systems. Knowledge-Based Systems 65 (2014), 96–105.](https://www.sciencedirect.com/science/article/pii/S0950705114001427) | KBS | 2014 | NA |
| CM-7 | [Wei Zhou, Junhao Wen, Qingyu Xiong, Min Gao, and Jun Zeng. 2016. SVM-TIA a shilling attack detection method based on SVM and target item analysis in recommender systems. Neurocomputing 210 (2016), 197–205.](https://dl.acm.org/doi/10.1016/j.neucom.2015.12.137) | J. Neucom. | 2016 | NA |
| CM-8 | [Zhihai Yang, Lin Xu, Zhongmin Cai, and Zongben Xu. 2016. Re-scale AdaBoost for attack detection in collaborative filtering recommender systems. Knowledge-Based Systems 100 (2016), 74–88.](https://www.sciencedirect.com/science/article/pii/S0950705116000861) | KBS | 2016 | NA |
| CM-9 | [Yaojun Hao, Fuzhi Zhang, Jian Wang, Qingshan Zhao, and Jianfang Cao. 2019. Detecting shilling attacks with automatic features from multiple views. Security and Communication Networks 2019 (2019).](https://www.hindawi.com/journals/scn/2019/6523183/) | Secur. Commun. Netw. | 2019 | NA |
| CM-10 | [Yishu Xu and Fuzhi Zhang. 2019. Detecting shilling attacks in social recommender systems based on time series analysis and trust features. Knowledge-Based Systems 178 (2019), 25–47.](https://dl.acm.org/doi/abs/10.1016/j.knosys.2019.04.012) | KBS | 2019 | NA |
| CM-11 | [Quanqiang Zhou, Jinxia Wu, and Liangliang Duan. 2020. Recommendation attack detection based on deep learning. Journal of Information Security and Applications 52 (2020), 102493.](https://www.sciencedirect.com/science/article/pii/S2214212619306131) | JISA | 2020 | NA |

### Semi Supervised
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| IRGPR | [Liu, W., Liu, Q., Tang, R., Chen, J., He, X., & Heng, P. A. (2020, October). Personalized Re-ranking with Item Relationships for E-commerce. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 925-934).](https://dl.acm.org/doi/abs/10.1145/3340531.3412332) | CIKM | 2020 | NA |

### UnSupervised
| **Name** | **Paper** | **Venue** | **Year** | **Code** |
| --- | --- | --- | --- | --- |
| IRGPR | [Liu, W., Liu, Q., Tang, R., Chen, J., He, X., & Heng, P. A. (2020, October). Personalized Re-ranking with Item Relationships for E-commerce. In _Proceedings of the 29th ACM International Conference on Information & Knowledge Management_ (pp. 925-934).](https://dl.acm.org/doi/abs/10.1145/3340531.3412332) | CIKM | 2020 | NA |



