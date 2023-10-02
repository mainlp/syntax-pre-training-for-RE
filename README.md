# Syntax pre-training for RE

This repository contains the data and code for the following paper:

Elisa Bassignana, Filip Ginter, Sampo Pyysalo, Rob van der Goot, and Barbara Plank. 2023. [Silver Syntax Pre-training for Cross-Domain Relation Extraction](https://aclanthology.org/2023.findings-acl.436.pdf). In Findings of the Association for Computational Linguistics: ACL 2023.

In order to reproduce the experiments in the paper
- download the CrossRE dataset from [HERE](https://github.com/mainlp/CrossRE)
- install the dependency packages using the command `pip install -r requirements.txt`
- run the command `./run.sh`

## Cite
If you use the code from this repository please include the following reference:
```
@inproceedings{bassignana-etal-2023-silver,
    title = "Silver Syntax Pre-training for Cross-Domain Relation Extraction",
    author = "Bassignana, Elisa  and
      Ginter, Filip  and
      Pyysalo, Sampo  and
      van der Goot, Rob  and
      Plank, Barbara",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-acl.436",
    doi = "10.18653/v1/2023.findings-acl.436",
    pages = "6984--6993",
    abstract = "Relation Extraction (RE) remains a challenging task, especially when considering realistic out-of-domain evaluations. One of the main reasons for this is the limited training size of current RE datasets: obtaining high-quality (manually annotated) data is extremely expensive and cannot realistically be repeated for each new domain. An intermediate training step on data from related tasks has shown to be beneficial across many NLP tasks. However, this setup still requires supplementary annotated data, which is often not available. In this paper, we investigate intermediate pre-training specifically for RE. We exploit the affinity between syntactic structure and semantic RE, and identify the syntactic relations which are closely related to RE by being on the shortest dependency path between two entities. We then take advantage of the high accuracy of current syntactic parsers in order to automatically obtain large amounts of low-cost pre-training data. By pre-training our RE model on the relevant syntactic relations, we are able to outperform the baseline in five out of six cross-domain setups, without any additional annotated data.",
}

```
