# A Survey of Poisoning Attacks and Countermeasures in Recommender Systems

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![arXiv](https://img.shields.io/badge/arXiv-2404.14942-b31b1b.svg)](https://arxiv.org/abs/2404.14942)
[![Website](https://img.shields.io/website?down_color=lightgrey&down_message=offline&label=Official%20Website&up_color=green&up_message=online&url=https%3A%2F%2Fawesome-recsys-poisoning.github.io%2F)](https://awesome-recsys-poisoning.github.io/)
![GitHub stars](https://img.shields.io/github/stars/tamlhp/awesome-recsys-poisoning?color=yellow&label=Stars)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Ftamlhp%2Fawesome-recsys-poisoning%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
<img src="https://img.shields.io/badge/Contributions-Welcome-278ea5" alt="Contrib"/>

A repository of poison attacks against recommender systems, as well as their countermeasures. This repository is associated with our systematic review, entitled **Manipulating Recommender Systems: A Survey of Poisoning Attacks and Countermeasures**. 


- [Existing Surveys](#existing-surveys)
- [Taxonomy](#Taxonomy)
- [Poison Attacks](#Poison-Attacks)
   - [Model-agnostic](#Model-agnostic)
   - [Model-intrinsic](#Model-intrinsic)
- [Countermeasures](#Countermeasures)
   - [Supervised](#Supervised)
   - [Semi Supervised](#Semi-Supervised)
   - [Unsupervised](#Unsupervised)
- [Datasets](#datasets)

A sortable version is available here: https://awesome-recsys-poisoning.github.io/

Please read and cite our paper: [![arXiv](https://img.shields.io/badge/arXiv-2404.14942-b31b1b.svg)](https://arxiv.org/abs/2404.14942)

>Nguyen, T.T., Nguyen, Q.V.H., Nguyen, T.T., Huynh, T.T., Nguyen, T.T., Weidlich, M. and Yin, H., 2024. Manipulating Recommender Systems: A Survey of Poisoning Attacks and Countermeasures. arXiv preprint arXiv:2404.14942.

## Citation

```
@article{nguyen2024manipulating,
  title={Manipulating Recommender Systems: A Survey of Poisoning Attacks and Countermeasures},
  author={Nguyen, Thanh Toan and Nguyen, Quoc Viet Hung and Nguyen, Thanh Tam and Huynh, Thanh Trung and Nguyen, Thanh Thi and Weidlich, Matthias and Yin, Hongzhi},
  journal={arXiv preprint arXiv:2404.14942},
  year={2024}
}
```

----------

## Existing Surveys

| **Paper Title** | **Venue** | **Year** | **Note** |
| --------------- | ---- | ---- | ---- | 
| [Poisoning Attacks against Recommender Systems: A Survey](https://arxiv.org/abs/2401.01527) | arXiv | 2024 | Focus on benchmarking |
| [Manipulating vulnerability: Poisoning attacks and countermeasures in federated cloud–edge–client learning for image classification](https://www.sciencedirect.com/science/article/pii/S0950705122011650) | KBS | 2023 | Focus on federated learning |
| [A Survey on Data Poisoning Attacks and Defenses](https://ieeexplore.ieee.org/abstract/document/9900151) | DSC | 2022 | Not focus on recommender systems |
| [A survey of attack detection approaches in collaborative filtering recommender systems](https://link.springer.com/article/10.1007/s10462-020-09898-3) | Artificial Intelligence Review | 2021 | Classic heuristic attacks only |
| [Understanding Shilling Attacks and Their Detection Traits: A Comprehensive Survey](https://ieeexplore.ieee.org/abstract/document/9205244) | IEEE Access | 2020 | Classic heuristic attacks only |
| [Shilling attacks against collaborative recommender systems: a review](https://link.springer.com/article/10.1007/s10462-018-9655-x) | Artificial Intelligence Review  | 2020 | Classic heuristic attacks only |
| [A Comparative Study on Shilling Detection Methods for Trustworthy Recommendations](https://link.springer.com/article/10.1007/s11518-018-5374-8) | SESC |  2018 | Classic heuristic attacks only |
| [A comparative study of shilling attack detectors for recommender systems](https://ieeexplore.ieee.org/abstract/document/7170330) | ICSSSM | 2015 | Classic heuristic attacks only |

----------

## Taxonomy

[![taxonomy](figs/taxonomy.png)](https://arxiv.org/abs/2404.14942)


----------


## Poison Attacks

Poisoning attacks are the process of tampering with the training data of a  machine learning (ML) model in order to corrupt its availability and integrity. Below figure presents the typical process of a poisoning attack  compared to the normal learning process. In the latter case, an ML  model is trained based on data, which is subsequently used to derive a 
recommendation. As such, the quality of the ML model depends on the quality of the data used for training. In a poisoning attack, data is injected into the training process, and hence the model, to produce unintended or harmful conclusions. 
[![Attack-Process](figs/attack_process.png)](https://arxiv.org/abs/2404.14942)


| **Paper** | **Venue** | **Year** | **Type** | **Data** | **Code** |
| --- | --- | --- | --- | --- | --- |
| [Poisoning GNN-based recommender systems with generative surrogate-based attacks](https://doi.org/10.1145/3567420) | ACM TOIS | 2023 | Model-intrinsic | [FR](#datasets), [ML](#datasets), [AMCP](#datasets), [LF](#datasets) | - |
| [Shilling Black-Box Recommender Systems by Learning to Generate Fake User Profiles](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9806457) | IEEE Trans. Neural Netw. Learn. Syst | 2022 | Model-agnostic | [ML](#datasets), [FT](#datasets), [YE](#datasets), [AAT](#datasets) | - |
| [Knowledge enhanced Black-box Attacks for Recommendations](https://dl.acm.org/doi/abs/10.1145/3534678.3539359) | KDD | 2022 | Model-agnostic | [ML](#datasets), [BC](#datasets), [LA](#datasets)  | - |
| [LOKI: A Practical Data Poisoning Attack Frameworkagainst Next Item Recommendations](https://ieeexplore.ieee.org/document/9806383) | TKDE | 2022 | Model-agnostic | [ABT](#datasets), [St](#datasets),[GOW](#datasets)  | - |
| [Pipattack: Poisoning federated recommender systems for manipulating item promotion](https://dl.acm.org/doi/10.1145/3488560.3498386) | WSDM | 2022 | Model-intrinsic | [ML](#datasets), [AMCP](#datasets) | - |
| [Poisoning Deep Learning based Recommender Model in Federated Learning Scenarios](https://www.ijcai.org/proceedings/2022/0306.pdf) | IJCAI | 2022 | Model-intrinsic | [ML](#datasets), [ADM](#datasets) | [Python](https://github.com/rdz98/PoisonFedDLRS) |
| [FedAttack: Effective and Covert Poisoning Attack on Federated Recommendation via Hard Sampling](https://arxiv.org/pdf/2202.04975.pdf) | Arxiv | 2022 | Model-intrinsic | [ML](#datasets), [ABT](#datasets)  | [Python](https://github.com/wuch15/FedAttack) |
| [UA-FedRec: Untargeted Attack on Federated News Recommendation](https://arxiv.org/abs/2202.06701) | Arxiv | 2022 | Model-intrinsic | [MIND](#datasets), [Feeds](#datasets)  | [Python](https://github.com/yjw1029/UA-FedRec) | - |
| [Triple Adversarial Learning for Influence based Poisoning Attack in Recommender Systems](https://dl.acm.org/doi/10.1145/3447548.3467335) | KDD | 2021 | Model-agnostic |  [ML](#datasets), [FT](#datasets) | [Python](https://github.com/Daftstone/TrialAttack) |
| [Reverse Attack: Black-box Attacks on Collaborative Recommendation](https://dl.acm.org/doi/10.1145/3460120.3484805) | CSS | 2021 | Model-agnostic |  [ML](#datasets), [NF](#datasets), [AMB & ADM](#datasets), [TW](#datasets), [G+](#datasets), [CIT](#datasets)  | - |
| [Attacking Black-box Recommendations via Copying Cross-domain User Profiles](https://ieeexplore.ieee.org/document/9458627) | ICDE | 2021 | Model-agnostic | [ML](#datasets), [NF](#datasets) | - |
| [Simulating real profiles for shilling attacks: A generative approach](https://www.sciencedirect.com/science/article/pii/S0950705121006523) | KBS | 2021 | Model-agnostic | [ML](#datasets) | - |
| [Ready for emerging threats to recommender systems? A graph convolution-based generative shilling attack](https://www.sciencedirect.com/science/article/pii/S0020025521007313) | IS | 2021 | Model-agnostic | [DB](#datasets), [CI](#datasets) | [Python](https://github.com/silentair/GOAT/tree/7c1747d40f9bc2b5b0ac5035770b3e9f2bbd5211) |
| [Data poisoning attacks on neighborhoodbased recommender systems](https://onlinelibrary.wiley.com/doi/full/10.1002/ett.3872) | ETT | 2021 | Model-intrinsic | [FT](#datasets), [ML](#datasets), [AMV](#datasets) | - |
| [Data Poisoning Attack against Recommender System Using Incomplete and Perturbed Data](https://dl.acm.org/doi/10.1145/3447548.3467233) | KDD | 2021 | Model-intrinsic | [ML](#datasets), [AIV](#datasets) | - |
| [Black-Box Attacks on Sequential Recommenders via Data-Free Model Extraction](https://dl.acm.org/doi/10.1145/3460231.3474275) | RecSys | 2021 | Model-intrinsic | [ML](#datasets),[St](#datasets), [ABT](#datasets) | [Python](https://github.com/Yueeeeeeee/RecSys-Extraction-Attack) |
| [Poisoning attacks against knowledge graph-based recommendation systems using deep reinforcement learning](https://dl.acm.org/doi/abs/10.1007/s00521-021-06573-8) | Neural. Comput. Appl. | 2021 | Model-intrinsic | [ML](#datasets), [FTr](#) | - |
| [Adversarial Item Promotion: Vulnerabilities at the Core of Top-N Recommenders that Use Images to Address Cold Start](https://dl.acm.org/doi/10.1145/3442381.3449891) | WWW | 2021 | Model-intrinsic | [AMMN](#datasets), [TC](#datasets) | [Python](https://github.com/liuzrcc/AIP) |
| [Data poisoning attacks to deep learning based recommender systems](https://arxiv.org/pdf/2012.10544.pdf) | arXiv | 2021 | Model-intrinsic | [ML](#datasets), [LA](#datasets) | - |
| [Practical data poisoning attack against next-item recommendation](https://dl.acm.org/doi/10.1145/3366423.3379992) | WWW | 2020 | Model-intrinsic | [ABT](#datasets) | - |
| [Influence function based data poisoning attacks to top-n recommender systems](https://dl.acm.org/doi/10.1145/3366423.3380072) | WWW | 2020 | Model-intrinsic | [YE](#datasets), [ADM](#datasets) | - |
| [Attacking recommender systems with augmented user profiles](https://dl.acm.org/doi/10.1145/3340531.3411884) | CIKM | 2020 | Model-agnostic |  [ML](#datasets), [FT](#datasets), [AAT](#datasets) | - |
| [Poisonrec: an adaptive data poisoning framework for attacking black-box recommender systems](https://ieeexplore.ieee.org/document/9101655/) | ICDE | 2020 | Model-agnostic | [St](#datasets), [AMCP](#datasets), [ML](#datasets) | - |
| [Revisiting adversarially learned injection attacks against recommender systems](https://dl.acm.org/doi/10.1145/3383313.3412243) | RecSys | 2020 | Model-agnostic | [GOW](#datasets) | [Python](https://github.com/graytowne/revisit_adv_rec) |
| [Adversarial attacks on an oblivious recommender](https://dl.acm.org/doi/10.1145/3298689.3347031) | RecSys | 2019 | Model-intrinsic | [ML](#datasets) | - |
| [Targeted poisoning attacks on social recommender systems](https://ieeexplore.ieee.org/document/9013539) | GLOBECOM | 2019 | Model-intrinsic | [FT](#datasets) | - |
| [Data poisoning attacks on cross-domain recommendation](https://dl.acm.org/doi/10.1145/3357384.3358116) | CIKM | 2019 | Model-intrinsic | [NF](#datasets), [ML](#datasets) | - |
| [Poisoning attacks to graph-based recommender systems](https://dl.acm.org/doi/10.1145/3274694.3274706) | ACSAC | 2018 | Model-intrinsic | [ML](#datasets), [AIV](#datasets) | - |
| [Fake Co-visitation Injection Attacks to Recommender Systems](https://people.duke.edu/~zg70/papers/ndss17-attackRS.pdf) | NDSS | 2017 | Model-intrinsic | [YT](#datasets), [eB](#datasets), [AMV](#datasets), [YE](#datasets), [LI](#datasets) | - |
| [Data poisoning attacks on factorization-based collaborative filtering](https://proceedings.neurips.cc/paper/2016/hash/83fa5a432ae55c253d0e60dbfa716723-Abstract.html) | NIPS | 2016 | Model-intrinsic | [ML](#datasets) | [Python](https://github.com/fuying-wang/Data-poisoning-attacks-on-factorization-based-collaborative-filtering) |
| [Shilling recommender systems for fun and profit](https://dl.acm.org/doi/10.1145/988672.988726) | WWW | 2004 | Model-agnostic | [ML](#datasets) |

----------

## Countermeasures
In this section, we review detection methods in more detail, starting with supervised methods, before turning to semi-supervised methods and unsupervised methods


| **Paper** | **Venue** | **Year** | **Type** | **Data** | **Code** |
| --- | --- | --- | --- | --- | --- |
| [Anti-FakeU: Defending Shilling Attacks on Graph Neural Network based Recommender Model](https://doi.org/10.1145/3543507.3583289) | WWW | 2023 | UnSupervised | [GOW](#datasets), [Yelp](#datasets) | - |
| [An unsupervised detection method for shilling attacks based on deep learning and community detection](https://dl.acm.org/doi/abs/10.1007/s00500-020-05162-6) | Soft Comput. | 2021 | UnSupervised | [NF](#datasets), [AMV](#datasets) | - |
| [Identification of Malicious Injection Attacks in Dense Rating and Co-Visitation Behaviors](https://dl.acm.org/doi/10.1109/TIFS.2020.3016827) | TIFS | 2020 | UnSupervised | [ML](#datasets), [AMB](#datasets), [LT](#datasets), [Trip](#datasets) | - |
| [Recommendation attack detection based on deep learning](https://www.sciencedirect.com/science/article/pii/S2214212619306131) | JISA | 2020 | Supervised | [ML](#datasets) | - |
| [Detecting shilling attacks with automatic features from multiple views](https://www.hindawi.com/journals/scn/2019/6523183/) | Secur. Commun. Netw. | 2019 | Supervised | [NF](#datasets), [ML](#datasets), [AMV](#datasets) | - |
| [Detecting shilling attacks in social recommender systems based on time series analysis and trust features](https://dl.acm.org/doi/abs/10.1016/j.knosys.2019.04.012) | KBS | 2019 | Supervised | [CI](#datasets), [EP](#datasets) | - |
| [BS-SC: An Unsupervised Approach for Detecting Shilling Profiles in Collaborative Recommender Systems](https://ieeexplore.ieee.org/document/8862947) | TKDE | 2019 | UnSupervised | [SYN](#datasets), [AMP](#datasets) | - |
| [Detecting shilling attacks in recommender systems based on analysis of user rating behavior](https://dl.acm.org/doi/abs/10.1016/j.knosys.2019.04.001) | KBS | 2019 | UnSupervised | [NF](#datasets), [ML](#datasets), [AMP](#datasets) | - |
| [Trustworthy and profit: A new value-based neighbor selection method in recommender systems under shilling attacks](https://dl.acm.org/doi/10.1016/j.dss.2019.113112) | DSS | 2019 | UnSupervised | [BC](#datasets), [AMB](#datasets) | - |
| [Quick and accurate attack detection in recommender systems through user attributes](https://dl.acm.org/doi/10.1145/3298689.3347050) | RecSys | 2019 | UnSupervised | [ML](#datasets) | - |
| [UD-HMM: An unsupervised method for shilling attack detection based on hidden Markov model and hierarchical clustering](https://www.sciencedirect.com/science/article/pii/S0950705118300959) | KBS | 2018 | UnSupervised | [ML](#datasets), [NF](#datasets), [AMP](#datasets) | - |
| [Shilling attack detection for recommender systems based on credibility of group users and rating time series](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0196533) | Plos One | 2018 | UnSupervised | [ML](#datasets) | - |
| [Spotting anomalous ratings for rating systems by analyzing target users and items](https://dl.acm.org/doi/abs/10.1016/j.neucom.2017.02.052) | Neurocomputing | 2017 | UnSupervised | [ML](#datasets), [AMP](#datasets) | - | 
| [Estimating user behavior toward detecting anomalous ratings in rating systems](https://dl.acm.org/doi/10.1016/j.knosys.2016.08.011) | KBS | 2016 | UnSupervised | [ML](#datasets) | - |
| [SVM-TIA a shilling attack detection method based on SVM and target item analysis in recommender systems](https://dl.acm.org/doi/10.1016/j.neucom.2015.12.137) | J. Neucom. | 2016 | Supervised | [ML](#datasets) | - |
| [Re-scale AdaBoost for attack detection in collaborative filtering recommender systems](https://www.sciencedirect.com/science/article/pii/S0950705116000861) | KBS | 2016 | Supervised | [ML](#datasets) | - |
| [Catch the black sheep: unified framework for shilling attack detection based on fraudulent action propagation](https://dl.acm.org/doi/10.5555/2832581.2832585) | IJCAI | 2015 | UnSupervised | [AMV](#datasets) | - |
| [Shilling attacks detection in recommender systems based on target item analysis](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0130968) | Plos One | 2015 | UnSupervised | [ML](#datasets), [NF](#datasets), [EM](#datasets) | - |
| [A novel item anomaly detection approach against shilling attacks in collaborative recommendation systems using the dynamic time interval segmentation technique](https://dl.acm.org/doi/abs/10.1016/j.ins.2015.02.019) | IS | 2015 | UnSupervised | [ML](#datasets) | - |
| [A novel shilling attack detection method](https://www.sciencedirect.com/science/article/pii/S1877050914004347) | Procedia Comput. Sci. | 2014 | UnSupervised | [ML](#datasets) | - |
| [Detection of abnormal profiles on group attacks in recommender systems](https://dl.acm.org/doi/10.1145/2600428.2609483) | SIGIR | 2014 | UnSupervised | [NF](#datasets), [ML](#datasets), [EM](#datasets) | - |
| [HHT–SVM: An online method for detecting profile injection attacks in collaborative recommender systems](https://www.sciencedirect.com/science/article/pii/S0950705114001427) | KBS | 2014 | Supervised | [ML](#datasets) | - |
| [Shilling attack detection utilizing semi-supervised learning method for collaborative recommender system](https://link.springer.com/article/10.1007/s11280-012-0164-6) | WWW | 2013 | Semi Supervised | [ML](#datasets) | - |
| [𝛽P: A novel approach to filter out malicious rating profiles from recommender systems](https://dl.acm.org/doi/abs/10.1016/j.dss.2013.01.020) | DSS | 2013 | UnSupervised | [ML](#datasets) | - |
| [A Meta-learning-based Approach for Detecting Profile Injection Attacks in Collaborative Recommender Systems](http://www.jcomputers.us/vol7/jcp0701-26.pdf) | J. Comput. | 2012 | Supervised | [ML](#datasets) | - |
| [HySAD: A semi-supervised hybrid shilling attack detector for trustworthy product recommendation](https://dl.acm.org/doi/10.1145/2339530.2339684) | KDD | 2012 | Semi Supervised | [NF](#datasets), [ML](#datasets) | - |
| [A clustering approach to unsupervised attack detection in collaborative recommender systems](https://www.semanticscholar.org/paper/A-Clustering-Approach-to-Unsupervised-Attack-in-Bhaumik-Mobasher/5da857634542a5d2e9b67158fbe2d93afc99412c) | ICDATA | 2011 | UnSupervised | [ML](#datasets) | - |
| [Unsupervised strategies for shilling detection and robust collaborative filtering](https://link.springer.com/article/10.1007/s11257-008-9050-4) | User Model. User-Adapt. Interact. | 2009 | UnSupervised | [ML](#datasets) | - |
| [Unsupervised retrieval of attack profiles in collaborative recommender systems](https://dl.acm.org/doi/10.1145/1454008.1454034) | RecSys | 2008 | UnSupervised | [ML](#datasets) | - |
| [Lies and propaganda: detecting spam users in collaborative filtering](https://dl.acm.org/doi/10.1145/1216295.1216307) | IUI | 2007 | UnSupervised | [ML](#datasets) | - |
| [Toward trustworthy recommender systems: An analysis of attack models and algorithm robustness](https://dl.acm.org/doi/10.1145/1278366.1278372) | TOIT | 2007 | Supervised | [ML](#datasets) | - |
| [Classification features for attack detection in collaborative recommender systems](https://dl.acm.org/doi/10.1145/1150402.1150465) | KDD | 2006 | Supervised | [ML](#datasets) | - |
| [Detecting profile injection attacks in collaborative recommender systems](https://dl.acm.org/doi/10.1109/CEC-EEE.2006.34) | CEC-EEE | 2006 | Supervised | [ML](#datasets) | - |
| [Attack detection in time series for recommender systems](https://dl.acm.org/doi/10.1145/1150402.1150508) | KDD | 2006 | UnSupervised | [ML](#datasets) | - |
| [Preventing shilling attacks in online recommender systems](https://dl.acm.org/doi/10.1145/1097047.1097061) | WIDM | 2005 | Supervised | [ML](#datasets) | - |


----------

## Datasets

| Dataset | Name |
| :-- | --- |
| [AAT](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Automotive |
| [ABT](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Beauty |
| [ADM](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Digital Music |
| [AIV](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Instant Video |
| [AMB](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Book |
| [AMMN](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Men |
| [AMV](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Movie |
| [AMCP](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Cell-phone |
| [AMP](http://jmcauley.ucsd.edu/data/amazon/) | Amazon Product |
| [BC](https://www.kaggle.com/datasets/somnambwl/bookcrossing-dataset) | Book-Crossing |
| [CI](https://paperswithcode.com/dataset/ciao) | Ciao |
| [CIT](https://www.aminer.org/citation/) | Citation Network |
| [DB](https://www.kaggle.com/datasets/fengzhujoey/douban-datasetratingreviewside-information) | Douban |
| [eB](https://www.kaggle.com/datasets/promptcloud/ebay-product-listing-dataset) | eBay |
| [EM](https://grouplens.org/datasets/eachmovie/) | Eachmovie |
| [EP](http://www.cse.msu.edu/~tangjili/trust.html) | Epinions |
| [Feeds](https://github.com/yjw1029/UA-FedRec) | Microsoft news App |
| [FR](https://www.baltrunas.info/context-aware) | FRappe - Mobile App Recommendations |
| [FT](https://guoguibing.github.io/librec/datasets.html) | Film Trust |
| [Ftr](https://link.springer.com/article/10.1007/s00521-021-06573-8) | Fund Transactions |
| [G+](https://snap.stanford.edu/data/ego-Gplus.html) | Google+ |
| [GOW](http://snap.stanford.edu/data/loc-Gowalla.html) | Gowalla |
| [MIND](https://msnews.github.io/) | Microsoft News |
| [LA](http://millionsongdataset.com/lastfm/) | Last.fm |
| [LI](https://www.kaggle.com/datasets/killbot/linkedin) | Linkedin |
| [LT](https://www.librarything.com/tag/dataset) | LibraryThing |
| [ML](https://grouplens.org/datasets/movielens/100k/) | MovieLens |
| [NF](https://www.kaggle.com/datasets/netflix-inc/netflix-prize-data) | Netflix |
| [St](https://www.kaggle.com/datasets/tamber/steam-video-games) | Steam |
| [TC](https://www.tradesy.com/) | Tradesy |
| [Trip](https://www.kaggle.com/datasets/andrewmvd/trip-advisor-hotel-reviews) | TripAdvisor |
| [TW](https://anlab-kaist.github.io/traces/) | Twitter [[Code]](https://github.com/ANLAB-KAIST/traces) |
| [YE](https://www.kaggle.com/c/yelp-recruiting/data) | Yelp |
| [YT](https://www.kaggle.com/datasets/rsrishav/youtube-trending-video-dataset) | YouTube |
| [SYNC](#) | Synthetic datasets |


----------
**Disclaimer**

Feel free to contact us if you have any queries or exciting news. In addition, we welcome all researchers to contribute to this repository and further contribute to the knowledge of this field.

If you have some other related references, please feel free to create a Github issue with the paper information. We will gladly update the repos according to your suggestions. (You can also create pull requests, but it might take some time for us to do the merge)


[![HitCount](https://hits.dwyl.com/tamlhp/awesome-recsys-poisoning.svg?style=flat-square)](http://hits.dwyl.com/tamlhp/awesome-recsys-poisoning)
 ![visitors](https://visitor-badge.laobi.icu/badge?page_id=tamlhp.awesome-recsys-poisoning)


