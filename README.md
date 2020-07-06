# Facet-Aware Evaluation for Extractive Summarization
This repo provides the annotated data and a self-contained demo for the paper ["Facet-Aware Evaluation for Extractive Summarization"](https://arxiv.org/abs/1908.10383), ACL 2020.

## Abstract
Commonly adopted metrics for extractive summarization focus on lexical overlap at the token level. In this paper, we present a facet-aware evaluation setup for better assessment of the information coverage in extracted summaries. Specifically, we treat each sentence in the reference summary as a facet, identify the sentences in the document that express the semantics of each facet as support sentences of the facet, and automatically evaluate extractive summarization methods by comparing the indices of extracted sentences and support sentences of all the facets in the reference summary. To facilitate this new evaluation setup, we construct an extractive version of the CNN/Daily Mail dataset and perform a thorough quantitative investigation, through which we demonstrate that facet-aware evaluation manifests better correlation with human judgment than ROUGE, enables fine-grained evaluation as well as comparative analysis, and reveals valuable insights of state-of-the-art summarization methods.

## Instructions

`facet_aware_eval.ipynb` illustrates how to use the annotated data for facet-aware evaluation. The raw extracted summaries are first mapped back to sentence indices and then compared with the indices of support sentences.

`data/*` contains files used in the notebook demo.

`output/*` contains human-readable plain text of the annotation results.



Please cite the following paper if you use our data. Thank you!

```
@inproceedings{mao-etal-2020-facet,
    title = "Facet-Aware Evaluation for Extractive Summarization",
    author = "Mao, Yuning  and
      Liu, Liyuan  and
      Zhu, Qi  and
      Ren, Xiang  and
      Han, Jiawei",
    booktitle = "Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics",
    month = jul,
    year = "2020",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2020.acl-main.445",
    pages = "4941--4957",
    abstract = "Commonly adopted metrics for extractive summarization focus on lexical overlap at the token level. In this paper, we present a facet-aware evaluation setup for better assessment of the information coverage in extracted summaries. Specifically, we treat each sentence in the reference summary as a \textit{facet}, identify the sentences in the document that express the semantics of each facet as \textit{support sentences} of the facet, and automatically evaluate extractive summarization methods by comparing the indices of extracted sentences and support sentences of all the facets in the reference summary. To facilitate this new evaluation setup, we construct an extractive version of the CNN/Daily Mail dataset and perform a thorough quantitative investigation, through which we demonstrate that facet-aware evaluation manifests better correlation with human judgment than ROUGE, enables fine-grained evaluation as well as comparative analysis, and reveals valuable insights of state-of-the-art summarization methods. Data can be found at \url{https://github.com/morningmoni/FAR}.",
}
```
