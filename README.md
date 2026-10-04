# ZCAIGC-SongCi-Soundscapes
Official implementation of HSI-KMeans model and multimodal bio-psychological dataset (PPG-HRV, EDA, RIP, STAI-S, ROS) for AIGC-driven Song Ci restorative soundscapes.
AIGC-SongCi-Soundscapes/
├── README.md                     # 项目概述、依赖环境及复现步骤指南
├── LICENSE                       # 开源协议（建议选择 MIT 或 Apache-2.0）
├── requirements.txt              # 依赖库清单（pandas, numpy, scipy, scikit-learn, etc.）
├── models/
│   ├── bert_valence_filter.py    # f(V) 情感效价提取与安全熔断函数实现
│   ├── art_dcc_weights.py        # g(ART) 环境恢复力与 h(DCC) 动态演变计算
│   └── hsi_calculator.py         # HSI 综合疗愈指数加权总分计算脚本
├── clustering/
│   └── kmeans_elbow.py           # K-Means 聚类与肘部法则最优簇数识别 (K=4)
├── empirical_analysis/
│   ├── psychometrics_anova.py    # STAI-S、ROS 与 De Freitas 组间方差与协方差分析 (ANOVA/ANCOVA)
│   └── physio_processing.py      # RIP 呼吸变异性、HRV RMSSD 与 EDA SCL 特征提取
└── sample_data/
    ├── questionnaire_clean.csv   # 去除隐私信息的 1-60 号量表打分样本
    └── physio_extracted.csv      # 多模态生理时域与频域指标汇总表
