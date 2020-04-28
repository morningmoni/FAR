# Facet-Aware Evaluation for Extractive Summarization
This repo provides the annotated data and a self-contained demo for the paper ["Facet-Aware Evaluation for Extractive Summarization"](https://arxiv.org/abs/1908.10383), ACL 2020.



## Instructions

`facet_aware_eval.ipynb` illustrates how to use the annotated data for facet-aware evaluation. The raw extracted summaries are first mapped back to sentence indices and then compared with the indices of support sentences.

`data/*` contains files used in the notebook demo.

`output/*` contains human-readable plain text of the annotation results.



Please cite the following paper if you use our data. Thank you!

```
@article{mao2019facet,
  title={Facet-Aware Evaluation for Extractive Text Summarization},
  author={Mao, Yuning and Liu, Liyuan and Zhu, Qi and Ren, Xiang and Han, Jiawei},
  journal={arXiv preprint arXiv:1908.10383},
  year={2019}
}
```