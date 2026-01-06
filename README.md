# Detecting-Government-Linked-Intervention-Language-on-Weibo
Data
Place the following files in the project directory:

knownWeibos_zg.csv
KPR replication dataset of government-linked Weibo posts (positives).

user_posts.json
RUW dataset (UIUC), a collection of public Weibo posts about the Russia–Ukraine war (unlabeled).


Reproducing results (notebook workflow)
Run the notebook top-to-bottom. The notebook export is included as Detecting 50c on Weibo.ipynb.
Main steps:
Load and preprocess KPR positives
Load and preprocess RUW unlabeled posts
Train baselines (proxy task)
Two-step PU learning (main model)
Diagnostics and interpretation: KPR examples vs RUW high/low score examples, Time-series plots, mean score by user, top/bottom accounts by average score


Outputs
The notebook produces:
Tables of model comparisons (KPR recall, proxy metrics, RN consistency check)
A qualitative verification table (translated examples)
Time-series plots of daily volume and daily mean KPR-style score
Account-level rankings (top/bottom by average score)


Thank you! 
